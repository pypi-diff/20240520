# Comparing `tmp/cmrsim-0.30.tar.gz` & `tmp/cmrsim-0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmrsim-0.30.tar", last modified: Mon Apr 15 12:19:29 2024, max compression
+gzip compressed data, was "cmrsim-0.31.tar", last modified: Mon May 20 10:33:14 2024, max compression
```

## Comparing `cmrsim-0.30.tar` & `cmrsim-0.31.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.836124 cmrsim-0.30/
--rw-rw-rw-   0 root         (0) root         (0)    35060 2024-04-15 12:17:37.000000 cmrsim-0.30/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3261 2024-04-15 12:19:29.836124 cmrsim-0.30/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2852 2024-04-15 12:17:37.000000 cmrsim-0.30/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.828124 cmrsim-0.30/cmrsim/
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-15 12:19:29.000000 cmrsim-0.30/cmrsim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.828124 cmrsim-0.30/cmrsim/analytic/
--rw-rw-rw-   0 root         (0) root         (0)      354 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5193 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/_composite_signal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.832124 cmrsim-0.30/cmrsim/analytic/contrast/
--rw-rw-rw-   0 root         (0) root         (0)      850 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/contrast/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18570 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/contrast/_spatial.py
--rw-rw-rw-   0 root         (0) root         (0)    15609 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/contrast/base.py
--rw-rw-rw-   0 root         (0) root         (0)    12862 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/contrast/coil_sensitivities.py
--rw-rw-rw-   0 root         (0) root         (0)     4116 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/contrast/diffusion_weighting.py
--rw-rw-rw-   0 root         (0) root         (0)     4871 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/contrast/offresonance.py
--rw-rw-rw-   0 root         (0) root         (0)     4644 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/contrast/phase_tracking.py
--rw-rw-rw-   0 root         (0) root         (0)    13231 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/contrast/sequences.py
--rw-rw-rw-   0 root         (0) root         (0)     4847 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/contrast/t2_star.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.832124 cmrsim-0.30/cmrsim/analytic/encoding/
--rw-rw-rw-   0 root         (0) root         (0)      707 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/encoding/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4218 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/encoding/_from_sequence.py
--rw-rw-rw-   0 root         (0) root         (0)    14772 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/encoding/base.py
--rw-rw-rw-   0 root         (0) root         (0)     9396 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/encoding/cartesian.py
--rw-rw-rw-   0 root         (0) root         (0)    13333 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/analytic/simulation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.832124 cmrsim-0.30/cmrsim/bloch/
--rw-rw-rw-   0 root         (0) root         (0)      493 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/bloch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5423 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/bloch/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    27331 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/bloch/_generic.py
--rw-rw-rw-   0 root         (0) root         (0)     3456 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/bloch/_ideal.py
--rw-rw-rw-   0 root         (0) root         (0)     6674 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/bloch/_multi_coil.py
--rw-rw-rw-   0 root         (0) root         (0)     7960 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/bloch/submodules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.832124 cmrsim-0.30/cmrsim/datasets/
--rw-rw-rw-   0 root         (0) root         (0)      702 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/datasets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3804 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/datasets/_analytic.py
--rw-rw-rw-   0 root         (0) root         (0)     2842 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/datasets/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1655 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/datasets/_bloch.py
--rw-rw-rw-   0 root         (0) root         (0)    41550 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/datasets/_cardiac_mesh.py
--rw-rw-rw-   0 root         (0) root         (0)    23193 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/datasets/_flow.py
--rw-rw-rw-   0 root         (0) root         (0)    14195 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/datasets/_regular_grid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.836124 cmrsim-0.30/cmrsim/reconstruction/
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/reconstruction/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1820 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/reconstruction/base.py
--rw-rw-rw-   0 root         (0) root         (0)     6823 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/reconstruction/cartesian.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.836124 cmrsim-0.30/cmrsim/simulation_templates/
--rw-rw-rw-   0 root         (0) root         (0)      189 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/simulation_templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9173 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/simulation_templates/experimental_optimization.py
--rw-rw-rw-   0 root         (0) root         (0)    20333 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/simulation_templates/flow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.836124 cmrsim-0.30/cmrsim/trajectory/
--rw-rw-rw-   0 root         (0) root         (0)     1437 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/trajectory/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3299 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/trajectory/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     5577 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/trajectory/_breathing.py
--rw-rw-rw-   0 root         (0) root         (0)     8492 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/trajectory/_diffusion.py
--rw-rw-rw-   0 root         (0) root         (0)    26069 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/trajectory/_flow.py
--rw-rw-rw-   0 root         (0) root         (0)    10625 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/trajectory/_proper_ortho_decomp.py
--rw-rw-rw-   0 root         (0) root         (0)     7554 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/trajectory/_taylor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.836124 cmrsim-0.30/cmrsim/utils/
--rw-rw-rw-   0 root         (0) root         (0)      376 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4170 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/utils/coordinates.py
--rw-rw-rw-   0 root         (0) root         (0)     6671 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/utils/display.py
--rw-rw-rw-   0 root         (0) root         (0)     1246 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/utils/particle_properties.py
--rw-rw-rw-   0 root         (0) root         (0)     7023 2024-04-15 12:17:37.000000 cmrsim-0.30/cmrsim/utils/snr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:19:29.828124 cmrsim-0.30/cmrsim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3261 2024-04-15 12:19:29.000000 cmrsim-0.30/cmrsim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1734 2024-04-15 12:19:29.000000 cmrsim-0.30/cmrsim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 12:19:29.000000 cmrsim-0.30/cmrsim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2024-04-15 12:19:29.000000 cmrsim-0.30/cmrsim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-15 12:19:29.000000 cmrsim-0.30/cmrsim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 12:19:29.836124 cmrsim-0.30/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1683 2024-04-15 12:17:37.000000 cmrsim-0.30/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 10:33:14.982579 cmrsim-0.31/
+-rw-rw-rw-   0 root         (0) root         (0)    35060 2024-05-18 08:23:52.000000 cmrsim-0.31/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3472 2024-05-20 10:33:14.982579 cmrsim-0.31/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-20 10:31:17.000000 cmrsim-0.31/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 10:33:14.970579 cmrsim-0.31/cmrsim/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-20 10:33:14.000000 cmrsim-0.31/cmrsim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 10:33:14.974579 cmrsim-0.31/cmrsim/analytic/
+-rw-rw-rw-   0 root         (0) root         (0)      354 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/analytic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5193 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/analytic/_composite_signal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 10:33:14.974579 cmrsim-0.31/cmrsim/analytic/contrast/
+-rw-rw-rw-   0 root         (0) root         (0)      850 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/analytic/contrast/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19179 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/analytic/contrast/_spatial.py
+-rw-rw-rw-   0 root         (0) root         (0)    15609 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/analytic/contrast/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    12860 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/analytic/contrast/coil_sensitivities.py
+-rw-rw-rw-   0 root         (0) root         (0)     4116 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/analytic/contrast/diffusion_weighting.py
+-rw-rw-rw-   0 root         (0) root         (0)     4871 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/analytic/contrast/offresonance.py
+-rw-rw-rw-   0 root         (0) root         (0)     4644 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/analytic/contrast/phase_tracking.py
+-rw-rw-rw-   0 root         (0) root         (0)    13231 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/analytic/contrast/sequences.py
+-rw-rw-rw-   0 root         (0) root         (0)     4847 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/analytic/contrast/t2_star.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 10:33:14.974579 cmrsim-0.31/cmrsim/analytic/encoding/
+-rw-rw-rw-   0 root         (0) root         (0)      707 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/analytic/encoding/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4788 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/analytic/encoding/_from_sequence.py
+-rw-rw-rw-   0 root         (0) root         (0)    15254 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/analytic/encoding/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     9504 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/analytic/encoding/cartesian.py
+-rw-rw-rw-   0 root         (0) root         (0)    13333 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/analytic/simulation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 10:33:14.978579 cmrsim-0.31/cmrsim/bloch/
+-rw-rw-rw-   0 root         (0) root         (0)      493 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/bloch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5423 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/bloch/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    31585 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/bloch/_generic.py
+-rw-rw-rw-   0 root         (0) root         (0)     3456 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/bloch/_ideal.py
+-rw-rw-rw-   0 root         (0) root         (0)     6949 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/bloch/_multi_coil.py
+-rw-rw-rw-   0 root         (0) root         (0)     7962 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/bloch/submodules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 10:33:14.978579 cmrsim-0.31/cmrsim/datasets/
+-rw-rw-rw-   0 root         (0) root         (0)      702 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/datasets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4076 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/datasets/_analytic.py
+-rw-rw-rw-   0 root         (0) root         (0)     2842 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/datasets/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/datasets/_bloch.py
+-rw-rw-rw-   0 root         (0) root         (0)    41550 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/datasets/_cardiac_mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)    23193 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/datasets/_flow.py
+-rw-rw-rw-   0 root         (0) root         (0)    14195 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/datasets/_regular_grid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 10:33:14.978579 cmrsim-0.31/cmrsim/reconstruction/
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/reconstruction/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1820 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/reconstruction/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6823 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/reconstruction/cartesian.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 10:33:14.978579 cmrsim-0.31/cmrsim/simulation_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      189 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/simulation_templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9173 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/simulation_templates/experimental_optimization.py
+-rw-rw-rw-   0 root         (0) root         (0)    20333 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/simulation_templates/flow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 10:33:14.982579 cmrsim-0.31/cmrsim/trajectory/
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/trajectory/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3299 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/trajectory/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6171 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/trajectory/_breathing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8492 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/trajectory/_diffusion.py
+-rw-rw-rw-   0 root         (0) root         (0)    26016 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/trajectory/_flow.py
+-rw-rw-rw-   0 root         (0) root         (0)    11429 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/trajectory/_proper_ortho_decomp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7554 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/trajectory/_taylor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 10:33:14.982579 cmrsim-0.31/cmrsim/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      410 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4170 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/utils/coordinates.py
+-rw-rw-rw-   0 root         (0) root         (0)     6671 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/utils/display.py
+-rw-rw-rw-   0 root         (0) root         (0)     4371 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/utils/eddy_current.py
+-rw-rw-rw-   0 root         (0) root         (0)     1246 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/utils/particle_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     7023 2024-05-18 08:23:52.000000 cmrsim-0.31/cmrsim/utils/snr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 10:33:14.974579 cmrsim-0.31/cmrsim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3472 2024-05-20 10:33:14.000000 cmrsim-0.31/cmrsim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1763 2024-05-20 10:33:14.000000 cmrsim-0.31/cmrsim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 10:33:14.000000 cmrsim-0.31/cmrsim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2024-05-20 10:33:14.000000 cmrsim-0.31/cmrsim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-20 10:33:14.000000 cmrsim-0.31/cmrsim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 10:33:14.982579 cmrsim-0.31/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1846 2024-05-20 10:07:16.000000 cmrsim-0.31/setup.py
```

### Comparing `cmrsim-0.30/LICENSE` & `cmrsim-0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/PKG-INFO` & `cmrsim-0.31/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: cmrsim
-Version: 0.30
+Version: 0.31
 Home-page: https://gitlab.ethz.ch//ibt-cmr/mri_simulation/cmrsim/
 Author: Jonathan Weine, Charles McGrath
 Project-URL: Documentation, https://people.ee.ethz.ch/~jweine/cmrsim/latest/index.html
 Project-URL: Source, https://gitlab.ethz.ch//ibt-cmr/mri_simulation/cmrsim/
 Project-URL: Institute, https://cmr.ethz.ch/
 Requires-Python: >=3.6
+Provides-Extra: cuda
 License-File: LICENSE
 
 .. image:: https://people.ee.ethz.ch/~jweine/cmrsim/latest/_images/Logo_cmrsim_moving_light.svg
    :align: right
    :scale: 150 %
 
 Welcome to CMRsim!
@@ -52,20 +53,28 @@
 
 Release versions are published on PyPI, which allows installing cmrsim with:
 
 .. code-block::
 
     pip install cmrsim
 
+
 Development versions are only available using the extra url:
 
 .. code-block::
 
     pip install cmrsim --extra-index-url https://gitlab.ethz.ch/api/v4/projects/23798/packages/pypi/simple
 
+
+To install cuda and cdnn for GPU accellaration (requires nvidia drivers to be installed on your system), from version 0.31 you can use:
+
+.. code-block::
+    
+    pip install cmrsim[cuda]
+
 Docker
 ^^^^^^^^
 For each major release a set of docker images are compiled and published in the
 `container registry`_ associated with repository. Within the docker images, all requirements
 are installed for simulation deployment.
 
 .. _container registry: https://gitlab.ethz.ch/jweine/cmrsim/container_registry
```

### Comparing `cmrsim-0.30/README.rst` & `cmrsim-0.31/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -41,20 +41,28 @@
 
 Release versions are published on PyPI, which allows installing cmrsim with:
 
 .. code-block::
 
     pip install cmrsim
 
+
 Development versions are only available using the extra url:
 
 .. code-block::
 
     pip install cmrsim --extra-index-url https://gitlab.ethz.ch/api/v4/projects/23798/packages/pypi/simple
 
+
+To install cuda and cdnn for GPU accellaration (requires nvidia drivers to be installed on your system), from version 0.31 you can use:
+
+.. code-block::
+    
+    pip install cmrsim[cuda]
+
 Docker
 ^^^^^^^^
 For each major release a set of docker images are compiled and published in the
 `container registry`_ associated with repository. Within the docker images, all requirements
 are installed for simulation deployment.
 
 .. _container registry: https://gitlab.ethz.ch/jweine/cmrsim/container_registry
```

### Comparing `cmrsim-0.30/cmrsim/analytic/_composite_signal.py` & `cmrsim-0.31/cmrsim/analytic/_composite_signal.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/analytic/contrast/__init__.py` & `cmrsim-0.31/cmrsim/analytic/contrast/__init__.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/analytic/contrast/_spatial.py` & `cmrsim-0.31/cmrsim/analytic/contrast/_spatial.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,16 +44,16 @@
                 uniform_mesh[f"signal_out{i}"] = np.abs(signal_out)[:, i, 0]
 
 
     :param expand_repetitions: if True, expands repetition axes with the factor determined by the first axes of the
                                 following input arguments
     :param slice_normal: (expansion_factor, 3) vector defining the slice normal of the excitation slice
     :param slice_position: (expansion_factor, 3) vector determining the slice-center-point
-    :param slice_thickness:(expansion_factor, )  scalar in meter, determining the slice thickness
-    :param device:
+    :param slice_thickness: (expansion_factor, ) scalar in meter, determining the slice thickness
+    :param device: name of the device to place this operation on
     """
     #: Additional mandatory keyword arguments for call
     required_quantities = ('r_vectors_excitation', )
     #: (expansion_factor, 3) vector defining the slice normal of the excitation slice
     slice_normal: tf.Variable = None
     #: (expansion_factor, 3) vector determining the slice-center-point
     slice_position: tf.Variable = None
@@ -128,17 +128,20 @@
                           ["Shape missmatch for input argument signal_tensor for case no-expand in SliceProfile! "
                            "Expected repetitions axis == self.expansion factor but got: ", input_shape, " | ",
                            self.expansion_factor])
                 result = tf.einsum('vrk, vrk -> vrk', signal_tensor, profile_factors)
             return result
 
     def slice_profile(self, s_coord: tf.Tensor) -> tf.Tensor:
-        """
-        :param s_coord: arbitrary shaped tensor containing the values for through-slice coordinate relative to slice
-            position
+        """ Computes the slice profile weighting factor for each through-slice position passed in. 
+        
+        This method can be overwritten by a subclass to implement a more sophisticated slice-profile.
+
+        :param s_coord: arbitrary shaped tensor containing the values for
+                        through-slice coordinate relative to slice position
         :return: factor between 0, 1 for each position (of stame shape as s_coord)
         """
         return tf.where(tf.abs(s_coord) < tf.reshape(self.slice_thickness, [1, -1, 1]) / 2,
                         tf.ones_like(s_coord), tf.zeros_like(s_coord))
 
 
 class LocalLookREST(BaseSignalModel):
@@ -193,14 +196,18 @@
     required_quantities = ('r_vectors_excitation', )
     #: (expansion_factor, 4, 4) orientation matrix containing the transformation matrix from r_vectors into MPS
     #: coordinates. Is composed from slice_normal, phase_encoding and readout directions. matrix per repetition
     #: is guaranteed to be orthogonal
     orientation_matrix: tf.Variable
     #: (expansion_factor, 3) spatial extend per M-P-S directions (conceptually equivalent to slice-thickness)
     spatial_extend: tf.Variable
+    #: (expansion_factor, 3) vector defining the slice normal of the excitation slice
+    slice_normal: tf.Variable = None
+    #: (expansion_factor, 3) vector determining the slice-center-point
+    slice_position: tf.Variable = None
 
     def __init__(self, expand_repetitions: bool,
                  slice_normal: Sequence[Union[float, Sequence[float]]],
                  readout_direction: Sequence[Union[float, Sequence[float]]],
                  phase_encoding_direction: Sequence[Union[float, Sequence[float]]],
                  slice_position: Sequence[Union[float, Sequence[float]]],
                  spatial_extends: Sequence[Union[float, Sequence[float]]],
@@ -284,27 +291,28 @@
             augmented_coords = tf.concat([relative_coords, tf.ones_like(relative_coords[..., :1])], axis=-1)
             mps_coords = tf.einsum("rij, vrki-> vrkj", self.orientation_matrix, augmented_coords)
             profile_factors = self.box_profile(mps_coords)
             profile_factors = tf.complex(profile_factors, tf.zeros_like(profile_factors))
 
             # Case 1: expand-dimensions
             if self.expand_repetitions or self.expansion_factor == 1:
-                tf.print(tf.shape(signal_tensor), tf.shape(profile_factors))
                 temp = tf.einsum('vrk, vek -> vrek', signal_tensor, profile_factors)
                 result = tf.reshape(temp, (input_shape[0], -1, input_shape[2]))
             else:  # Case 2: repetition-axis of signal_tensor must match self.expansion_factor
                 tf.Assert(input_shape[1] == self.expansion_factor,
                           ["Shape missmatch for input argument signal_tensor for case no-expand in SliceProfile! "
                            "Expected repetitions axis == self.expansion factor but got: ", input_shape, " | ",
                            self.expansion_factor])
                 result = tf.einsum('vrk, vrk -> vrk', signal_tensor, profile_factors)
             return result
 
     def box_profile(self, mps_coords: tf.Tensor) -> tf.Tensor:
-        """
+        """ Computes the spatial weighting factor based on the 3D coordinate passed in as argument.
+        This method can be overwritten by a subclass to implement a more sophisticated weighting.
+        
         :param mps_coords: arbitrary shaped tensor containing the values for MPS coordinate relative to slice position
         :return: factor between 0, 1 for each position (of same shape as mps_coords[..., 0])
         """
         in_x = tf.abs(mps_coords[..., 0]) < tf.reshape(self.spatial_extend[..., 0], [1, -1, 1]) / 2
         in_y = tf.abs(mps_coords[..., 1]) < tf.reshape(self.spatial_extend[..., 1], [1, -1, 1]) / 2
         in_z = tf.abs(mps_coords[..., 2]) < tf.reshape(self.spatial_extend[..., 2], [1, -1, 1]) / 2
         binary_factors = tf.where(tf.reduce_prod(tf.cast(tf.stack([in_x, in_y, in_z], axis=0), tf.float32), axis=0)> 0.,
```

### Comparing `cmrsim-0.30/cmrsim/analytic/contrast/base.py` & `cmrsim-0.31/cmrsim/analytic/contrast/base.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/analytic/contrast/coil_sensitivities.py` & `cmrsim-0.31/cmrsim/analytic/contrast/coil_sensitivities.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     Instantiates a Module that looks up coil sensitivities and multiplies the sensitivy
     value for the corresponding position to the signal vector when called.
 
     .. note::
 
         expand_repetitions is always set to True for coil-sensitivities, which means that
-        the output hast a #repetions * #coils dimension on the repetitions axis
+        the output has a #repetions * #coils dimension on the repetitions axis
 
     :param coil_sensitivities: (X, Y, Z, #channels) with dtype complex64
     :param map_dimensions: (3, 2) -> [(xlow, xhigh), (ylow, yhigh), (zlow, zhigh)]
                             Extend of the map in scanner coordinate system. Used to sort
                             iso-chromat positions into bins. This is assumed to be the *length*
                             in meter in each spatial direction
     :param device: (str) Device on which all operations except for the look-up
@@ -156,15 +156,15 @@
                          map_dimensions: np.ndarray, relative_coil_radius: float = 1.5,
                          device: str = 'CPU:0', **kwargs):
         """Lookup for ideal bird-cage coil sensitivities.
 
         .. note::
 
             expand_repetitions is always set to True for coil-sensitivities, which means that
-            the output hast a #repetions * #coils dimension on the repetitions axis
+            the output has a #repetions * #coils dimension on the repetitions axis
 
         :param map_shape: (X, Y, Z, #coils) array shape of the resulting coil-maps
         :param map_dimensions: (3, 2) -> [(xlow, xhigh), (ylow, yhigh), (zlow, zhigh)] Extend of
         :param relative_coil_radius: distance of the birdcage ring from the map center
             the map in scanner coordinate system. Used to sort iso-chromat positions into bins.
             This is assumed to be the *length* in meter in each spatial direction
         :param device: (str) Device on which all operations except for the look-up are
```

### Comparing `cmrsim-0.30/cmrsim/analytic/contrast/diffusion_weighting.py` & `cmrsim-0.31/cmrsim/analytic/contrast/diffusion_weighting.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/analytic/contrast/offresonance.py` & `cmrsim-0.31/cmrsim/analytic/contrast/offresonance.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/analytic/contrast/phase_tracking.py` & `cmrsim-0.31/cmrsim/analytic/contrast/phase_tracking.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/analytic/contrast/sequences.py` & `cmrsim-0.31/cmrsim/analytic/contrast/sequences.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/analytic/contrast/t2_star.py` & `cmrsim-0.31/cmrsim/analytic/contrast/t2_star.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/analytic/encoding/__init__.py` & `cmrsim-0.31/cmrsim/analytic/encoding/__init__.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/analytic/encoding/_from_sequence.py` & `cmrsim-0.31/cmrsim/analytic/encoding/_from_sequence.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,25 @@
 import numpy as np
 import tensorflow as tf
 
 from cmrsim.analytic.encoding.base import BaseSampling
 
 # pylint: disable=abstract-method
 class GenericEncoding(BaseSampling):
-    """"Encoding module that allowing to directly define the k-space sampling events"""
+    """"Encoding module that allowing to directly define the k-space sampling events
+
+    :param name: Name of the module
+    :param k_space_vectors: List or single instance of a numpy array containing the all sampled
+                            k-space vectors, each with shape (N_i, 3)
+    :param sampling_times: List or single instance of numpy array containing corresponding
+                            sampling times, each with shape (N_i, ).
+    :param absolute_noise_std: Noise standard deviation
+    :param k_space_segments: If not specified, the number of sequences is used.
+    :param device: Name of device that the operation is placed on
+    """
     #: (N, 3) - Tensor containing all sampled k-space vectors
     _kspace_vectors: tf.Tensor
     #: (N, ) - Tensor containing the timing, corresponding to the kspace vectors
     _sampling_times: tf.Tensor
 
     def __init__(self, name: str,
                  k_space_vectors: Iterable[np.ndarray],
```

### Comparing `cmrsim-0.30/cmrsim/analytic/encoding/base.py` & `cmrsim-0.31/cmrsim/analytic/encoding/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -260,19 +260,24 @@
         """
         if int(self.k_space_segments) > 1:  # noqa
             return self._segmented_sampling_times
 
         return self.sampling_times.read_value()
 
     def set_orientation_matrix(self, slice_position: Quantity, slice_normal: np.ndarray,
-                               readout_direction: np.ndarray):
-        """
-        :param slice_position: (3, )
-        :param slice_normal:
-        :param readout_direction:
+                               readout_direction: np.ndarray) -> None:
+        """Sets the 4x4 orientation matrix of the encoding module, by constructing the 
+        transformation I -> MPS from the slice position, normal and readout direction.
+        Phase encoding computed by cross product of slice normal and readout. 
+
+        Modifies the attribute `self.ori_matrix`.
+
+        :param slice_position: 3D coordinate of slice center in XYZ coordinates with shape (3, )
+        :param slice_normal: Normal vector of slice in XYZ coordinates with shape (3, )
+        :param readout_direction: Readout direction vector in XYZ coordinates with shape (3, )
         """
         from cmrsim.utils.coordinates import compute_orientation_matrix
         # Strip the last row to make it a (3, 4) matrix
         trafo_mat = compute_orientation_matrix(slice_normal, slice_position, readout_direction)[:3]
         
         if self.ori_matrix is None:
             self.ori_matrix = tf.Variable(trafo_mat.astype(np.float32), shape=(3, 4),
```

### Comparing `cmrsim-0.30/cmrsim/analytic/encoding/cartesian.py` & `cmrsim-0.31/cmrsim/analytic/encoding/cartesian.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 import tensorflow as tf
 
 from cmrsim.analytic.encoding.base import BaseSampling
 
 
 # pylint: disable=abstract-method
 class SingleLinePerShot(BaseSampling):
-    """ Encoding Module that assumes the handed in signal tensor in images space to be calculated
+    """ 
+    :warning: DEPRECATED planned for removal 
+
+    Encoding Module that assumes the handed in signal tensor in images space to be calculated
     according to one process per k-space line. Number of segments in this implementation
     corresponds to number of acquired k-space lines
     """
     # pylint: disable=too-many-arguments
     def __init__(self, field_of_view: Union[Tuple[float, float], List[float]],
                  sampling_matrix_size: Union[Tuple[int, int], List[int], 'numpy.ndarray'],
                  absolute_noise_std: float,
@@ -71,15 +74,18 @@
                                  [self.matrix_size[1], ]) - self.readout_duration.read_value() / 2
         k_vectors = tf.einsum('ij, nj -> ni', tf.transpose(self.orientation), k_vectors)
         return k_vectors, sampling_times
 
         
 # pylint: disable=abstract-method
 class EPI(BaseSampling):
-    """ Encoding Module implementing a single shot echo planar imaging trajectory.
+    """ 
+    :warning: DEPRECATED planned for removal 
+    
+    Encoding Module implementing a single shot echo planar imaging trajectory.
      The subdivision into segments is solely used to manage memory limitation during simulation.
     """
     # pylint: disable=too-many-arguments
     def __init__(self, field_of_view: Union[Tuple[float, float], List[float]],
                  sampling_matrix_size: Union[Tuple[int, int], List[int], 'numpy.ndarray'],
                  absolute_noise_std: float,
                  read_out_duration: float = None,
```

### Comparing `cmrsim-0.30/cmrsim/analytic/simulation.py` & `cmrsim-0.31/cmrsim/analytic/simulation.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/bloch/_base.py` & `cmrsim-0.31/cmrsim/bloch/_base.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/bloch/_generic.py` & `cmrsim-0.31/cmrsim/bloch/_generic.py`

 * *Files 18% similar despite different names*

```diff
@@ -69,15 +69,21 @@
                                   **phantom_batch)
 
     :param name: Verbose name of the module (non-functionally relevant)
     :param gamma: gyromagnetic ratio in rad/ms/m
     :param time_grid: (n_steps) - tf.float32 - time definition for numerical integration steps
     :param gradient_waveforms: (#repetitions, #steps, 3) - tf.float32 - Definition of gradients
                         in mT/m
-    :param rf_waveforms: (#repetitions, #steps) - tf.complex64 -
+    :param higher_order_gradient_waveforms: (#repetitions, #steps, N)- tf.float32 - Definition of 0th and 2nd order
+                        spherical harmonic gradient terms. First order terms are assumed to be incroporated into 
+                        the gradient\_waveforms argument.
+                        Last dimension contains N spherical harmonic terms ordered according to
+                        (0,0), (2,-2), (2,-1), (2,0), (2,1), (2,2). This corresponds to the definition 
+                        in Vannesjo et al. (2012) (https://doi.org/10.1002/mrm.24263) 
+    :param rf_waveforms: (#repetitions, #steps) - tf.complex64 - complex valued RF waveforms 
     :param adc_events: (#repetition, #steps, 2) - tf.float32 - last axis contains the adc-on
                             definitions and the adc-phase
     :param submodules: List[tf.Modules] implementing the __call__ function returning the
                             resulting phase increment contribution
     :param device: str
     """
     #: (Non-uniform) temporal raster defining the simulation steps in milliseconds - shape: (T, )
@@ -100,45 +106,56 @@
 
     #: Accumulator variables for the signal acquired at specified adc-events. This is empty if no
     #: ADC==On events where specified. The length of the List is equal to the number of repetitions
     #: and the shape of each tf.Variable is (sum(ADC[R]==1), ), which can result different length
     #: if the repetitions have different numbers of samples.
     time_signal_acc: List[tf.Variable] = None
 
+    #: Definition of higher order spherical harmonic gradient terms. Last dimension contains
+    #: N spherical harmonic terms ordered according to (0,0), (2,-2), (2,-1), (2,0), (2,1),
+    #:  (2,2), (3,-3) ..., 
+    #: 1th order terms should be incorporated into gradient_waveforms
+    higher_order_gradient_waveforms: tf.Variable = None
+
     #: Number of repetitions derived from specified waveforms
     n_repetitions: int
 
     #: Gyromagnetic ration in rad/ms/m specified on instantiation
     gamma: float
 
     def __init__(self, name: str,
                  gamma: float,
                  time_grid: tf.Tensor,
                  gradient_waveforms: tf.Tensor = None,
+                 higher_order_gradient_waveforms: tf.Tensor = None,
                  rf_waveforms: tf.Tensor = None,
                  adc_events: tf.Tensor = None,
                  submodules: Tuple[BaseSubmodule, ...] = (),
                  device: str = None):
         """
         :param name: Verbose name of the module (non-functionaly relevant)
         :param gamma: gyromagnetic ratio in rad/ms/m
         :param time_grid: (n_steps) - tf.float32 -
         :param gradient_waveforms: (#repetitions, #steps, 3) - tf.float32 - Definition of gradients
                             in mT/m
+        :param higher_order_gradient_waveforms: (#repetitions, #steps, N)- tf.float32 - Definition of higher order
+                                spherical harmonic gradient terms. Last dimension contains N spherical harmonic terms
+                                ordered according to (0,0), (2,-2), (2,-1), (2,0), (2,1), (2,2), (3,-3) ...
+                                1st order terms should be incorporated into gradient_waveforms
         :param rf_waveforms: (#repetitions, #steps) - tf.complex64 -
         :param adc_events: (#repetition, #steps, 2) - tf.float32 - last axis contains the adc-on
                                 definitions and the adc-phase
         :param submodules: List[tf.Modules] implementing the __call__ function returning the
                                 resulting phase increment contribution
         :param device: str
         """
         super().__init__(name, device=device)
 
         # Validate input waveforms such that they match in shape
-        waveforms = [gradient_waveforms, rf_waveforms, adc_events]
+        waveforms = [gradient_waveforms, higher_order_gradient_waveforms, rf_waveforms, adc_events]
         shape_matching_time = [g.shape[1] == time_grid.shape[0] for g in waveforms if g is not None]
         shape_matching_reps = set([g.shape[0] for g in waveforms if g is not None])
         if len(shape_matching_time) == 0:
             raise ValueError("No wave-forms (rf/grads) specified")
         if not all(shape_matching_time):
             raise ValueError("Number of time-steps in specified wave-forms do not "
                              f"match {shape_matching_time}")
@@ -155,14 +172,20 @@
             self.dt_grid = tf.Variable(np.diff(time_grid), dtype=tf.float32, shape=(None,),
                                        trainable=False)
 
         if gradient_waveforms is not None:
             with tf.device(self.device):
                 self.gradient_waveforms = tf.Variable(gradient_waveforms, dtype=tf.float32,
                                                       shape=(None, None, 3), trainable=False)
+
+        if higher_order_gradient_waveforms is not None:
+            with tf.device(self.device):
+                self.higher_order_gradient_waveforms = tf.Variable(higher_order_gradient_waveforms, dtype=tf.float32,
+                                                                   shape=(None, None, None), trainable=False)
+
         if rf_waveforms is not None:
             with tf.device(self.device):
                 self.rf_waveforms = tf.Variable(rf_waveforms, dtype=tf.complex64,
                                                 shape=(None, None), trainable=False)
         if adc_events is not None:
             with tf.device(self.device):
                 self.adc_events = tf.Variable(adc_events[:, :, 0], dtype=tf.float32,
@@ -332,15 +355,15 @@
         :param M0: (n_repetitions/1, #batch)
         :param kwargs:
         :return:  - magnetization
                   - r_next
                   - signal at adc_on==True with shape (n_repetitions, n_samples)
         """
         with tf.device(self.device):
-            rf_waveforms, grad_waveforms, adc_on, adc_phase, adc_widx, batch_signal = \
+            rf_waveforms, grad_waveforms, higher_order_grad, adc_on, adc_phase, adc_widx, batch_signal = \
                 self._init_tensors(n_samples, n_repetitions, repetition_index)
 
             r_prev = tf.reshape(initial_position, [1, -1, 3])
             r_next = r_prev
 
             # Iterate over all time intervals to obtain the magnetization evolution
             for t_idx in tf.range(1, tf.shape(self.dt_grid)[0]+1):
@@ -368,14 +391,17 @@
                 delta_phi = tf.zeros_like(M0, dtype=tf.float32)
                 if self.gradient_waveforms is not None:
                     grad = grad_waveforms[..., t_idx-1:t_idx+1, :]
                     gdotr_l = tf.reduce_sum(grad[..., 0, :] * r_prev, axis=-1)
                     gdotr_r = tf.reduce_sum(grad[..., 1, :] * r_next, axis=-1)
                     delta_phi += (gdotr_l + gdotr_r) / 2. * self.gamma * self.dt_grid[t_idx-1]
 
+                if self.higher_order_gradient_waveforms is not None:
+                    delta_phi += self._apply_ecc(t_idx, higher_order_grad, r_prev, r_next)
+   
                 for submod in self._submodules:
                     phi_s = submod(
                         gradient_wave_form=grad_waveforms[:, 0, t_idx:t_idx+1, :],
                         trajectories=r_next[:, :, tf.newaxis], dt=self.dt_grid[t_idx-1],
                         **additional_fields, **kwargs)
                     if tf.shape(phi_s)[0] < tf.shape(delta_phi)[0]:
                         phi_s = tf.tile(phi_s, [tf.shape(delta_phi)[0], 1, 1])
@@ -415,14 +441,15 @@
         number of samples.
 
         :param n_samples:
         :param n_repetitions:
         :param repetition_index:
         :return: - rf_waveform (#reps, #steps) or None
                  - grad_waveform (#reps, #steps, 3) or None
+                 - higher_order (#reps, #steps, N) or None
                  - adc_events (#reps, #steps) or None
                  - adc_phase (#reps, #steps) or None
                  - adc_writing_idx (#reps, #steps) or None
                  - batch_signal (#reps, #samples) -> used for signal accumulation
         """
         batch_signal = tf.zeros(shape=(n_samples, n_repetitions), dtype=tf.complex64)
         repetitions = tf.range(repetition_index, repetition_index + n_repetitions, 1)
@@ -437,26 +464,68 @@
         # and calculate the left value of for trapezoidal phase integration
         if self.gradient_waveforms is not None:
             current_gradient_waveforms = tf.gather(self.gradient_waveforms, repetitions,
                                                    axis=0)[:, tf.newaxis]
         else:
             current_gradient_waveforms = None
 
+        if self.higher_order_gradient_waveforms is not None:
+            current_higher_order_grad = tf.gather(self.higher_order_gradient_waveforms, repetitions,
+                                                  axis=0)[:, tf.newaxis]
+        else:
+            current_higher_order_grad = None
+
         # If adc events are specified, gather all required repetitions (either all or 1)
         # or otherwise create a default zero return value for the batch signal as this it is
         # required autographing this function by tensorflow
         if self.adc_events is not None:
             current_adc_events = tf.gather(self.adc_events, repetitions, axis=0)
             current_adc_phase = tf.gather(self.adc_phase, repetitions, axis=0)
             adc_writing_indices = tf.cast(tf.math.cumsum(current_adc_events, axis=1) * current_adc_events - 1, tf.int32)
         else:
             current_adc_events, current_adc_phase, adc_writing_indices = None, None, None
 
-        return (current_rf_waveforms, current_gradient_waveforms, current_adc_events,
-                current_adc_phase, adc_writing_indices, batch_signal)
+        return (current_rf_waveforms, current_gradient_waveforms, current_higher_order_grad, current_adc_events,
+                current_adc_phase, adc_writing_indices, batch_signal)        
+
+    def _apply_ecc(self, t_idx: tf.Tensor, higher_order_grad: tf.Tensor, r_prev: tf.Tensor, 
+                   r_next: tf.Tensor) -> tf.Tensor:
+        """Computes the phase delta caused by eddy currents from 0th and 2nd order, assuming 
+        the first order terms are already included in the gradient waveform definition
+        """
+        # Oth order, (0,0)=1
+        order00 = (higher_order_grad[..., t_idx - 1, 0] + higher_order_grad[..., t_idx, 0]) / 2
+
+        # 2nd order = xy
+        order20 = (higher_order_grad[..., t_idx - 1, 1] * r_prev[..., 0] * r_prev[..., 1] +
+                    higher_order_grad[..., t_idx, 1] * r_next[..., 0] * r_next[..., 1]) / 2
+
+        # 2nd order yz
+        order21 = (higher_order_grad[..., t_idx - 1, 2] * r_prev[..., 1] * r_prev[..., 2] +
+                    higher_order_grad[..., t_idx, 2] * r_next[..., 1] * r_next[..., 2]) / 2
+
+        # 2nd order 2z^2 - (x^2 + y^2)
+        order22 = (higher_order_grad[..., t_idx-1, 3] * 
+                        (2 * r_prev[..., 2]**2 - (r_prev[..., 0]**2 + r_prev[..., 1]**2)) 
+                   +  higher_order_grad[..., t_idx, 3] * 
+                        (2 * r_next[..., 2]**2 - (r_next[..., 0]**2 + r_next[..., 1]**2)) 
+                   ) / 2
+
+        # 2nd order xz
+        order23 = (higher_order_grad[..., t_idx - 1, 4] * r_prev[..., 0] * r_prev[..., 2] +
+                    higher_order_grad[..., t_idx, 4] * r_next[..., 0] * r_next[..., 2]) / 2
+
+
+        # 2nd order x^2-y^2
+        order24 = (higher_order_grad[..., t_idx - 1, 5] * (r_prev[..., 0] ** 2 - r_prev[..., 1] ** 2) 
+                   + higher_order_grad[..., t_idx, 5] * (r_next[..., 0] ** 2 - r_next[..., 1] ** 2)
+                   ) / 2
+
+        total_contribution = (order00 + order20 + order21 + order22 + order23 + order24)
+        return  total_contribution * self.gamma * self.dt_grid[t_idx - 1]
 
     @staticmethod
     def _sample(adc_events: tf.Tensor, adc_phase: tf.Tensor, adc_writing_idx: tf.Tensor,
                 magnetization: tf.Tensor, M0: tf.Tensor, r: tf.Tensor, batch_signal: tf.Tensor):
         """Sums up the :math:`m_{xy}^{+}` magnetization weighted with the associated proton-density
         of the particles and adds the signal to the batch-signal accumulator ad index specified
         in adc_writing_index.
```

### Comparing `cmrsim-0.30/cmrsim/bloch/_ideal.py` & `cmrsim-0.31/cmrsim/bloch/_ideal.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/bloch/_multi_coil.py` & `cmrsim-0.31/cmrsim/bloch/_multi_coil.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,24 +46,24 @@
 
     def __init__(self, name: str,
                  gamma: float,
                  coil_module: Union['cmrsim.analytic.contrast.coil_sensitivities.CoilSensitivity'],
                  time_grid: tf.Tensor,
                  adc_events: tf.Tensor,
                  gradient_waveforms: tf.Tensor = None,
+                 higher_order_gradient_waveforms: tf.Tensor = None,
                  rf_waveforms: tf.Tensor = None,
                  submodules: Tuple[BaseSubmodule, ...] = (),
                  device: str = None):
-        """
-
 
-        """
         super().__init__(name=name, gamma=gamma, time_grid=time_grid,
-                         gradient_waveforms=gradient_waveforms, rf_waveforms=rf_waveforms,
-                         adc_events=adc_events, submodules=submodules, device=device)
+                         gradient_waveforms=gradient_waveforms, 
+                         higher_order_gradient_waveforms=higher_order_gradient_waveforms,
+                         rf_waveforms=rf_waveforms, adc_events=adc_events,
+                         submodules=submodules, device=device)
         self.coil_lookup_module = coil_module
         self.n_coils = self.coil_lookup_module.expansion_factor
 
         # Expand the dimension of the signal accumulator to incorporate coil-maps
         with tf.device("CPU"):
             self.time_signal_acc = [
                 tf.Variable(initial_value=tf.zeros([v.read_value().shape[0], self.n_coils], dtype=tf.complex64),
@@ -80,19 +80,20 @@
         :return: - rf_waveform (#reps, #steps) or None
                  - grad_waveform (#reps, #steps, 3) or None
                  - adc_events (#reps, #steps) or None
                  - adc_phase (#reps, #steps) or None
                  - adc_writing_idx (#reps, #steps) or None
                  - batch_signal (#reps, #samples, #coils) -> used for signal accumulation
         """
-        (rf_waveforms, gradient_waveforms, adc_events, adc_phase, adc_writing_indices,
-         batch_signal) = super()._init_tensors(n_samples, n_repetitions, repetition_index)
+        # (rf_waveforms, gradient_waveforms, adc_events, adc_phase, adc_writing_indices,
+        #     batch_signal) = super()._init_tensors(n_samples, n_repetitions, repetition_index)
         batch_signal = tf.zeros(shape=(n_samples, n_repetitions, self.n_coils), dtype=tf.complex64)
-        return (rf_waveforms, gradient_waveforms, adc_events, adc_phase,
-                adc_writing_indices, batch_signal)
+        # return (rf_waveforms, gradient_waveforms, adc_events, adc_phase,
+        #         adc_writing_indices, batch_signal)
+        return super()._init_tensors(n_samples, n_repetitions, repetition_index)[:-1] + (batch_signal, )
 
     def _sample(self, adc_events: tf.Tensor, adc_phase: tf.Tensor, adc_writing_idx: tf.Tensor,
                 magnetization: tf.Tensor, M0: tf.Tensor, r: tf.Tensor, batch_signal: tf.Tensor):
         """Sums up the :math:`m_{xy}^{+}` magnetization weighted with the associated proton-density
         of the particles and adds the signal to the batch-signal accumulator ad index specified
         in adc_writing_index. Before summation, a coil-sensitivity weighting is applied
```

### Comparing `cmrsim-0.30/cmrsim/bloch/submodules.py` & `cmrsim-0.31/cmrsim/bloch/submodules.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     # pylint: disable=anomalous-backslash-in-string
     """Submodule for Bloch simulations that implements T2 start weighting by accumulating a phase
     per particle. The particle properties should be assigned randomly according to a Lorentzian
     distribution. The phase difference is evaluated according to:
 
     .. math::
 
-        \delta \phi = \omega_{T_2^\*} \delta t
+        \delta \phi = \omega_{T_2^*} \delta t
 
     :param device: name for device placing
     """
     #: Tuple of names specifying the input quantities (datasets) to run this submodule
     required_quantities: Tuple[str, ...] = ("trajectories", "omega_t2s")
 
     def __init__(self, device: str = 'GPU'):
@@ -83,17 +83,17 @@
     # pylint: disable=anomalous-backslash-in-string
     """Submodule for Bloch simulations that evaluates the concomitant field variation in
     z-direction (field variation in direction of the main magnetic field) at all particle positions
     contained in the trajectories according to:
 
     .. math::
 
-        r = (x, y, z)^T \\
-        G = (G_x, G_y, G_z)^T \\
-        \Delta \phi = (\gamma \Delta t / 2B_0) \cdot
+        r &= (x, y, z)^T \\
+        G &= (G_x, G_y, G_z)^T \\
+        \Delta \phi &= (\gamma \Delta t / 2B_0) \cdot
                     \left[ (G_x z + G_z x/2)^2 + (G_y z - G_z y/2)^2 \\right]
 
     :param gamma: gyromagnetic ratio in MHz/T (=1/ms/mT)
     :param b0: in T
     """
     required_quantities: Tuple[str] = ("gradient_wave_form", "trajectory", "dt")
```

### Comparing `cmrsim-0.30/cmrsim/datasets/__init__.py` & `cmrsim-0.31/cmrsim/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/datasets/_analytic.py` & `cmrsim-0.31/cmrsim/datasets/_analytic.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,33 +8,35 @@
 from cmrsim.datasets._base import BaseDataset
 
 if TYPE_CHECKING:
     from cmrsim.trajectory._base import BaseTrajectoryModule
 
 
 class AnalyticDataset(BaseDataset):
-    
+    """ Convenient class to create a stream buffer from numpy arrays for
+    analytic simulations, adhering to the shape and data-type definitions.
+
+    Initializes a callable module, that yields an iterable tf.Dataset on call . The target
+    shape of the yielded batches is (#batch, #repetitions, #kspace-samples, ...)
+
+    :raises: InvalidArgument - if shape of M0 and r_vector entry of the dictionary do not match
+                                (#MaterialPoints, #Repetitions, #k-space-samples)
+                                (#MaterialPoints, #Repetitions, 3, #k-space-samples)
+                                InvalidArgumentError is raised
+
+    :param array_dictionary: (OrderedDict) containing the required quantities as numpy arrays
+    :param filter_inputs: If set to true, trivial material points are filtered (M0=0),
+                            on instantiation
+    :param expand_dimension: If set to true, the numpy arrays passed in the `array_dictionary`
+                             argument are expected to not have the repetition and kspace 
+                             axis yet. In this case the axes are added respectively.
+    """
     def __init__(self, array_dictionary: OrderedDict, filter_inputs: bool = True,
                  expand_dimension: bool = False):
-        """ Initializes a callable module, that yields an iterable tf.Dataset on call. The target
-        shape of the yielded batches is (#batch, #repetitions, #kspace-samples, ...)
-
 
-        :raises: InvalidArgument - if shape of M0 and r_vector entry of the dictionary do not match
-                                  (#MaterialPoints, #Repetitions, #k-space-samples)
-                                  (#MaterialPoints, #Repetitions, 3, #k-space-samples)
-                                  InvalidArgumentError is raised
-
-        :param array_dictionary: (OrderedDict) containing the required quantities as numpy arrays
-        :param filter_inputs: If set to true, trivial material points are filtered (M0=0),
-                                on instantiation
-        :param expand_dimension:
-        :param trajectory_module:
-        :param trajectory_signatures:
-        """
         if expand_dimension:
             if len(array_dictionary["M0"].shape) > 1:
                 dtype_list = [f"{k}: {v.shape}" for k, v in array_dictionary.items()]
                 raise ValueError("Arrays appear to have repetition/sample axis already. Please"
                                  "disable the expand-dims argument. Shapes \n\t".join(dtype_list))
             array_dictionary = {k: v[:, np.newaxis, np.newaxis]
                                 for k, v in array_dictionary.items()}
```

### Comparing `cmrsim-0.30/cmrsim/datasets/_base.py` & `cmrsim-0.31/cmrsim/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/datasets/_bloch.py` & `cmrsim-0.31/cmrsim/datasets/_bloch.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,29 @@
 __all__ = ["BlochDataset"]
 
 from collections import OrderedDict
 from cmrsim.datasets._base import BaseDataset
 
 
 class BlochDataset(BaseDataset):
-    def __init__(self, array_dictionary: OrderedDict, filter_inputs: bool = True):
-        """ Initializes a callable module, that yields an iterable tf.Dataset on call. The target
-        shape of the yielded batches is (#batch, ...)
+    """Convenient class to create a stream buffer from numpy arrays for
+    Bloch simulations, adhering to the shape and data-type definitions.
+
+    Initializes a callable module, that yields an iterable tf.Dataset on call. The target
+    shape of the yielded batches is (#batch, ...)
 
-        :raises: InvalidArgument - if shape of M0, magnetization entries of the dictionary do
-                    not match (#MaterialPoints, ), (#MaterialPoints, 3)
+    :raises: InvalidArgument - if shape of M0, magnetization entries of the dictionary do
+            not match (#MaterialPoints, ), (#MaterialPoints, 3)
+
+    :param array_dictionary: (OrderedDict) containing the required quantities as numpy arrays
+    :param filter_inputs: If set to true, trivial material points are filtered (M0=0),
+                        on instantiation
+    """
+    def __init__(self, array_dictionary: OrderedDict, filter_inputs: bool = True):
 
-        :param array_dictionary: (OrderedDict) containing the required quantities as numpy arrays
-        :param filter_inputs: If set to true, trivial material points are filtered (M0=0),
-                                on instantiation
-        """
         if len(array_dictionary["M0"].shape) != 1:
             raise ValueError("Shape of input array M0 invalid")
         if len(array_dictionary["magnetization"].shape) != 2:
             raise ValueError("Shape of input array magnetization invalid")
         if len(array_dictionary["T1"].shape) != 1:
             raise ValueError("Shape of input array T1 invalid")
         if len(array_dictionary["T2"].shape) != 1:
```

### Comparing `cmrsim-0.30/cmrsim/datasets/_cardiac_mesh.py` & `cmrsim-0.31/cmrsim/datasets/_cardiac_mesh.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/datasets/_flow.py` & `cmrsim-0.31/cmrsim/datasets/_flow.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/datasets/_regular_grid.py` & `cmrsim-0.31/cmrsim/datasets/_regular_grid.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/reconstruction/base.py` & `cmrsim-0.31/cmrsim/reconstruction/base.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/reconstruction/cartesian.py` & `cmrsim-0.31/cmrsim/reconstruction/cartesian.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/simulation_templates/experimental_optimization.py` & `cmrsim-0.31/cmrsim/simulation_templates/experimental_optimization.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/simulation_templates/flow.py` & `cmrsim-0.31/cmrsim/simulation_templates/flow.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/trajectory/__init__.py` & `cmrsim-0.31/cmrsim/trajectory/__init__.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/trajectory/_base.py` & `cmrsim-0.31/cmrsim/trajectory/_base.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/trajectory/_breathing.py` & `cmrsim-0.31/cmrsim/trajectory/_breathing.py`

 * *Files 18% similar despite different names*

```diff
@@ -45,20 +45,30 @@
         self.sub_trajectory = sub_trajectory
         self.breathing_cycle_duration = tf.constant(breathing_cycle_duration, dtype=tf.float32)
         self.breathing_curve = tf.constant(breathing_curve, dtype=tf.float32)
         self.current_time_ms = tf.Variable(0., dtype=tf.float32, shape=(), trainable=False)
 
     def __call__(self, initial_positions: tf.Tensor, timing: tf.Tensor,
                  **kwargs) -> (tf.Tensor, Dict):
+        """Evaluates the contained trajectory module and adds the breathing displacement
+        :param initial_positions: passed into the submodule
+        :param timing: passed into submodule and is used to calculate breathing displacement
+        :param kwargs: passed to submodule
+        """
         positional_offset = self._interpolate_breathing_curve(timing)
         sub_trajectory_r, additional_fields = self.sub_trajectory(initial_positions=initial_positions,
                                                                   timing=timing, **kwargs)
         return positional_offset[tf.newaxis] + sub_trajectory_r, additional_fields
 
     def increment_particles(self, particle_positions: tf.Tensor, dt: tf.Tensor, **kwargs) -> (tf.Tensor, Dict):
+        """Evaluates the contained trajectory module and adds the breathing displacement
+        :param initial_positions: passed into the submodule
+        :param timing: passed into submodule and is used to calculate breathing displacement
+        :param kwargs: passed to submodule
+        """
         prev_positional_offset = self._interpolate_breathing_curve(self.current_time_ms)
         particle_positions = particle_positions - prev_positional_offset
         _t = tf.reshape(self.current_time_ms.assign_add(dt), [1, ])
         positional_offset = self._interpolate_breathing_curve(_t)
         sub_trajectory_r, additional_fields = self.sub_trajectory.increment_particles(particle_positions, dt, **kwargs)
         return positional_offset + sub_trajectory_r, additional_fields
```

### Comparing `cmrsim-0.30/cmrsim/trajectory/_diffusion.py` & `cmrsim-0.31/cmrsim/trajectory/_diffusion.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/trajectory/_flow.py` & `cmrsim-0.31/cmrsim/trajectory/_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,32 +204,32 @@
                 :caption: increment particle positions
 
                 r_init = ...  # initial_positions of shape (N, 3)
                 delta_t = tf.constant(0.01, tf.float32)
                 r_new, fields = self.trajectory_module.increment_particles(r_init, dt=delta_t)
 
 
-        :param velocity_field: (X, Y, Z, 10+n) 3D map storing gridded fields at positions X, Y, Z.
-                                            Fields 0-2 : Mean velocities (X, Y, Z).  Unit should be m/ms
-                                            Fields 3-8 : Lower triangular Cholesky decomposition of the turbulent
-                                                         Reynolds stress tensor, L. Ordering is
-                                                         (L11, L21, L22, L31, L32, L33)
-                                            Field 9 : Langevin timescale tau, in Hz.
-                                            Additional dimensions past 9 are treated as additional
-                                            data fields and returned
-        :param map_dimensions: (3, 2) -> [(xlow, xhigh), (ylow, yhigh), (zlow, zhigh)]
-                                         Physical extend of the gridded velocity fields.
-        :param additional_dimension_mapping: List of name/len pairs to unstack the looked up
-                                              values. If not None this mapping must explain all
-                                              'n' additional dimension in the parameter
-                                              velocity-field e.g. [('off_res', 1)] meaning that
-                                              off-resonance for all time points has a size of 1,
-                                              starting from index 10 in velocity field.
-        :param kwargs: - device: str defaults to CPU:0
-        """
+    :param velocity_field: (X, Y, Z, 10+n) 3D map storing gridded fields at positions X, Y, Z.
+                                        Fields 0-2 : Mean velocities (X, Y, Z).  Unit should be m/ms
+                                        Fields 3-8 : Lower triangular Cholesky decomposition of the turbulent
+                                                        Reynolds stress tensor, L. Ordering is
+                                                        (L11, L21, L22, L31, L32, L33)
+                                        Field 9 : Langevin timescale tau, in Hz.
+                                        Additional dimensions past 9 are treated as additional
+                                        data fields and returned
+    :param map_dimensions: (3, 2) -> [(xlow, xhigh), (ylow, yhigh), (zlow, zhigh)]
+                                        Physical extend of the gridded velocity fields.
+    :param additional_dimension_mapping: List of name/len pairs to unstack the looked up
+                                            values. If not None this mapping must explain all
+                                            'n' additional dimension in the parameter
+                                            velocity-field e.g. [('off_res', 1)] meaning that
+                                            off-resonance for all time points has a size of 1,
+                                            starting from index 10 in velocity field.
+    :param kwargs: - device: str defaults to CPU:0
+    """
 
     def __init__(self, velocity_field: np.ndarray, map_dimensions: np.ndarray,
                  additional_dimension_mapping: List[Tuple[str, int]] = None, **kwargs):
         """
         :param velocity_field: (X, Y, Z, 10+n) 3D map storing gridded fields at positions X, Y, Z.
                                             Fields 0-2 : Mean velocities (X, Y, Z).  Unit should be m/ms
                                             Fields 3-8 : Lower triangular Cholesky decomposition of the turbulent
```

### Comparing `cmrsim-0.30/cmrsim/trajectory/_proper_ortho_decomp.py` & `cmrsim-0.31/cmrsim/trajectory/_proper_ortho_decomp.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,17 +42,19 @@
             ## reconstructed_states.shape == (#particles, 100, #channels)
 
 
     :param time_grid: (#time_steps)
     :param trajectories: (#particles, #time_steps, 3)
     :param n_modes: Number of modes used for reduce-order representation
     :param poly_order: Order of the Taylor-series used to fit the mode-weights
-    :param additional_data: Dict[str, np.ndarray] of shape (#particles, #time_steps, #channels)
-    :param batch_size: int
-    :param is_periodic:
+    :param additional_data: Dictionary containing additional field data of shape (#particles, #time_steps, #channels)
+    :param batch_size: If not None, the output of call and increment positions will be batched in given size. 
+                        Which batch is returned depends on the argument `batch_index` as decribed below
+    :param is_periodic: If true, the mode-weights are periodically interpolated for times exceeding the 
+                        specified time-grid.
     """
     #: Number of modes used for reduce-order representation
     n_modes: tf.Variable
     #: Computed basis-functions (modes) :math:`\phi_j` used to represent the input data in
     #: a reduced order. Shape (#particles * #channels, #modes)
     basis_function: tf.Variable
     #: Keeps track of the current timing when increment_particles is called.
@@ -60,17 +62,17 @@
     #: Allows to only evaluate the position for a batch of stored particle trajectories
     current_batch_idx: tf.Variable
     #: Together with self.current_batch_size determines the subset of particle trajectories that
     #: is evaluated on call and increment_particles
     batch_size: tf.Variable
     #: Keeps track of the current timing when increment_particles is called.
     current_time_ms: tf.Variable
-    #:
+    #: Start time of the specified time grid, used for internal calculations
     ref_time: tf.Variable
-    #:
+    #: End time of the specified time grid, used for internal calculations
     end_time: tf.Variable
     #:
     _nchannels: tf.Variable
     #:
     _additional_keys: Tuple[str]
     #:
     _additional_channels: Tuple[int]
@@ -153,15 +155,19 @@
         return phi, weights
 
     def __call__(self, initial_positions: tf.Tensor, timing: tf.Tensor,
                  batch_index: int = 0, **kwargs) -> (tf.Tensor, dict):
         """Reconstructs the data state at given times t, by evaluating the taylor series
         of mode-weights and computing the weighted sum.
 
+        :param initial_positions: Unused argument which can be set to None, 
+                                    specified only to adhere to base implementaton
         :param timing: (#timesteps) in milliseconds
+        :param batch_index: determines which batch to return if `batch_size` was 
+                            specified on instantiation (sets `self.current_batch_idx`) 
         :return: (#particles, #timesteps, self._channels), {k: v} - additional data
         """
         idx_before = self.current_batch_idx.read_value()
         self.current_batch_idx.assign(batch_index)
         data = self._evaluate_trajectory(timing)
         if len(self._additional_keys) > 0:
             additional_data = {k: data[..., self._additional_channel_idx[i]:self._additional_channel_idx[i+1]]
```

### Comparing `cmrsim-0.30/cmrsim/trajectory/_taylor.py` & `cmrsim-0.31/cmrsim/trajectory/_taylor.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/utils/coordinates.py` & `cmrsim-0.31/cmrsim/utils/coordinates.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/utils/display.py` & `cmrsim-0.31/cmrsim/utils/display.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/utils/particle_properties.py` & `cmrsim-0.31/cmrsim/utils/particle_properties.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim/utils/snr.py` & `cmrsim-0.31/cmrsim/utils/snr.py`

 * *Files identical despite different names*

### Comparing `cmrsim-0.30/cmrsim.egg-info/PKG-INFO` & `cmrsim-0.31/cmrsim.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: cmrsim
-Version: 0.30
+Version: 0.31
 Home-page: https://gitlab.ethz.ch//ibt-cmr/mri_simulation/cmrsim/
 Author: Jonathan Weine, Charles McGrath
 Project-URL: Documentation, https://people.ee.ethz.ch/~jweine/cmrsim/latest/index.html
 Project-URL: Source, https://gitlab.ethz.ch//ibt-cmr/mri_simulation/cmrsim/
 Project-URL: Institute, https://cmr.ethz.ch/
 Requires-Python: >=3.6
+Provides-Extra: cuda
 License-File: LICENSE
 
 .. image:: https://people.ee.ethz.ch/~jweine/cmrsim/latest/_images/Logo_cmrsim_moving_light.svg
    :align: right
    :scale: 150 %
 
 Welcome to CMRsim!
@@ -52,20 +53,28 @@
 
 Release versions are published on PyPI, which allows installing cmrsim with:
 
 .. code-block::
 
     pip install cmrsim
 
+
 Development versions are only available using the extra url:
 
 .. code-block::
 
     pip install cmrsim --extra-index-url https://gitlab.ethz.ch/api/v4/projects/23798/packages/pypi/simple
 
+
+To install cuda and cdnn for GPU accellaration (requires nvidia drivers to be installed on your system), from version 0.31 you can use:
+
+.. code-block::
+    
+    pip install cmrsim[cuda]
+
 Docker
 ^^^^^^^^
 For each major release a set of docker images are compiled and published in the
 `container registry`_ associated with repository. Within the docker images, all requirements
 are installed for simulation deployment.
 
 .. _container registry: https://gitlab.ethz.ch/jweine/cmrsim/container_registry
```

### Comparing `cmrsim-0.30/cmrsim.egg-info/SOURCES.txt` & `cmrsim-0.31/cmrsim.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -48,9 +48,10 @@
 cmrsim/trajectory/_diffusion.py
 cmrsim/trajectory/_flow.py
 cmrsim/trajectory/_proper_ortho_decomp.py
 cmrsim/trajectory/_taylor.py
 cmrsim/utils/__init__.py
 cmrsim/utils/coordinates.py
 cmrsim/utils/display.py
+cmrsim/utils/eddy_current.py
 cmrsim/utils/particle_properties.py
 cmrsim/utils/snr.py
```

### Comparing `cmrsim-0.30/setup.py` & `cmrsim-0.31/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,20 +32,26 @@
     raise ValueError('No version as keyword "--version" was specified')
 
 with open(f'{project_name}/__init__.py', 'r+') as module_header_file:
     content = module_header_file.read()
     module_header_file.seek(0)
     module_header_file.write(f"__version__ = '{current_version}'\n" + content)
 
+extras = {
+    "cuda": ["tensorflow[and-cuda]==2.15.1", ],
+    # "phantoms": [] Planned for future installation of resources
+}
+
 setuptools.setup(
     name=project_name,
     url=url,
     project_urls=project_urls,
     version=current_version,
     author=author_list,
     author_email_=author_email_list,
     long_description=long_description,
     packages=setuptools.find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     include_package_data=True,
-    install_requires=["tensorflow", "pyvista>=0.37", "numpy>=1.19", "pint>=0.18", "cmrseq>=0.17"],
+    install_requires=["tensorflow==2.15.1", "pyvista>=0.42", "numpy>=1.22", "pint>=0.18", "cmrseq>=0.23"],
+    extras_require=extras,
     python_requires=">=3.6"
 )
```


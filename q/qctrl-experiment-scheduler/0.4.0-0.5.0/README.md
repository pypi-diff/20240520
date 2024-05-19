# Comparing `tmp/qctrl_experiment_scheduler-0.4.0.tar.gz` & `tmp/qctrl_experiment_scheduler-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_experiment_scheduler-0.4.0.tar", max compression
+gzip compressed data, was "qctrl_experiment_scheduler-0.5.0.tar", max compression
```

## Comparing `qctrl_experiment_scheduler-0.4.0.tar` & `qctrl_experiment_scheduler-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    36653 2023-10-17 00:41:48.001002 qctrl_experiment_scheduler-0.4.0/LICENSE
--rw-r--r--   0        0        0      695 2023-10-17 00:41:48.001002 qctrl_experiment_scheduler-0.4.0/README.md
--rw-r--r--   0        0        0     2918 2023-10-17 00:42:11.657134 qctrl_experiment_scheduler-0.4.0/pyproject.toml
--rwxr-xr-x   0        0        0     1181 2023-10-17 00:42:11.673134 qctrl_experiment_scheduler-0.4.0/qctrlexperimentscheduler/__init__.py
--rwxr-xr-x   0        0        0    18603 2023-10-17 00:41:48.001002 qctrl_experiment_scheduler-0.4.0/qctrlexperimentscheduler/graph.py
--rw-r--r--   0        0        0     8557 2023-10-17 00:41:48.001002 qctrl_experiment_scheduler-0.4.0/qctrlexperimentscheduler/graph_traversal.py
--rw-r--r--   0        0        0    11020 2023-10-17 00:41:48.001002 qctrl_experiment_scheduler-0.4.0/qctrlexperimentscheduler/node.py
--rwxr-xr-x   0        0        0      990 2023-10-17 00:42:11.669134 qctrl_experiment_scheduler-0.4.0/qctrlexperimentscheduler/predefined/__init__.py
--rw-r--r--   0        0        0    19928 2023-10-17 00:41:48.005002 qctrl_experiment_scheduler-0.4.0/qctrlexperimentscheduler/predefined/amplitude_calibration.py
--rw-r--r--   0        0        0    16220 2023-10-17 00:41:48.005002 qctrl_experiment_scheduler-0.4.0/qctrlexperimentscheduler/predefined/simulation_backend.py
--rw-r--r--   0        0        0     7252 2023-10-17 00:41:48.005002 qctrl_experiment_scheduler-0.4.0/qctrlexperimentscheduler/variable.py
--rw-r--r--   0        0        0     2851 1970-01-01 00:00:00.000000 qctrl_experiment_scheduler-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    36587 2024-05-19 22:55:35.205302 qctrl_experiment_scheduler-0.5.0/LICENSE
+-rw-r--r--   0        0        0      177 2024-05-19 22:55:35.205302 qctrl_experiment_scheduler-0.5.0/README.md
+-rw-r--r--   0        0        0     2861 2024-05-19 22:55:58.429101 qctrl_experiment_scheduler-0.5.0/pyproject.toml
+-rwxr-xr-x   0        0        0     1181 2024-05-19 22:55:58.437101 qctrl_experiment_scheduler-0.5.0/qctrlexperimentscheduler/__init__.py
+-rwxr-xr-x   0        0        0    18635 2024-05-19 22:55:35.209302 qctrl_experiment_scheduler-0.5.0/qctrlexperimentscheduler/graph.py
+-rw-r--r--   0        0        0     8557 2024-05-19 22:55:35.209302 qctrl_experiment_scheduler-0.5.0/qctrlexperimentscheduler/graph_traversal.py
+-rw-r--r--   0        0        0    11020 2024-05-19 22:55:35.209302 qctrl_experiment_scheduler-0.5.0/qctrlexperimentscheduler/node.py
+-rwxr-xr-x   0        0        0      990 2024-05-19 22:55:58.437101 qctrl_experiment_scheduler-0.5.0/qctrlexperimentscheduler/predefined/__init__.py
+-rw-r--r--   0        0        0    19928 2024-05-19 22:55:35.209302 qctrl_experiment_scheduler-0.5.0/qctrlexperimentscheduler/predefined/amplitude_calibration.py
+-rw-r--r--   0        0        0    16220 2024-05-19 22:55:35.209302 qctrl_experiment_scheduler-0.5.0/qctrlexperimentscheduler/predefined/simulation_backend.py
+-rw-r--r--   0        0        0     7256 2024-05-19 22:55:35.209302 qctrl_experiment_scheduler-0.5.0/qctrlexperimentscheduler/variable.py
+-rw-r--r--   0        0        0     2323 1970-01-01 00:00:00.000000 qctrl_experiment_scheduler-0.5.0/PKG-INFO
```

### Comparing `qctrl_experiment_scheduler-0.4.0/LICENSE` & `qctrl_experiment_scheduler-0.5.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
                             Q-CTRL Terms of service
-                            Updated August 8, 2022
+                            Updated November 8, 2023
                             https://q-ctrl.com/terms
 
 BY ACCEPTING THESE TERMS OF SERVICE YOU ARE ENTERING INTO A BINDING AGREEMENT
 THAT APPLIES TO ANY USE OF THE PLATFORM. WE HAVE ENDEAVORED TO MAKE THE TERMS
 SIMPLE AND CLEAR. YOU ACKNOWLEDGE THAT YOU HAVE READ AND UNDERSTOOD THIS
 AGREEMENT, AND REPRESENT THAT YOU HAVE THE AUTHORITY TO ENTER INTO THIS
 AGREEMENT ON BEHALF OF ANY ORGANIZATION OR PERSON FOR WHOM YOU ARE USING THE
@@ -106,17 +106,16 @@
 
 "Platform" shall mean the software made available by us from time to time via
 the access method, as may be changed or updated from time to time by us. The
 features of the platform available to you will depend on the plan you have
 subscribed to and whether the platform is hosted by us, hosted on-premises, or
 installed locally.
 
-"Q-CTRL" shall mean Q-CTRL Pty Ltd (ABN 78 622 325 535) of ℅ Scendar, Suite 1,
-Level 18, 219-227 Elizabeth Street, SYDNEY NSW 2000, Australia (also referred to
-as "we", "us" or "our").
+"Q-CTRL" shall mean Q-CTRL Pty Ltd (ABN 78 622 325 535) - Sydney, Australia
+(also referred to as "we", "us" or "our").
 
 "Subscriber" shall mean the person who registers to use the platform and, where
 the context permits, includes any entity on whose behalf that person registers
 to use the platform.
 
 "Support" shall mean the support services offered to you by us, the nature and
 extent of such are determined by your plan.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qctrl_experiment_scheduler-0.4.0/pyproject.toml` & `qctrl_experiment_scheduler-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [tool.poetry]
 name = "qctrl-experiment-scheduler"
-version = "0.4.0"
+version = "0.5.0"
 description = "Q-CTRL Experiment Scheduler"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
-repository = ""
-documentation = ""
+documentation = "https://docs.q-ctrl.com/references/qctrl-experiment-scheduler/"
 keywords = [
     "black opal",
     "boulder opal",
     "fire opal",
     "nisq",
     "open controls",
     "q control",
@@ -42,15 +41,14 @@
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "Natural Language :: English",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Software Development :: Embedded Systems",
@@ -64,33 +62,34 @@
 LinkedIn = "https://www.linkedin.com/company/q-ctrl/"
 Facebook = "https://www.facebook.com/qctrl"
 Twitter = "https://twitter.com/qctrlHQ"
 YouTube = "https://www.youtube.com/qctrl"
 GitHub = "https://github.com/qctrl"
 
 [tool.poetry.dependencies]
-python = ">=3.8, <3.12"
+python = ">=3.9, <3.12"
 numpy = "^1.23.5"
 networkx = "^2.7"
 boulder-opal = { version = "^1.0.0", source = "PyPI" }
-qctrl-commons = { version = "^21.0.0", source = "PyPI" }
-qctrl-sphinx-theme = { version = "^2.1.3", source = "PyPI" }
-qctrl-visualizer = { version = "^6.1.3", source = "PyPI" }
+qctrl-commons = "^21.2.4"
+qctrl-visualizer = "^6.1.3"
 
 [tool.poetry.dev-dependencies]
-black = "^23.7.0"
+black = "^24.3.0"
 isort = "^5.12.0"
 mypy = "^1.5.1"
 pre-commit = "^3.3.3"
 pylint = "^2.17.1"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
+qctrl-sphinx-theme = "^2.1.4"
 sphinx = "^5.0.0"
 sphinx-reredirects = "^0.0.1"
 tomli = "^2.0.1"
+sphinx-markdown-builder = "^0.6.6"
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "supplemental"
 
 [[tool.poetry.source]]
 name = "Q-CTRL PyPI"
```

### Comparing `qctrl_experiment_scheduler-0.4.0/qctrlexperimentscheduler/__init__.py` & `qctrl_experiment_scheduler-0.5.0/qctrlexperimentscheduler/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Q-CTRL. All rights reserved.
+# Copyright 2024 Q-CTRL. All rights reserved.
 #
 # Licensed under the Q-CTRL Terms of service (the "License"). Unauthorized
 # copying or use of this file, via any medium, is strictly prohibited.
 # Proprietary and confidential. You may not use this file except in compliance
 # with the License. You may obtain a copy of the License at
 #
 #    https://q-ctrl.com/terms
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 """
 Q-CTRL Experiment Scheduler
 """
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 __author__ = "Q-CTRL <support@q-ctrl.com>"
 
 from qctrlexperimentscheduler.graph import (
     CalibrationGraph,
     CalibrationProtocol,
 )
 from qctrlexperimentscheduler.graph_traversal import Verbosity
```

### Comparing `qctrl_experiment_scheduler-0.4.0/qctrlexperimentscheduler/graph.py` & `qctrl_experiment_scheduler-0.5.0/qctrlexperimentscheduler/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Q-CTRL. All rights reserved.
+# Copyright 2024 Q-CTRL. All rights reserved.
 #
 # Licensed under the Q-CTRL Terms of service (the "License"). Unauthorized
 # copying or use of this file, via any medium, is strictly prohibited.
 # Proprietary and confidential. You may not use this file except in compliance
 # with the License. You may obtain a copy of the License at
 #
 #    https://q-ctrl.com/terms
@@ -90,15 +90,15 @@
     therein. Afterwards, the bounding box is computed. In the future, it might make
     sense to compute the size without creating a `plt.figure`. Also see the following
     discussion in the PR:
     https://github.com/qctrl/experiment-scheduler/pull/44#discussion_r1120879110.
     """
 
     figure = plt.figure()
-    renderer = figure.canvas.get_renderer()
+    renderer = figure.canvas.get_renderer()  # type: ignore
     text_box = plt.text(0, 0, text, fontsize=font_size)
 
     bounding_box = text_box.get_window_extent(renderer=renderer)
     width = bounding_box.width
     height = bounding_box.height
     plt.close()
 
@@ -492,15 +492,15 @@
             # of the origin and `x1`, `y1` determine the size of the axis. These parameters are
             # retrieved through`.bounds`. Since we are only interested in the size, we select
             # `x1` (figure_width) and `y1` (figure_height).
             figure_width, figure_height = (
                 scaling
                 * pixels
                 * np.array(
-                    axis.get_tightbbox(renderer=fig.canvas.get_renderer()).bounds
+                    axis.get_tightbbox(renderer=fig.canvas.get_renderer()).bounds  # type: ignore
                 )[2:4]
             )
         else:
             check_argument(
                 isinstance(figure_size, list) and len(figure_size) == 2,
                 "figure_size must be a list of length 2.",
                 {"figure_size": figure_size},
```

### Comparing `qctrl_experiment_scheduler-0.4.0/qctrlexperimentscheduler/graph_traversal.py` & `qctrl_experiment_scheduler-0.5.0/qctrlexperimentscheduler/graph_traversal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Q-CTRL. All rights reserved.
+# Copyright 2024 Q-CTRL. All rights reserved.
 #
 # Licensed under the Q-CTRL Terms of service (the "License"). Unauthorized
 # copying or use of this file, via any medium, is strictly prohibited.
 # Proprietary and confidential. You may not use this file except in compliance
 # with the License. You may obtain a copy of the License at
 #
 #    https://q-ctrl.com/terms
```

### Comparing `qctrl_experiment_scheduler-0.4.0/qctrlexperimentscheduler/node.py` & `qctrl_experiment_scheduler-0.5.0/qctrlexperimentscheduler/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Q-CTRL. All rights reserved.
+# Copyright 2024 Q-CTRL. All rights reserved.
 #
 # Licensed under the Q-CTRL Terms of service (the "License"). Unauthorized
 # copying or use of this file, via any medium, is strictly prohibited.
 # Proprietary and confidential. You may not use this file except in compliance
 # with the License. You may obtain a copy of the License at
 #
 #    https://q-ctrl.com/terms
```

### Comparing `qctrl_experiment_scheduler-0.4.0/qctrlexperimentscheduler/predefined/__init__.py` & `qctrl_experiment_scheduler-0.5.0/qctrlexperimentscheduler/predefined/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Q-CTRL. All rights reserved.
+# Copyright 2024 Q-CTRL. All rights reserved.
 #
 # Licensed under the Q-CTRL Terms of service (the "License"). Unauthorized
 # copying or use of this file, via any medium, is strictly prohibited.
 # Proprietary and confidential. You may not use this file except in compliance
 # with the License. You may obtain a copy of the License at
 #
 #    https://q-ctrl.com/terms
```

### Comparing `qctrl_experiment_scheduler-0.4.0/qctrlexperimentscheduler/predefined/amplitude_calibration.py` & `qctrl_experiment_scheduler-0.5.0/qctrlexperimentscheduler/predefined/amplitude_calibration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Q-CTRL. All rights reserved.
+# Copyright 2024 Q-CTRL. All rights reserved.
 #
 # Licensed under the Q-CTRL Terms of service (the "License"). Unauthorized
 # copying or use of this file, via any medium, is strictly prohibited.
 # Proprietary and confidential. You may not use this file except in compliance
 # with the License. You may obtain a copy of the License at
 #
 #    https://q-ctrl.com/terms
```

### Comparing `qctrl_experiment_scheduler-0.4.0/qctrlexperimentscheduler/predefined/simulation_backend.py` & `qctrl_experiment_scheduler-0.5.0/qctrlexperimentscheduler/predefined/simulation_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Q-CTRL. All rights reserved.
+# Copyright 2024 Q-CTRL. All rights reserved.
 #
 # Licensed under the Q-CTRL Terms of service (the "License"). Unauthorized
 # copying or use of this file, via any medium, is strictly prohibited.
 # Proprietary and confidential. You may not use this file except in compliance
 # with the License. You may obtain a copy of the License at
 #
 #    https://q-ctrl.com/terms
```

### Comparing `qctrl_experiment_scheduler-0.4.0/qctrlexperimentscheduler/variable.py` & `qctrl_experiment_scheduler-0.5.0/qctrlexperimentscheduler/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Q-CTRL. All rights reserved.
+# Copyright 2024 Q-CTRL. All rights reserved.
 #
 # Licensed under the Q-CTRL Terms of service (the "License"). Unauthorized
 # copying or use of this file, via any medium, is strictly prohibited.
 # Proprietary and confidential. You may not use this file except in compliance
 # with the License. You may obtain a copy of the License at
 #
 #    https://q-ctrl.com/terms
@@ -93,24 +93,24 @@
         calibration variable.
 
         You can use this to use Boulder Opal's graphs to perform curve
         fitting with the calibration variables.
 
         Parameters
         ----------
-        graph : :py:class:`~qctrl.graphs.Graph`
+        graph : :py:class:`~boulderopal.Graph`
             The Boulder Opal model-based optimization graph object to
             which you want to pass the variable.
         name : str or None, optional
             The name of the variable in the Boulder Opal graph. Defaults to
             the same name of the calibration variable.
 
         Returns
         -------
-        :py:class:`~qctrl.graphs.Tensor`
+        :py:class:`~boulderopal.graph.Tensor`
             The name of the tensor that corresponds to the optimization
             variable.
         """
         check_argument(
             isinstance(graph, Graph),
             "The graph must be a Boulder Opal optimization graph.",
             {"graph": graph},
```


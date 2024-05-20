# Comparing `tmp/qnngds-2.4.1.tar.gz` & `tmp/qnngds-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qnngds-2.4.1.tar", last modified: Wed May 15 18:22:39 2024, max compression
+gzip compressed data, was "qnngds-2.5.0.tar", last modified: Mon May 20 15:57:43 2024, max compression
```

## Comparing `qnngds-2.4.1.tar` & `qnngds-2.5.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1100 2024-04-04 20:17:36.246389 qnngds-2.4.1/LICENSE.txt
--rw-r--r--   0        0        0     1158 2024-05-08 16:03:17.277791 qnngds-2.4.1/README.md
--rw-r--r--   0        0        0     1161 2024-05-15 18:22:39.668427 qnngds-2.4.1/pyproject.toml
--rw-r--r--   0        0        0      558 2024-05-15 16:51:34.256862 qnngds-2.4.1/src/qnngds/__init__.py
--rw-r--r--   0        0        0      308 2024-05-08 19:19:07.161040 qnngds-2.4.1/src/qnngds/_default_param.py
--rw-r--r--   0        0        0    29562 2024-05-15 18:17:45.122055 qnngds-2.4.1/src/qnngds/cells.py
--rw-r--r--   0        0        0    10670 2024-05-14 21:22:22.267309 qnngds-2.4.1/src/qnngds/circuits.py
--rw-r--r--   0        0        0    31300 2024-05-15 18:17:45.123054 qnngds-2.4.1/src/qnngds/design.py
--rw-r--r--   0        0        0      162 2024-05-08 19:19:07.169035 qnngds-2.4.1/src/qnngds/devices/__init__.py
--rw-r--r--   0        0        0      237 2024-05-08 19:19:07.169035 qnngds-2.4.1/src/qnngds/devices/htron.py
--rw-r--r--   0        0        0     1355 2024-05-14 21:22:22.267309 qnngds-2.4.1/src/qnngds/devices/nanowire.py
--rw-r--r--   0        0        0     3248 2024-05-14 21:22:22.267309 qnngds-2.4.1/src/qnngds/devices/ntron.py
--rw-r--r--   0        0        0     6550 2024-05-14 21:22:22.267309 qnngds-2.4.1/src/qnngds/devices/resistor.py
--rw-r--r--   0        0        0     4705 2024-05-15 18:17:45.129726 qnngds-2.4.1/src/qnngds/devices/snspd.py
--rw-r--r--   0        0        0     1343 2024-05-14 21:22:22.267309 qnngds-2.4.1/src/qnngds/geometries.py
--rw-r--r--   0        0        0     8949 2024-05-14 21:22:22.267309 qnngds-2.4.1/src/qnngds/tests.py
--rw-r--r--   0        0        0    29441 2024-05-15 18:17:45.137086 qnngds-2.4.1/src/qnngds/utilities.py
--rw-r--r--   0        0        0  1099544 2024-05-15 17:54:44.364180 qnngds-2.4.1/tests/all_dev.gds
--rw-r--r--   0        0        0     3430 2024-05-15 18:17:45.139090 qnngds-2.4.1/tests/all_dev_on_gds.py
--rw-r--r--   0        0        0      953 2024-05-15 18:17:45.139090 qnngds-2.4.1/tests/single_dev_on_gds.py
--rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 qnngds-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-05-20 15:57:30.798371 qnngds-2.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1129 2024-05-20 15:57:30.798371 qnngds-2.5.0/README.md
+-rw-r--r--   0        0        0     1161 2024-05-20 15:57:43.642317 qnngds-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0      543 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/__init__.py
+-rw-r--r--   0        0        0      290 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/_default_param.py
+-rw-r--r--   0        0        0    29539 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/cells.py
+-rw-r--r--   0        0        0    10385 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/circuits.py
+-rw-r--r--   0        0        0    30497 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/design.py
+-rw-r--r--   0        0        0      158 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/devices/__init__.py
+-rw-r--r--   0        0        0      231 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/devices/htron.py
+-rw-r--r--   0        0        0     1313 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/devices/nanowire.py
+-rw-r--r--   0        0        0     3136 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/devices/ntron.py
+-rw-r--r--   0        0        0     6365 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/devices/resistor.py
+-rw-r--r--   0        0        0     6479 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/devices/snspd.py
+-rw-r--r--   0        0        0     1300 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/geometries.py
+-rw-r--r--   0        0        0     8683 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/tests.py
+-rw-r--r--   0        0        0    30179 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/utilities.py
+-rw-r--r--   0        0        0     3316 2024-05-20 15:57:30.814370 qnngds-2.5.0/tests/all_dev_on_gds.py
+-rw-r--r--   0        0        0     1126 2024-05-20 15:57:30.814370 qnngds-2.5.0/tests/single_dev_on_gds.py
+-rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 qnngds-2.5.0/PKG-INFO
```

### Comparing `qnngds-2.4.1/LICENSE.txt` & `qnngds-2.5.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2016 The Python Packaging Authority (PyPA)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (c) 2016 The Python Packaging Authority (PyPA)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `qnngds-2.4.1/README.md` & `qnngds-2.5.0/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# QNNGDS
-
-## Description
-QNNGDS is a toolbox built on top of phidl for device design in the QNN group.
-It is made for helping in the design of gds files. The package is composed of 5 main modules:
-- design (contains pre-built cells, ready to be added to a design)
-- utilities (contains useful functions for building a new cell)
-- geometries (contains test structures and geometry tools)
-- circuits (contains circuits made of devices)
-- devices (contains devices like ntron, htron, snspd)
-
-## Getting Started
-### Installing
-- Make sure [gdspy](https://pypi.org/project/gdspy/) is installed
-- Install qnngds package with 'pip install qnngds'
-
-### Dependencies
-- [phidl](https://pypi.org/project/phidl/)
-- [scipy](https://pypi.org/project/scipy/)
-
-## License
-This project is licensed under the MIT License - see the LICENSE.txt file for details
-
-## [Documentation](https://qnngds.readthedocs.io/en/latest/)
-- [API](https://qnngds.readthedocs.io/en/latest/api.html)
-- [Tutorials](https://qnngds.readthedocs.io/en/latest/tutorials.html)
-
-## How to contribute
-- [Developer's documentation](https://qnngds-dev.readthedocs.io/en/latest)
+# QNNGDS
+
+## Description
+QNNGDS is a toolbox built on top of phidl for device design in the QNN group.
+It is made for helping in the design of gds files. The package is composed of 5 main modules:
+- design (contains pre-built cells, ready to be added to a design)
+- utilities (contains useful functions for building a new cell)
+- geometries (contains test structures and geometry tools)
+- circuits (contains circuits made of devices)
+- devices (contains devices like ntron, htron, snspd)
+
+## Getting Started
+### Installing
+- Make sure [gdspy](https://pypi.org/project/gdspy/) is installed
+- Install qnngds package with 'pip install qnngds'
+
+### Dependencies
+- [phidl](https://pypi.org/project/phidl/)
+- [scipy](https://pypi.org/project/scipy/)
+
+## License
+This project is licensed under the MIT License - see the LICENSE.txt file for details
+
+## [Documentation](https://qnngds.readthedocs.io/en/latest/)
+- [API](https://qnngds.readthedocs.io/en/latest/api.html)
+- [Tutorials](https://qnngds.readthedocs.io/en/latest/tutorials.html)
+
+## How to contribute
+- [Developer's documentation](https://qnngds-dev.readthedocs.io/en/latest)
```

### Comparing `qnngds-2.4.1/pyproject.toml` & `qnngds-2.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "qnngds"
-version = "2.4.1"
+version = "2.5.0"
 authors = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
     { name = "A. Jacquillat", email = "audrey.jacquillat@gmail.com" },
     { name = "R. Foster", email = "reedf@mit.edu" },
 ]
 maintainers = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
```

### Comparing `qnngds-2.4.1/src/qnngds/__init__.py` & `qnngds-2.5.0/src/qnngds/__init__.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from . import devices, circuits, cells, design, geometries, tests, utilities
-
-
-def help():
-    """Provides links to documentation."""
-
-    print(
-        "Need help? Check qnngds documentation: https://qnngds.readthedocs.io/en/latest/ \n"
-    )
-    print(" - Tutorials: https://qnngds.readthedocs.io/en/latest/tutorials.html \n")
-    print(" - API: https://qnngds.readthedocs.io/en/latest/api.html \n\n")
-
-    print(
-        "You are a contributor? Check this documentation: https://qnngds.readthedocs.io/projects/qnngds-dev/en/latest/"
-    )
+from . import devices, circuits, cells, design, geometries, tests, utilities
+
+
+def help():
+    """Provides links to documentation."""
+
+    print(
+        "Need help? Check qnngds documentation: https://qnngds.readthedocs.io/en/latest/ \n"
+    )
+    print(" - Tutorials: https://qnngds.readthedocs.io/en/latest/tutorials.html \n")
+    print(" - API: https://qnngds.readthedocs.io/en/latest/api.html \n\n")
+
+    print(
+        "You are a contributor? Check this documentation: https://qnngds.readthedocs.io/projects/qnngds-dev/en/latest/"
+    )
```

### Comparing `qnngds-2.4.1/src/qnngds/cells.py` & `qnngds-2.5.0/src/qnngds/cells.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,803 +1,823 @@
-"""Library of pre-built cells containing text, border marks, and an experiment,
-connected to pads for wirebonding."""
-
-from phidl import Device
-import phidl.geometry as pg
-import phidl.routing as pr
-from typing import Tuple, List, Union, Optional
-import math
-
-import qnngds.tests as test
-import qnngds.devices as device
-import qnngds.circuits as circuit
-import qnngds.utilities as utility
-import qnngds._default_param as dflt
-
-# basics
-
-
-def alignment(
-    die_w: Union[int, float] = dflt.die_w,
-    layers_to_align: List[int] = [dflt.layers["die"], dflt.layers["pad"]],
-    outline_die: Union[int, float] = dflt.die_outline,
-    die_layer: int = dflt.layers["die"],
-    text: Union[None, str] = dflt.text,
-) -> Device:
-    """Creates alignment marks in an integer number of unit cells.
-
-    Parameters:
-        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
-        layers_to_align (list of int): Layers to align.
-        outline_die (int or float): The width of the die's outline.
-        die_layer (int): The layer where the die is placed.
-        text (str, optional): If None, the text is f"lay={layers_to_align}".
-
-    Returns:
-        DIE_ALIGN (Device): A device that centers the alignment marks in an n*m unit cell.
-    """
-
-    if text is None:
-        text = f"lay={layers_to_align}"
-    DIE = Device(f"CELL.ALIGN({text})")
-
-    ALIGN = test.alignment_mark(layers_to_align)
-
-    n = math.ceil((ALIGN.xsize) / die_w)
-    m = math.ceil((ALIGN.ysize) / die_w)
-
-    BORDER = utility.die_cell(
-        die_size=(n * die_w, m * die_w),
-        device_max_size=(ALIGN.xsize + 20, ALIGN.ysize + 20),
-        ports={},
-        ports_gnd={},
-        isolation=outline_die,
-        text=f"ALIGN {text}",
-        layer=die_layer,
-        invert=True,
-    )
-
-    DIE << BORDER.flatten()
-    DIE << ALIGN
-
-    return DIE
-
-
-def vdp(
-    die_w: Union[int, float] = dflt.die_w,
-    pad_size: Tuple[float] = dflt.pad_size,
-    layers_to_probe: List[int] = [dflt.layers["die"]],
-    layers_to_outline: Union[None, List[int]] = dflt.auto_param,
-    outline: Union[int, float] = dflt.die_outline,
-    die_layer: Union[int, float] = dflt.layers["die"],
-    pad_layer: int = dflt.layers["pad"],
-    text: Union[None, str] = dflt.text,
-) -> Device:
-    r"""Creates a cell containing a Van Der Pauw structure between 4 contact
-    pads.
-
-    Parameters:
-        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
-        pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
-        layers_to_probe (list of int): The layers on which to place the VDP structure.
-        layers_to_outline (list of int): Among the VDP layers, the ones for which structure must not be filled but outlined.
-        outline (int or float): The width of the VDP and die's outline.
-        die_layer (int or tuple of int): The layer where the die is placed.
-        pad_layer (int or tuple of int): The layer where the pads are placed.
-        text (str, optional): If None, the text is f"lay={layers_to_probe}".
-    Returns:
-        DIE_VANDP (Device): The created device.
-    """
-    # Initialize parameters left to default (=None)
-
-    if text is None:
-        text = f"lay={layers_to_probe}"
-    if layers_to_outline is None:
-        layers_to_outline = [die_layer]  # default layer to outline if None is given
-
-    DIE_VANDP = Device(f"CELL.VDP({text})")
-
-    device_max_w = die_w - 2 * (
-        pad_size[1] + 2 * outline
-    )  # width of max device size for this cell
-    contact_w = device_max_w / 10  # choosing a contact width 10 times smaller
-    device_w = (
-        device_max_w - 2 * contact_w
-    )  # choosing a smaller device to have space for routing from pad to contact
-
-    # Creates the DIE, it contains only the cell text and bordure
-
-    DIE = utility.die_cell(
-        die_size=(die_w, die_w),
-        device_max_size=(device_max_w, device_max_w),
-        ports={},
-        ports_gnd=[],
-        isolation=outline,
-        text=f"VDP \n{text}",
-        layer=die_layer,
-        pad_layer=pad_layer,
-        invert=True,
-        fill_pad_layer=False,
-    )
-    DIE_VANDP << DIE.flatten()
-
-    # Creates the vdp structure, add pads and route
-
-    VDP = Device()
-
-    ## VDP probed area
-    AREA = test.vdp(device_w, contact_w)
-    VDP << AREA
-
-    ## pads
-    PADS = utility.die_cell(
-        die_size=(die_w, die_w),
-        device_max_size=(device_max_w, device_max_w),
-        pad_size=pad_size,
-        contact_w=pad_size[0],
-        contact_l=0,
-        ports={"N": 1, "E": 1, "W": 1, "S": 1},
-        ports_gnd=["N", "E", "W", "S"],
-        isolation=outline,
-        text="PADS ONLY",
-        layer=0,
-        pad_layer=pad_layer,
-        invert=False,
-        fill_pad_layer=False,
-    )
-    PADS.remove_layers([pad_layer], invert_selection=True)
-    VDP << PADS
-
-    ## routes from pads to probing area
-    ROUTES = utility.route_to_dev(PADS.get_ports(), AREA.ports)
-    VDP << ROUTES
-
-    VDP.flatten(0)
-
-    # Outline the vdp structure for layers that need to be outlined
-
-    DEVICE = Device(f"VDP(lay={layers_to_probe})")
-
-    for layer in layers_to_probe:
-        TEST_LAY = pg.deepcopy(VDP)
-        if layer in layers_to_outline:
-            TEST_LAY = pg.outline(TEST_LAY, outline)
-        TEST_LAY.name = f"VDP(lay={layer})"
-        DEVICE << TEST_LAY.flatten(single_layer=layer)
-
-    DIE_VANDP << DEVICE
-
-    # Add pads if they are not in already present
-    if pad_layer not in layers_to_probe:
-        PADS = pg.union(PADS, layer=pad_layer)
-        PADS.name = "PADS"
-        DIE_VANDP << PADS
-
-    return DIE_VANDP
-
-
-def etch_test(
-    die_w: Union[int, float] = dflt.die_w,
-    layers_to_etch: List[List[int]] = [[dflt.layers["pad"]]],
-    outline_die: Union[int, float] = dflt.die_outline,
-    die_layer: int = dflt.layers["die"],
-    text: Union[None, str] = dflt.text,
-) -> Device:
-    """Creates etch test structures in an integer number of unit cells.
-
-    These test structures are thought to be used by probing on pads (with a
-    simple multimeter) that should be isolated one from another if the etching
-    is complete.
-
-    Parameters:
-        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
-        layers_to_etch (list of list of int): Each element of the list corresponds to one test point, to put on the list of layers specified.
-                                               Example: [[1, 2], [1], [2]]
-        outline_die (int or float): The width of the die's outline.
-        die_layer (int): The layer where the die is placed.
-        text (str, optional): If None, the text is f"lay={layers_to_etch}".
-
-    Returns:
-        DIE_ETCH_TEST (Device): A device (with size n*m of unit cells) with etch tests in its center.
-    """
-
-    if text is None:
-        text = f"lay={layers_to_etch}"
-    DIE_ETCH_TEST = Device(f"CELL.ETCH_TEST({text})")
-
-    TEST = Device(f"ETCH_TEST({text})")
-
-    ## Create the probing areas
-
-    margin = 0.12 * die_w
-    rect = pg.rectangle((die_w - 2 * margin, die_w - 2 * margin))
-    for i, layer_to_etch in enumerate(layers_to_etch):
-        probe = Device()
-        probe.add_array(rect, 2, 1, (die_w, die_w))
-        for layer in layer_to_etch:
-            TEST << pg.outline(probe, -outline_die, layer=layer).movey(i * die_w)
-
-    ## Create the die
-
-    n = math.ceil((TEST.xsize + 2 * dflt.die_cell_border) / die_w)
-    m = math.ceil((TEST.ysize + 2 * dflt.die_cell_border) / die_w)
-    BORDER = utility.die_cell(
-        die_size=(n * die_w, m * die_w),
-        ports={},
-        ports_gnd={},
-        text=f"ETCH TEST {text}",
-        isolation=outline_die,
-        layer=die_layer,
-        invert=True,
-    )
-
-    BORDER.move(TEST.center)
-    DIE_ETCH_TEST << BORDER.flatten()
-    DIE_ETCH_TEST << TEST.flatten()
-    DIE_ETCH_TEST.move(DIE_ETCH_TEST.center, (0, 0))
-
-    return DIE_ETCH_TEST
-
-
-def resolution_test(
-    die_w: Union[int, float] = dflt.die_w,
-    layer_to_resolve: int = dflt.layers["device"],
-    resolutions_to_test: List[float] = [
-        0.025,
-        0.05,
-        0.075,
-        0.1,
-        0.25,
-        0.5,
-        1,
-        1.5,
-        2.0,
-    ],
-    outline: Union[int, float] = dflt.die_outline,
-    die_layer: int = dflt.layers["die"],
-    text: Union[None, str] = dflt.text,
-) -> Device:
-    r"""Creates a cell containing a resolution test.
-
-    Parameters:
-        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
-        layer_to_resolve (int): The layer to put the resolution test on.
-        resolutions_to_test (list of float): The resolutions to test in µm.
-        outline (int or float): The width of the VDP and die's outline.
-        die_layer (int or tuple of int): The layer where the die is placed.
-        text (str, optional): If None, the text is f"lay={layer_to_resolve}".
-
-    Returns:
-        DIE_RES_TEST (Device): The created device.
-    """
-
-    if text is None:
-        text = f"lay={layer_to_resolve}"
-    DIE_RES_TEST = Device(f"CELL.RESOLUTION_TEST({text})")
-
-    ## Create the test structure
-    TEST_RES = Device(f"RESOLUTION_TEST({text})")
-    test_res = TEST_RES << test.resolution_test(
-        resolutions=resolutions_to_test, inverted=False, layer=layer_to_resolve
-    )
-    test_res_invert = TEST_RES << test.resolution_test(
-        resolutions=resolutions_to_test,
-        inverted=resolutions_to_test[-1],
-        layer=layer_to_resolve,
-    )
-    test_res_invert.movey(
-        test_res_invert.ymin, test_res.ymax + 5 * resolutions_to_test[-1]
-    )
-
-    DIE_RES_TEST << TEST_RES.move(TEST_RES.center, (0, 0))
-
-    ## Create the die
-    n = math.ceil((TEST_RES.xsize) / die_w)
-    m = math.ceil((TEST_RES.ysize) / die_w)
-    BORDER = utility.die_cell(
-        die_size=(n * die_w, m * die_w),
-        ports={},
-        ports_gnd=[],
-        text=f"RES TEST \n{text}",
-        isolation=outline,
-        layer=die_layer,
-        invert=True,
-    )
-
-    DIE_RES_TEST << BORDER.flatten()
-    return DIE_RES_TEST
-
-
-## devices:
-
-
-def nanowires(
-    die_w: Union[int, float] = dflt.die_w,
-    pad_size: Tuple[float] = dflt.pad_size,
-    channels_sources_w: List[Tuple[float, float]] = [(0.1, 1), (0.5, 3), (1, 10)],
-    overlap_w: Union[int, float] = dflt.ebeam_overlap,
-    outline_die: Union[int, float] = dflt.die_outline,
-    outline_dev: Union[int, float] = dflt.device_outline,
-    device_layer: int = dflt.layers["device"],
-    die_layer: int = dflt.layers["die"],
-    pad_layer: int = dflt.layers["pad"],
-    text: Union[None, str] = dflt.text,
-    fill_pad_layer: bool = False,
-) -> Device:
-    """Creates a cell that contains several nanowires of given channel and
-    source.
-
-    Parameters:
-        die_w (int or float): Width of a unit die/cell in the design (the output
-            device will be an integer number of unit cells).
-        pad_size (tuple of int or float): Dimensions of the die's pads (width,
-            height).
-        channels_sources_w (list of tuple of float): The list of (channel_w,
-            source_w) of the nanowires to create.
-        overlap_w (int or float): Extra length of the routes above the die's
-            ports to assure alignment with the device (useful for ebeam
-            lithography).
-        outline_die (int or float): The width of the pads outline.
-        outline_dev (int or float): The width of the device's outline.
-        device_layer (int or tuple of int): The layer where the device is placed.
-        die_layer (int or tuple of int): The layer where the die is placed.
-        pad_layer (int or tuple of int): The layer where the pads are placed.
-        text (str, optional): If None, the text is f"w={channels_w}".
-        fill_pad_layer (bool): If True, the space reserved for pads in the
-            die_cell in filled in pad's layer.
-
-    Returns:
-        Device: A device (of size n*m unit cells) containing the nanowires, the
-        border of the die (created with die_cell function), and the connections
-        between the nanowires and pads.
-    """
-
-    if text is None:
-        channels_w = [item[0] for item in channels_sources_w]
-        text = f"w={channels_w}"
-    cell_text = text.replace(" \n", ", ")
-
-    NANOWIRES_DIE = Device(f"CELL.NWIRES({cell_text})")
-
-    DEVICE = Device(f"NWIRES({cell_text})")
-
-    ## Create the NANOWIRES
-
-    NANOWIRES = Device(f"NWIRES({cell_text})")
-    nanowires_ref = []
-    for i, channel_source_w in enumerate(channels_sources_w):
-        nanowire_ref = NANOWIRES << device.nanowire.spot(
-            channel_source_w[0], channel_source_w[1]
-        )
-        nanowires_ref.append(nanowire_ref)
-    DEVICE << NANOWIRES
-
-    ## Create the DIE
-
-    # die parameters, checkup conditions
-    n = len(channels_sources_w)
-    die_size = (math.ceil((2 * (n + 1) * pad_size[0]) / die_w) * die_w, die_w)
-    die_contact_w = NANOWIRES.xsize + overlap_w
-    dev_contact_w = NANOWIRES.xsize
-    routes_margin = 4 * die_contact_w
-    dev_max_size = (2 * n * pad_size[0], NANOWIRES.ysize + routes_margin)
-
-    # die, with calculated parameters
-    BORDER = utility.die_cell(
-        die_size=die_size,
-        device_max_size=dev_max_size,
-        pad_size=pad_size,
-        contact_w=die_contact_w,
-        contact_l=overlap_w,
-        ports={"N": n, "S": n},
-        ports_gnd=["S"],
-        isolation=outline_die,
-        text=f"NWIRES\n{text}",
-        layer=die_layer,
-        pad_layer=pad_layer,
-        invert=True,
-        fill_pad_layer=fill_pad_layer,
-    )
-
-    ## Place the nanowires
-
-    for i, nanowire_ref in enumerate(nanowires_ref):
-        nanowire_ref.movex(BORDER.ports[f"N{i+1}"].x)
-        NANOWIRES.add_port(port=nanowire_ref.ports[1], name=f"N{i+1}")
-        NANOWIRES.add_port(port=nanowire_ref.ports[2], name=f"S{i+1}")
-
-    ## Route the nanowires and the die
-
-    # hyper tapers
-    HT, dev_ports = utility.add_hyptap_to_cell(
-        BORDER.get_ports(), overlap_w, dev_contact_w
-    )
-    DEVICE.ports = dev_ports.ports
-    DEVICE << HT
-
-    # routes from nanowires to hyper tapers
-    ROUTES = utility.route_to_dev(HT.get_ports(), NANOWIRES.ports)
-    DEVICE << ROUTES
-
-    DEVICE.ports = dev_ports.ports
-    DEVICE = pg.outline(
-        DEVICE, outline_dev, open_ports=2 * outline_dev, layer=device_layer
-    )
-    DEVICE.name = f"NWIRES({cell_text})"
-
-    NANOWIRES_DIE << DEVICE
-    NANOWIRES_DIE << BORDER
-
-    return NANOWIRES_DIE
-
-
-def ntron(
-    die_w: Union[int, float] = dflt.die_w,
-    pad_size: Tuple[float, float] = dflt.pad_size,
-    choke_w: Union[int, float] = 0.1,
-    channel_w: Union[int, float] = 0.5,
-    gate_w: Union[None, int, float] = dflt.auto_param,
-    source_w: Union[None, int, float] = dflt.auto_param,
-    drain_w: Union[None, int, float] = dflt.auto_param,
-    choke_shift: Union[None, int, float] = dflt.auto_param,
-    overlap_w: Union[None, int, float] = dflt.ebeam_overlap,
-    outline_die: Union[None, int, float] = dflt.die_outline,
-    outline_dev: Union[None, int, float] = dflt.device_outline,
-    device_layer: int = dflt.layers["device"],
-    die_layer: int = dflt.layers["die"],
-    pad_layer: int = dflt.layers["pad"],
-    text: Union[None, str] = dflt.text,
-    fill_pad_layer: bool = False,
-) -> Device:
-    r"""Creates a standardized cell specifically for a single ntron.
-
-    Unless specified, scales the ntron parameters as:
-    gate_w = drain_w = source_w = 3 * channel_w
-    choke_shift = -3 * channel_w
-
-    Parameters:
-        die_w (int or float): Width of a unit die/cell in the design (the output
-            device will be an integer number of unit cells).
-        pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
-        choke_w (int or float): The width of the ntron's choke in µm.
-        channel_w (int or float): The width of the ntron's channel in µm.
-        gate_w (int or float, optional): If None, gate width is 3 times the channel width.
-        source_w (int or float, optional): If None, source width is 3 times the channel width.
-        drain_w (int or float, optional): If None, drain width is 3 times the channel width.
-        choke_shift (int or float, optional): If None, choke shift is -3 times the channel width.
-        overlap_w (int or float): Extra length of the routes above the die's
-            ports to assure alignment with the device (useful for ebeam
-            lithography).
-        outline_die (int or float): The width of the pads outline.
-        outline_dev (int or float): The width of the device's outline.
-        device_layer (int or array-like[2]): The layer where the device is placed.
-        die_layer (int or array-like[2]): The layer where the die is placed.
-        pad_layer (int or array-like[2]): The layer where the pads are placed.
-        text (string, optional): If None, the text is f"chk: {choke_w} \\nchnl: {channel_w}".
-        fill_pad_layer (bool): If True, the space reserved for pads in the
-            die_cell in filled in pad's layer.
-
-    Returns:
-        Device: A device containing the ntron, the border of the die (created with die_cell function),
-        and the connections between the ports.
-    """
-
-    ## Create the NTRON
-
-    # sizes the ntron parameters that were not given
-    if source_w is None and drain_w is None:
-        drain_w = source_w = 3 * channel_w
-    elif source_w is None:
-        source_w = drain_w
-    else:
-        drain_w = source_w
-    if gate_w is None:
-        gate_w = source_w
-    if choke_shift is None:
-        choke_shift = -3 * channel_w
-
-    NTRON = device.ntron.smooth(
-        choke_w, gate_w, channel_w, source_w, drain_w, choke_shift, device_layer
-    )
-    NTRON = utility.rename_ports_to_compass(NTRON)
-    if text is None:
-        text = f"chk: {choke_w} \nchnl: {channel_w}"
-    cell_text = text.replace(" \n", ", ")
-    DIE_NTRON = Device(f"CELL.NTRON({cell_text})")
-
-    DEVICE = Device(f"NTRON({cell_text})")
-    DEVICE << NTRON
-
-    ## Create the DIE
-
-    # die parameters, checkup conditions
-    die_contact_w = NTRON.ports["N1"].width + overlap_w
-    routes_margin = 2 * die_contact_w
-    dev_min_w = (
-        die_contact_w + 3 * outline_die
-    )  # condition imposed by the die parameters (contacts width)
-    device_max_w = max(2 * routes_margin + max(NTRON.size), dev_min_w)
-
-    # the die with calculated parameters
-    BORDER = utility.die_cell(
-        die_size=(die_w, die_w),
-        device_max_size=(device_max_w, device_max_w),
-        pad_size=pad_size,
-        contact_w=die_contact_w,
-        contact_l=overlap_w,
-        ports={"N": 1, "W": 1, "S": 1},
-        ports_gnd=["S"],
-        text=f"NTRON \n{text}",
-        isolation=outline_die,
-        layer=die_layer,
-        pad_layer=pad_layer,
-        invert=True,
-        fill_pad_layer=fill_pad_layer,
-    )
-
-    # place the ntron
-    NTRON.movex(NTRON.ports["N1"].midpoint[0], BORDER.ports["N1"].midpoint[0])
-
-    # Route DIE and NTRON
-
-    # hyper tapers
-    dev_contact_w = NTRON.ports["N1"].width
-    HT, device_ports = utility.add_hyptap_to_cell(
-        BORDER.get_ports(), overlap_w, dev_contact_w, device_layer
-    )
-    DEVICE << HT
-    DEVICE.ports = device_ports.ports
-    # routes
-    ROUTES = utility.route_to_dev(HT.get_ports(), NTRON.ports, device_layer)
-    DEVICE << ROUTES
-
-    DEVICE = pg.outline(DEVICE, outline_dev, precision=0.000001, open_ports=outline_dev)
-    DEVICE = pg.union(DEVICE, layer=device_layer)
-    DEVICE.name = f"NTRON({cell_text})"
-
-    DIE_NTRON << DEVICE
-    DIE_NTRON << BORDER
-
-    return DIE_NTRON
-
-
-def snspd(
-    die_w: Union[int, float] = dflt.die_w,
-    pad_size: Tuple[float] = dflt.pad_size,
-    snspd_width: float = 0.2,
-    snspd_pitch: float = 0.6,
-    snspd_size: Tuple[Union[int, float], Union[int, float]] = tuple(
-        x / 2 for x in utility.calculate_available_space_for_dev()
-    ),
-    snspd_num_squares: Optional[int] = None,
-    overlap_w: Union[int, float] = dflt.ebeam_overlap,
-    outline_die: Union[int, float] = dflt.die_outline,
-    outline_dev: Union[int, float] = dflt.device_outline,
-    device_layer: int = dflt.layers["device"],
-    die_layer: int = dflt.layers["die"],
-    pad_layer: int = dflt.layers["pad"],
-    text: Union[None, str] = dflt.text,
-    fill_pad_layer: bool = False,
-) -> Device:
-    """Creates a cell that contains a vertical superconducting nanowire single-
-    photon detector (SNSPD).
-
-    Parameters:
-        die_w (int or float): Width of a unit die/cell in the design (the output
-        device will be an integer number of unit cells).
-        pad_size (tuple of int or float): Dimensions of the die's pads (width,
-            height).
-        snspd_width (float): Width of the nanowire.
-        snspd_pitch (float): Pitch of the nanowire.
-        snspd_size (tuple of int or float): Size of the detector in squares (width, height).
-        snspd_num_squares (Optional[int]): Number of squares in the detector.
-        overlap_w (int or float): Extra length of the routes above the die's
-            ports to assure alignment with the device (useful for ebeam
-            lithography).
-        outline_die (int or float): The width of the pads outline.
-        outline_dev (int or float): The width of the device's outline.
-        device_layer (int or array-like[2]): The layer where the device is placed.
-        die_layer (int or array-like[2]): The layer where the die is placed.
-        pad_layer (int or array-like[2]): The layer where the pads are placed.
-        text (string, optional): If None, the text is f"w={snspd_width}".
-        fill_pad_layer (bool): If True, the space reserved for pads in the
-            die_cell in filled in pad's layer.
-
-    Returns:
-        Device: A cell (of size n*m unit die_cells) containing the SNSPD.
-    """
-    if text is None:
-        text = f"w={snspd_width}"
-    cell_text = text.replace(" \n", ", ")
-
-    SNSPD_CELL = Device(f"CELL.SNSPD({cell_text})")
-    DEVICE = Device(f"SNSPD({cell_text})")
-
-    # create SNSPD, make its ports compass, add safe optimal step
-    SNSPD = device.snspd.vertical(
-        wire_width=snspd_width,
-        wire_pitch=snspd_pitch,
-        size=snspd_size,
-        num_squares=snspd_num_squares,
-        layer=device_layer,
-    )
-    SNSPD = utility.rename_ports_to_compass(SNSPD)
-    SNSPD = utility.add_optimalstep_to_dev(SNSPD, ratio=10)
-    DEVICE << SNSPD
-
-    # create die
-    die_contact_w = utility.calculate_contact_w(
-        circuit_ports=SNSPD.get_ports(), overlap_w=overlap_w
-    )
-    device_max_size = tuple(
-        x + 2 * overlap_w for x in SNSPD.size
-    )  # not valide anymore if pads are not aligned with dev ports
-    n, m = utility.find_num_diecells_for_dev(
-        device_max_size, (die_w, die_w), pad_size, overlap_w, outline_die
-    )
-    BORDER = utility.die_cell(
-        die_size=(n * die_w, m * die_w),
-        device_max_size=device_max_size,
-        pad_size=pad_size,
-        contact_w=die_contact_w,
-        contact_l=overlap_w,
-        ports={"N": 1, "S": 1},
-        ports_gnd=["S"],
-        text=f"SNSPD \n{text}",
-        isolation=outline_die,
-        layer=die_layer,
-        pad_layer=pad_layer,
-        invert=True,
-        fill_pad_layer=fill_pad_layer,
-    )
-
-    # add hyper tapers at die pads
-    dev_contact_w = SNSPD.ports["N1"].width
-    HT, dev_ports = utility.add_hyptap_to_cell(
-        BORDER.get_ports(), overlap_w, dev_contact_w, device_layer
-    )
-    DEVICE.ports = dev_ports.ports
-    DEVICE << HT
-
-    # link hyper tapers to the device
-    ROUTES = utility.route_to_dev(
-        HT.get_ports(), SNSPD.ports
-    )  # absolutly no need to route, but will be useful when ports are no longer aligned with pads
-    DEVICE << ROUTES
-
-    DEVICE = pg.outline(
-        DEVICE, outline_dev, open_ports=2 * outline_dev, layer=device_layer
-    )
-    DEVICE.name = f"SNSPD({cell_text})"
-
-    SNSPD_CELL << DEVICE
-    SNSPD_CELL << BORDER
-    return SNSPD_CELL
-
-
-def snspd_ntron(
-    die_w: Union[int, float] = dflt.die_w,
-    pad_size: Tuple[float, float] = dflt.pad_size,
-    w_choke: Union[int, float] = 0.1,
-    w_snspd: Union[int, float] = dflt.auto_param,
-    overlap_w: Union[int, float] = dflt.ebeam_overlap,
-    outline_die: Union[int, float] = dflt.die_outline,
-    outline_dev: Union[int, float] = dflt.device_outline,
-    device_layer: int = dflt.layers["device"],
-    die_layer: int = dflt.layers["die"],
-    pad_layer: int = dflt.layers["pad"],
-    text: Union[None, str] = dflt.text,
-    fill_pad_layer: bool = False,
-) -> Device:
-    """Creates a cell that contains an SNSPD coupled to an NTRON. The device's
-    parameters are sized according to the SNSPD's width and the NTRON's choke.
-
-    Parameters:
-        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
-        pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
-        w_choke (int or float): The width of the NTRON choke in µm.
-        w_snspd (int or float, optional): The width of the SNSPD nanowire in µm (if None, scaled to 5 * w_choke).
-        overlap_w (int or float): Extra length of the routes above the die's ports to assure alignment with the device
-                                             (useful for ebeam lithography).
-        outline_die (int or float): The width of the pads outline.
-        outline_dev (int or float): The width of the device's outline.
-        device_layer (int or array-like[2]): The layer where the device is placed.
-        die_layer (int or array-like[2]): The layer where the die is placed.
-        pad_layer (int or array-like[2]): The layer where the pads are placed.
-        text (string, optional): If None, the text is f"w={w_snspd}, {w_choke}".
-        fill_pad_layer (bool): If True, the space reserved for pads in the
-            die_cell in filled in pad's layer.
-
-    Returns:
-        Device: A cell containing a die in die_layer, pads in pad layer,
-        and an SNSPD-NTRON properly routed in the device layer.
-    """
-
-    # Create SNSPD-NTRON
-    if w_snspd is None:
-        w_snspd = 5 * w_choke
-
-    if text is None:
-        text = f"w={w_snspd}, {w_choke}"
-    cell_text = text.replace(" \n", ", ")
-
-    DIE_SNSPD_NTRON = Device(f"CELL.SNSPD-NTRON({cell_text})")
-    DEVICE = Device(f"SNSPD-NTRON({cell_text})")
-
-    SNSPD_NTRON = circuit.snspd_ntron(
-        w_snspd=w_snspd,
-        pitch_snspd=3 * w_snspd,
-        size_snspd=(30 * w_snspd, 30 * w_snspd),
-        w_inductor=3 * w_snspd,
-        pitch_inductor=6 * w_snspd,
-        k_inductor13=20 * w_snspd,
-        k_inductor2=8 * w_snspd,
-        w_choke=w_choke,
-        w_channel=6 * w_choke,
-        w_pad=10 * w_snspd,
-        layer=device_layer,
-    )
-    DEVICE << SNSPD_NTRON
-
-    # Create DIE
-
-    die_contact_w = min(
-        10 * SNSPD_NTRON.ports["N1"].width + overlap_w, 0.5 * pad_size[0]
-    )
-
-    routes_margin = 2 * die_contact_w
-    margin = 2 * (pad_size[1] + outline_die + routes_margin)
-    n = max(2, math.ceil((SNSPD_NTRON.xsize + margin) / die_w))
-    m = max(1, math.ceil((SNSPD_NTRON.ysize + margin) / die_w))
-
-    dev_min_size = [
-        (die_contact_w + 3 * outline_die) * x for x in (5, 3)
-    ]  # condition imposed by the die parameters (contacts width)
-    device_max_size = (
-        max(
-            min(n * die_w - margin, 8 * routes_margin + SNSPD_NTRON.size[0]),
-            dev_min_size[0],
-        ),
-        max(
-            min(m * die_w - margin, 2 * routes_margin + SNSPD_NTRON.size[1]),
-            dev_min_size[1],
-        ),
-    )
-
-    BORDER = utility.die_cell(
-        die_size=(n * die_w, m * die_w),
-        device_max_size=device_max_size,
-        pad_size=pad_size,
-        contact_w=die_contact_w,
-        contact_l=overlap_w,
-        ports={"N": 3, "E": 1, "W": 1, "S": 2},
-        ports_gnd=["S"],
-        text=f"SNSPD-NTRON\n{text}",
-        isolation=outline_die,
-        layer=die_layer,
-        pad_layer=pad_layer,
-        invert=True,
-        fill_pad_layer=fill_pad_layer,
-    )
-
-    # Route DIE and SNSPD-NTRON
-
-    # hyper tapers
-    dev_contact_w = min(4 * SNSPD_NTRON.ports["N1"].width, 0.8 * die_contact_w)
-    HT, device_ports = utility.add_hyptap_to_cell(
-        BORDER.get_ports(), overlap_w, dev_contact_w, device_layer
-    )
-    DEVICE << HT
-    DEVICE.ports = device_ports.ports
-
-    # routes
-    ROUTES = utility.route_to_dev(HT.get_ports(), SNSPD_NTRON.ports, device_layer)
-    DEVICE << ROUTES
-
-    DEVICE = pg.outline(DEVICE, outline_dev, precision=0.000001, open_ports=outline_dev)
-    DEVICE = pg.union(DEVICE, layer=device_layer)
-    DEVICE.name = f"SNSPD-NTRON({cell_text})"
-
-    DIE_SNSPD_NTRON << DEVICE
-    DIE_SNSPD_NTRON << BORDER
-
-    return DIE_SNSPD_NTRON
+"""Library of pre-built cells containing text, border marks, and an experiment,
+connected to pads for wirebonding."""
+
+from phidl import Device
+import phidl.geometry as pg
+import phidl.routing as pr
+from typing import Tuple, List, Union, Optional
+import math
+
+import qnngds.tests as test
+import qnngds.devices as device
+import qnngds.circuits as circuit
+import qnngds.utilities as utility
+import qnngds._default_param as dflt
+
+# basics
+
+
+def alignment(
+    die_w: Union[int, float] = dflt.die_w,
+    layers_to_align: List[int] = [dflt.layers["die"], dflt.layers["pad"]],
+    outline_die: Union[int, float] = dflt.die_outline,
+    die_layer: int = dflt.layers["die"],
+    text: Union[None, str] = dflt.text,
+) -> Device:
+    """Creates alignment marks in an integer number of unit cells.
+
+    Parameters:
+        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
+        layers_to_align (list of int): Layers to align.
+        outline_die (int or float): The width of the die's outline.
+        die_layer (int): The layer where the die is placed.
+        text (str, optional): If None, the text is f"lay={layers_to_align}".
+
+    Returns:
+        DIE_ALIGN (Device): A device that centers the alignment marks in an n*m unit cell.
+    """
+
+    if text is None:
+        text = f"lay={layers_to_align}"
+    DIE = Device(f"CELL.ALIGN({text})")
+
+    ALIGN = test.alignment_mark(layers_to_align)
+
+    n = math.ceil((ALIGN.xsize) / die_w)
+    m = math.ceil((ALIGN.ysize) / die_w)
+
+    BORDER = utility.die_cell(
+        die_size=(n * die_w, m * die_w),
+        device_max_size=(ALIGN.xsize + 20, ALIGN.ysize + 20),
+        ports={},
+        ports_gnd={},
+        isolation=outline_die,
+        text=f"ALIGN {text}",
+        layer=die_layer,
+        invert=True,
+    )
+
+    DIE << BORDER.flatten()
+    DIE << ALIGN
+
+    return DIE
+
+
+def vdp(
+    die_w: Union[int, float] = dflt.die_w,
+    pad_size: Tuple[float] = dflt.pad_size,
+    layers_to_probe: List[int] = [dflt.layers["die"]],
+    layers_to_outline: Union[None, List[int]] = dflt.auto_param,
+    outline: Union[int, float] = dflt.die_outline,
+    die_layer: Union[int, float] = dflt.layers["die"],
+    pad_layer: int = dflt.layers["pad"],
+    text: Union[None, str] = dflt.text,
+) -> Device:
+    r"""Creates a cell containing a Van Der Pauw structure between 4 contact
+    pads.
+
+    Parameters:
+        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
+        pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
+        layers_to_probe (list of int): The layers on which to place the VDP structure.
+        layers_to_outline (list of int): Among the VDP layers, the ones for which structure must not be filled but outlined.
+        outline (int or float): The width of the VDP and die's outline.
+        die_layer (int or tuple of int): The layer where the die is placed.
+        pad_layer (int or tuple of int): The layer where the pads are placed.
+        text (str, optional): If None, the text is f"lay={layers_to_probe}".
+    Returns:
+        DIE_VANDP (Device): The created device.
+    """
+    # Initialize parameters left to default (=None)
+
+    if text is None:
+        text = f"lay={layers_to_probe}"
+    if layers_to_outline is None:
+        layers_to_outline = [die_layer]  # default layer to outline if None is given
+
+    DIE_VANDP = Device(f"CELL.VDP({text})")
+
+    device_max_w = die_w - 2 * (
+        pad_size[1] + 2 * outline
+    )  # width of max device size for this cell
+    contact_w = device_max_w / 10  # choosing a contact width 10 times smaller
+    device_w = (
+        device_max_w - 2 * contact_w
+    )  # choosing a smaller device to have space for routing from pad to contact
+
+    # Creates the DIE, it contains only the cell text and bordure
+
+    DIE = utility.die_cell(
+        die_size=(die_w, die_w),
+        device_max_size=(device_max_w, device_max_w),
+        ports={},
+        ports_gnd=[],
+        isolation=outline,
+        text=f"VDP \n{text}",
+        layer=die_layer,
+        pad_layer=pad_layer,
+        invert=True,
+        fill_pad_layer=False,
+    )
+    DIE_VANDP << DIE.flatten()
+
+    # Creates the vdp structure, add pads and route
+
+    VDP = Device()
+
+    ## VDP probed area
+    AREA = test.vdp(device_w, contact_w)
+    VDP << AREA
+
+    ## pads
+    PADS = utility.die_cell(
+        die_size=(die_w, die_w),
+        device_max_size=(device_max_w, device_max_w),
+        pad_size=pad_size,
+        contact_w=pad_size[0],
+        contact_l=0,
+        ports={"N": 1, "E": 1, "W": 1, "S": 1},
+        ports_gnd=["N", "E", "W", "S"],
+        isolation=outline,
+        text="PADS ONLY",
+        layer=0,
+        pad_layer=pad_layer,
+        invert=False,
+        fill_pad_layer=False,
+    )
+    PADS.remove_layers([pad_layer], invert_selection=True)
+    VDP << PADS
+
+    ## routes from pads to probing area
+    ROUTES = utility.route_to_dev(PADS.get_ports(), AREA.ports)
+    VDP << ROUTES
+
+    VDP.flatten(0)
+
+    # Outline the vdp structure for layers that need to be outlined
+
+    DEVICE = Device(f"VDP(lay={layers_to_probe})")
+
+    for layer in layers_to_probe:
+        TEST_LAY = pg.deepcopy(VDP)
+        if layer in layers_to_outline:
+            TEST_LAY = pg.outline(TEST_LAY, outline)
+        TEST_LAY.name = f"VDP(lay={layer})"
+        DEVICE << TEST_LAY.flatten(single_layer=layer)
+
+    DIE_VANDP << DEVICE
+
+    # Add pads if they are not in already present
+    if pad_layer not in layers_to_probe:
+        PADS = pg.union(PADS, layer=pad_layer)
+        PADS.name = "PADS"
+        DIE_VANDP << PADS
+
+    return DIE_VANDP
+
+
+def etch_test(
+    die_w: Union[int, float] = dflt.die_w,
+    layers_to_etch: List[List[int]] = [[dflt.layers["pad"]]],
+    outline_die: Union[int, float] = dflt.die_outline,
+    die_layer: int = dflt.layers["die"],
+    text: Union[None, str] = dflt.text,
+) -> Device:
+    """Creates etch test structures in an integer number of unit cells.
+
+    These test structures are thought to be used by probing on pads (with a
+    simple multimeter) that should be isolated one from another if the etching
+    is complete.
+
+    Parameters:
+        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
+        layers_to_etch (list of list of int): Each element of the list corresponds to one test point, to put on the list of layers specified.
+                                               Example: [[1, 2], [1], [2]]
+        outline_die (int or float): The width of the die's outline.
+        die_layer (int): The layer where the die is placed.
+        text (str, optional): If None, the text is f"lay={layers_to_etch}".
+
+    Returns:
+        DIE_ETCH_TEST (Device): A device (with size n*m of unit cells) with etch tests in its center.
+    """
+
+    if text is None:
+        text = f"lay={layers_to_etch}"
+    DIE_ETCH_TEST = Device(f"CELL.ETCH_TEST({text})")
+
+    TEST = Device(f"ETCH_TEST({text})")
+
+    ## Create the probing areas
+
+    margin = 0.12 * die_w
+    rect = pg.rectangle((die_w - 2 * margin, die_w - 2 * margin))
+    for i, layer_to_etch in enumerate(layers_to_etch):
+        probe = Device()
+        probe.add_array(rect, 2, 1, (die_w, die_w))
+        for layer in layer_to_etch:
+            TEST << pg.outline(probe, -outline_die, layer=layer).movey(i * die_w)
+
+    ## Create the die
+
+    n = math.ceil((TEST.xsize + 2 * dflt.die_cell_border) / die_w)
+    m = math.ceil((TEST.ysize + 2 * dflt.die_cell_border) / die_w)
+    BORDER = utility.die_cell(
+        die_size=(n * die_w, m * die_w),
+        ports={},
+        ports_gnd={},
+        text=f"ETCH TEST {text}",
+        isolation=outline_die,
+        layer=die_layer,
+        invert=True,
+    )
+
+    BORDER.move(TEST.center)
+    DIE_ETCH_TEST << BORDER.flatten()
+    DIE_ETCH_TEST << TEST.flatten()
+    DIE_ETCH_TEST.move(DIE_ETCH_TEST.center, (0, 0))
+
+    return DIE_ETCH_TEST
+
+
+def resolution_test(
+    die_w: Union[int, float] = dflt.die_w,
+    layer_to_resolve: int = dflt.layers["device"],
+    resolutions_to_test: List[float] = [
+        0.025,
+        0.05,
+        0.075,
+        0.1,
+        0.25,
+        0.5,
+        1,
+        1.5,
+        2.0,
+    ],
+    outline: Union[int, float] = dflt.die_outline,
+    die_layer: int = dflt.layers["die"],
+    text: Union[None, str] = dflt.text,
+) -> Device:
+    r"""Creates a cell containing a resolution test.
+
+    Parameters:
+        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
+        layer_to_resolve (int): The layer to put the resolution test on.
+        resolutions_to_test (list of float): The resolutions to test in µm.
+        outline (int or float): The width of the VDP and die's outline.
+        die_layer (int or tuple of int): The layer where the die is placed.
+        text (str, optional): If None, the text is f"lay={layer_to_resolve}".
+
+    Returns:
+        DIE_RES_TEST (Device): The created device.
+    """
+
+    if text is None:
+        text = f"lay={layer_to_resolve}"
+    DIE_RES_TEST = Device(f"CELL.RESOLUTION_TEST({text})")
+
+    ## Create the test structure
+    TEST_RES = Device(f"RESOLUTION_TEST({text})")
+    test_res = TEST_RES << test.resolution_test(
+        resolutions=resolutions_to_test, inverted=False, layer=layer_to_resolve
+    )
+    test_res_invert = TEST_RES << test.resolution_test(
+        resolutions=resolutions_to_test,
+        inverted=resolutions_to_test[-1],
+        layer=layer_to_resolve,
+    )
+    test_res_invert.movey(
+        test_res_invert.ymin, test_res.ymax + 5 * resolutions_to_test[-1]
+    )
+
+    DIE_RES_TEST << TEST_RES.move(TEST_RES.center, (0, 0))
+
+    ## Create the die
+    n = math.ceil((TEST_RES.xsize) / die_w)
+    m = math.ceil((TEST_RES.ysize) / die_w)
+    BORDER = utility.die_cell(
+        die_size=(n * die_w, m * die_w),
+        ports={},
+        ports_gnd=[],
+        text=f"RES TEST \n{text}",
+        isolation=outline,
+        layer=die_layer,
+        invert=True,
+    )
+
+    DIE_RES_TEST << BORDER.flatten()
+    return DIE_RES_TEST
+
+
+## devices:
+
+
+def nanowires(
+    die_w: Union[int, float] = dflt.die_w,
+    pad_size: Tuple[float] = dflt.pad_size,
+    channels_sources_w: List[Tuple[float, float]] = [(0.1, 1), (0.5, 3), (1, 10)],
+    overlap_w: Union[int, float] = dflt.ebeam_overlap,
+    outline_die: Union[int, float] = dflt.die_outline,
+    outline_dev: Union[int, float] = dflt.device_outline,
+    device_layer: int = dflt.layers["device"],
+    die_layer: int = dflt.layers["die"],
+    pad_layer: int = dflt.layers["pad"],
+    text: Union[None, str] = dflt.text,
+    fill_pad_layer: bool = False,
+) -> Device:
+    """Creates a cell that contains several nanowires of given channel and
+    source.
+
+    Parameters:
+        die_w (int or float): Width of a unit die/cell in the design (the output
+            device will be an integer number of unit cells).
+        pad_size (tuple of int or float): Dimensions of the die's pads (width,
+            height).
+        channels_sources_w (list of tuple of float): The list of (channel_w,
+            source_w) of the nanowires to create.
+        overlap_w (int or float): Extra length of the routes above the die's
+            ports to assure alignment with the device (useful for ebeam
+            lithography).
+        outline_die (int or float): The width of the pads outline.
+        outline_dev (int or float): The width of the device's outline.
+        device_layer (int or tuple of int): The layer where the device is placed.
+        die_layer (int or tuple of int): The layer where the die is placed.
+        pad_layer (int or tuple of int): The layer where the pads are placed.
+        text (str, optional): If None, the text is f"w={channels_w}".
+        fill_pad_layer (bool): If True, the space reserved for pads in the
+            die_cell in filled in pad's layer.
+
+    Returns:
+        Device: A device (of size n*m unit cells) containing the nanowires, the
+        border of the die (created with die_cell function), and the connections
+        between the nanowires and pads.
+    """
+
+    if text is None:
+        channels_w = [item[0] for item in channels_sources_w]
+        text = f"w={channels_w}"
+    cell_text = text.replace(" \n", ", ")
+
+    NANOWIRES_DIE = Device(f"CELL.NWIRES({cell_text})")
+
+    DEVICE = Device(f"NWIRES({cell_text})")
+
+    ## Create the NANOWIRES
+
+    NANOWIRES = Device(f"NWIRES({cell_text})")
+    nanowires_ref = []
+    for i, channel_source_w in enumerate(channels_sources_w):
+        nanowire_ref = NANOWIRES << device.nanowire.spot(
+            channel_source_w[0], channel_source_w[1]
+        )
+        nanowires_ref.append(nanowire_ref)
+    DEVICE << NANOWIRES
+
+    ## Create the DIE
+
+    # die parameters, checkup conditions
+    n = len(channels_sources_w)
+    die_size = (math.ceil((2 * (n + 1) * pad_size[0]) / die_w) * die_w, die_w)
+    die_contact_w = NANOWIRES.xsize + overlap_w
+    dev_contact_w = NANOWIRES.xsize
+    routes_margin = 4 * die_contact_w
+    dev_max_size = (2 * n * pad_size[0], NANOWIRES.ysize + routes_margin)
+
+    # die, with calculated parameters
+    BORDER = utility.die_cell(
+        die_size=die_size,
+        device_max_size=dev_max_size,
+        pad_size=pad_size,
+        contact_w=die_contact_w,
+        contact_l=overlap_w,
+        ports={"N": n, "S": n},
+        ports_gnd=["S"],
+        isolation=outline_die,
+        text=f"NWIRES\n{text}",
+        layer=die_layer,
+        pad_layer=pad_layer,
+        invert=True,
+        fill_pad_layer=fill_pad_layer,
+    )
+
+    ## Place the nanowires
+
+    for i, nanowire_ref in enumerate(nanowires_ref):
+        nanowire_ref.movex(BORDER.ports[f"N{i+1}"].x)
+        NANOWIRES.add_port(port=nanowire_ref.ports[1], name=f"N{i+1}")
+        NANOWIRES.add_port(port=nanowire_ref.ports[2], name=f"S{i+1}")
+
+    ## Route the nanowires and the die
+
+    # hyper tapers
+    HT, dev_ports = utility.add_hyptap_to_cell(
+        BORDER.get_ports(), overlap_w, dev_contact_w
+    )
+    DEVICE.ports = dev_ports.ports
+    DEVICE << HT
+
+    # routes from nanowires to hyper tapers
+    ROUTES = utility.route_to_dev(HT.get_ports(), NANOWIRES.ports)
+    DEVICE << ROUTES
+
+    DEVICE.ports = dev_ports.ports
+    DEVICE = pg.outline(
+        DEVICE, outline_dev, open_ports=2 * outline_dev, layer=device_layer
+    )
+    DEVICE.name = f"NWIRES({cell_text})"
+
+    NANOWIRES_DIE << DEVICE
+    NANOWIRES_DIE << BORDER
+
+    return NANOWIRES_DIE
+
+
+def ntron(
+    die_w: Union[int, float] = dflt.die_w,
+    pad_size: Tuple[float, float] = dflt.pad_size,
+    choke_w: Union[int, float] = 0.1,
+    channel_w: Union[int, float] = 0.5,
+    gate_w: Union[None, int, float] = dflt.auto_param,
+    source_w: Union[None, int, float] = dflt.auto_param,
+    drain_w: Union[None, int, float] = dflt.auto_param,
+    choke_shift: Union[None, int, float] = dflt.auto_param,
+    overlap_w: Union[None, int, float] = dflt.ebeam_overlap,
+    outline_die: Union[None, int, float] = dflt.die_outline,
+    outline_dev: Union[None, int, float] = dflt.device_outline,
+    device_layer: int = dflt.layers["device"],
+    die_layer: int = dflt.layers["die"],
+    pad_layer: int = dflt.layers["pad"],
+    text: Union[None, str] = dflt.text,
+    fill_pad_layer: bool = False,
+) -> Device:
+    r"""Creates a standardized cell specifically for a single ntron.
+
+    Unless specified, scales the ntron parameters as:
+    gate_w = drain_w = source_w = 3 * channel_w
+    choke_shift = -3 * channel_w
+
+    Parameters:
+        die_w (int or float): Width of a unit die/cell in the design (the output
+            device will be an integer number of unit cells).
+        pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
+        choke_w (int or float): The width of the ntron's choke in µm.
+        channel_w (int or float): The width of the ntron's channel in µm.
+        gate_w (int or float, optional): If None, gate width is 3 times the channel width.
+        source_w (int or float, optional): If None, source width is 3 times the channel width.
+        drain_w (int or float, optional): If None, drain width is 3 times the channel width.
+        choke_shift (int or float, optional): If None, choke shift is -3 times the channel width.
+        overlap_w (int or float): Extra length of the routes above the die's
+            ports to assure alignment with the device (useful for ebeam
+            lithography).
+        outline_die (int or float): The width of the pads outline.
+        outline_dev (int or float): The width of the device's outline.
+        device_layer (int or array-like[2]): The layer where the device is placed.
+        die_layer (int or array-like[2]): The layer where the die is placed.
+        pad_layer (int or array-like[2]): The layer where the pads are placed.
+        text (string, optional): If None, the text is f"chk: {choke_w} \\nchnl: {channel_w}".
+        fill_pad_layer (bool): If True, the space reserved for pads in the
+            die_cell in filled in pad's layer.
+
+    Returns:
+        Device: A device containing the ntron, the border of the die (created with die_cell function),
+        and the connections between the ports.
+    """
+
+    ## Create the NTRON
+
+    # sizes the ntron parameters that were not given
+    if source_w is None and drain_w is None:
+        drain_w = source_w = 3 * channel_w
+    elif source_w is None:
+        source_w = drain_w
+    else:
+        drain_w = source_w
+    if gate_w is None:
+        gate_w = source_w
+    if choke_shift is None:
+        choke_shift = -3 * channel_w
+
+    NTRON = device.ntron.smooth(
+        choke_w, gate_w, channel_w, source_w, drain_w, choke_shift, device_layer
+    )
+    NTRON = utility.rename_ports_to_compass(NTRON)
+    if text is None:
+        text = f"chk: {choke_w} \nchnl: {channel_w}"
+    cell_text = text.replace(" \n", ", ")
+    DIE_NTRON = Device(f"CELL.NTRON({cell_text})")
+
+    DEVICE = Device(f"NTRON({cell_text})")
+    DEVICE << NTRON
+
+    ## Create the DIE
+
+    # die parameters, checkup conditions
+    die_contact_w = NTRON.ports["N1"].width + overlap_w
+    routes_margin = 2 * die_contact_w
+    dev_min_w = (
+        die_contact_w + 3 * outline_die
+    )  # condition imposed by the die parameters (contacts width)
+    device_max_w = max(2 * routes_margin + max(NTRON.size), dev_min_w)
+
+    # the die with calculated parameters
+    BORDER = utility.die_cell(
+        die_size=(die_w, die_w),
+        device_max_size=(device_max_w, device_max_w),
+        pad_size=pad_size,
+        contact_w=die_contact_w,
+        contact_l=overlap_w,
+        ports={"N": 1, "W": 1, "S": 1},
+        ports_gnd=["S"],
+        text=f"NTRON \n{text}",
+        isolation=outline_die,
+        layer=die_layer,
+        pad_layer=pad_layer,
+        invert=True,
+        fill_pad_layer=fill_pad_layer,
+    )
+
+    # place the ntron
+    NTRON.movex(NTRON.ports["N1"].midpoint[0], BORDER.ports["N1"].midpoint[0])
+
+    # Route DIE and NTRON
+
+    # hyper tapers
+    dev_contact_w = NTRON.ports["N1"].width
+    HT, device_ports = utility.add_hyptap_to_cell(
+        BORDER.get_ports(), overlap_w, dev_contact_w, device_layer
+    )
+    DEVICE << HT
+    DEVICE.ports = device_ports.ports
+    # routes
+    ROUTES = utility.route_to_dev(HT.get_ports(), NTRON.ports, device_layer)
+    DEVICE << ROUTES
+
+    DEVICE = pg.outline(DEVICE, outline_dev, precision=0.000001, open_ports=outline_dev)
+    DEVICE = pg.union(DEVICE, layer=device_layer)
+    DEVICE.name = f"NTRON({cell_text})"
+
+    DIE_NTRON << DEVICE
+    DIE_NTRON << BORDER
+
+    return DIE_NTRON
+
+
+def snspds(
+    die_w: Union[int, float] = dflt.die_w,
+    pad_size: Tuple[float] = dflt.pad_size,
+    snspds_width_pitch: List[Tuple[float, float]] = [
+        (0.1, 0.3),
+        (0.2, 0.6),
+        (0.3, 0.9),
+    ],
+    snspd_size: Tuple[Union[int, float], Union[int, float]] = tuple(
+        round(x / 3) for x in utility.calculate_available_space_for_dev()
+    ),
+    snspd_num_squares: Optional[int] = None,
+    overlap_w: Union[int, float] = dflt.ebeam_overlap,
+    outline_die: Union[int, float] = dflt.die_outline,
+    outline_dev: Union[int, float] = dflt.device_outline,
+    device_layer: int = dflt.layers["device"],
+    die_layer: int = dflt.layers["die"],
+    pad_layer: int = dflt.layers["pad"],
+    text: Union[None, str] = dflt.text,
+    fill_pad_layer: bool = False,
+) -> Device:
+    """Creates a cell that contains vertical superconducting nanowire single-
+    photon detectors (SNSPD).
+
+    Parameters:
+        die_w (int or float): Width of a unit die/cell in the design (the output
+            device will be an integer number of unit cells).
+        pad_size (tuple of int or float): Dimensions of the die's pads (width,
+            height).
+        snspds_width_pitch (list of tuple of float): list of (width, pitch) of
+            the nanowires. For creating n SNSPD, the list of snspds_width_pitch
+            should have a size of n.
+        snspd_size (tuple of int or float): Size of the detectors in squares (width, height).
+        snspd_num_squares (Optional[int]): Number of squares in the detectors.
+        overlap_w (int or float): Extra length of the routes above the die's
+            ports to assure alignment with the device (useful for ebeam
+            lithography).
+        outline_die (int or float): The width of the pads outline.
+        outline_dev (int or float): The width of the device's outline.
+        device_layer (int or array-like[2]): The layer where the device is placed.
+        die_layer (int or array-like[2]): The layer where the die is placed.
+        pad_layer (int or array-like[2]): The layer where the pads are placed.
+        text (string, optional): If None, the text is f"w={snspds_width}".
+        fill_pad_layer (bool): If True, the space reserved for pads in the
+            die_cell in filled in pad's layer.
+
+    Returns:
+        Device: A cell (of size n*m unit die_cells) containing the SNSPDs.
+    """
+    if text is None:
+        snspds_width = [item[0] for item in snspds_width_pitch]
+        text = f"w={snspds_width}"
+    cell_text = text.replace(" \n", ", ")
+
+    SNSPD_CELL = Device(f"CELL.SNSPD({cell_text})")
+    DEVICE = Device(f"SNSPD({cell_text})")
+
+    # create SNSPD, make its ports compass, add safe optimal step
+    snspds_ref = []
+    for i, snspd_width_pitch in enumerate(snspds_width_pitch):
+        SNSPD = device.snspd.vertical(
+            wire_width=snspd_width_pitch[0],
+            wire_pitch=snspd_width_pitch[1],
+            size=snspd_size,
+            num_squares=snspd_num_squares,
+            layer=device_layer,
+        )
+        SNSPD = utility.rename_ports_to_compass(SNSPD)
+        SNSPD = utility.add_optimalstep_to_dev(SNSPD, ratio=10)
+        snspd_ref = DEVICE << SNSPD
+        snspds_ref.append(snspd_ref)
+
+    # create die
+    num_snspds = len(snspds_width_pitch)
+    die_contact_w = utility.calculate_contact_w(
+        circuit_ports=DEVICE.get_ports(depth=1), overlap_w=overlap_w
+    )
+    device_max_y = DEVICE.ysize + 2 * overlap_w
+    device_max_x = num_snspds * max(pad_size[0] * 1.5, DEVICE.xsize + 2 * outline_die)
+    device_max_size = (device_max_x, device_max_y)
+
+    n, m = utility.find_num_diecells_for_dev(
+        device_max_size,
+        {"N": num_snspds, "S": num_snspds},
+        (die_w, die_w),
+        pad_size,
+        overlap_w,
+        outline_die,
+    )
+
+    BORDER = utility.die_cell(
+        die_size=(n * die_w, m * die_w),
+        device_max_size=device_max_size,
+        pad_size=pad_size,
+        contact_w=die_contact_w,
+        contact_l=overlap_w,
+        ports={"N": len(snspds_width_pitch), "S": len(snspds_width_pitch)},
+        ports_gnd=["S"],
+        text=f"SNSPD \n{text}",
+        isolation=outline_die,
+        layer=die_layer,
+        pad_layer=pad_layer,
+        invert=True,
+        fill_pad_layer=fill_pad_layer,
+    )
+
+    # align SNSPDs to the die's ports
+    for i, ref in enumerate(snspds_ref):
+        ref.movex(0, BORDER.ports[f"N{i+1}"].x)
+    DEVICE = utility.rename_ports_to_compass(DEVICE, depth=1)
+    snspds_ports = DEVICE.ports
+
+    # add hyper tapers at die pads
+    dev_contact_w = max([port.width for port in DEVICE.get_ports()])
+    HT, dev_ports = utility.add_hyptap_to_cell(
+        BORDER.get_ports(), overlap_w, dev_contact_w, device_layer
+    )
+    DEVICE.ports = dev_ports.ports
+    DEVICE << HT
+
+    # link hyper tapers to the device
+    ROUTES = utility.route_to_dev(HT.get_ports(), snspds_ports)
+    DEVICE << ROUTES
+
+    DEVICE = pg.outline(
+        DEVICE, outline_dev, open_ports=2 * outline_dev, layer=device_layer
+    )
+    DEVICE.name = f"SNSPD({cell_text})"
+
+    SNSPD_CELL << DEVICE
+    SNSPD_CELL << BORDER
+    return SNSPD_CELL
+
+
+def snspd_ntron(
+    die_w: Union[int, float] = dflt.die_w,
+    pad_size: Tuple[float, float] = dflt.pad_size,
+    w_choke: Union[int, float] = 0.1,
+    w_snspd: Union[int, float] = dflt.auto_param,
+    overlap_w: Union[int, float] = dflt.ebeam_overlap,
+    outline_die: Union[int, float] = dflt.die_outline,
+    outline_dev: Union[int, float] = dflt.device_outline,
+    device_layer: int = dflt.layers["device"],
+    die_layer: int = dflt.layers["die"],
+    pad_layer: int = dflt.layers["pad"],
+    text: Union[None, str] = dflt.text,
+    fill_pad_layer: bool = False,
+) -> Device:
+    """Creates a cell that contains an SNSPD coupled to an NTRON. The device's
+    parameters are sized according to the SNSPD's width and the NTRON's choke.
+
+    Parameters:
+        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
+        pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
+        w_choke (int or float): The width of the NTRON choke in µm.
+        w_snspd (int or float, optional): The width of the SNSPD nanowire in µm (if None, scaled to 5 * w_choke).
+        overlap_w (int or float): Extra length of the routes above the die's ports to assure alignment with the device
+                                             (useful for ebeam lithography).
+        outline_die (int or float): The width of the pads outline.
+        outline_dev (int or float): The width of the device's outline.
+        device_layer (int or array-like[2]): The layer where the device is placed.
+        die_layer (int or array-like[2]): The layer where the die is placed.
+        pad_layer (int or array-like[2]): The layer where the pads are placed.
+        text (string, optional): If None, the text is f"w={w_snspd}, {w_choke}".
+        fill_pad_layer (bool): If True, the space reserved for pads in the
+            die_cell in filled in pad's layer.
+
+    Returns:
+        Device: A cell containing a die in die_layer, pads in pad layer,
+        and an SNSPD-NTRON properly routed in the device layer.
+    """
+
+    # Create SNSPD-NTRON
+    if w_snspd is None:
+        w_snspd = 5 * w_choke
+
+    if text is None:
+        text = f"w={w_snspd}, {w_choke}"
+    cell_text = text.replace(" \n", ", ")
+
+    DIE_SNSPD_NTRON = Device(f"CELL.SNSPD-NTRON({cell_text})")
+    DEVICE = Device(f"SNSPD-NTRON({cell_text})")
+
+    SNSPD_NTRON = circuit.snspd_ntron(
+        w_snspd=w_snspd,
+        pitch_snspd=3 * w_snspd,
+        size_snspd=(30 * w_snspd, 30 * w_snspd),
+        w_inductor=3 * w_snspd,
+        pitch_inductor=6 * w_snspd,
+        k_inductor13=20 * w_snspd,
+        k_inductor2=8 * w_snspd,
+        w_choke=w_choke,
+        w_channel=6 * w_choke,
+        w_pad=10 * w_snspd,
+        layer=device_layer,
+    )
+    DEVICE << SNSPD_NTRON
+
+    # Create DIE
+
+    die_contact_w = min(
+        10 * SNSPD_NTRON.ports["N1"].width + overlap_w, 0.5 * pad_size[0]
+    )
+
+    routes_margin = 2 * die_contact_w
+    margin = 2 * (pad_size[1] + outline_die + routes_margin)
+    n = max(2, math.ceil((SNSPD_NTRON.xsize + margin) / die_w))
+    m = max(1, math.ceil((SNSPD_NTRON.ysize + margin) / die_w))
+
+    dev_min_size = [
+        (die_contact_w + 3 * outline_die) * x for x in (5, 3)
+    ]  # condition imposed by the die parameters (contacts width)
+    device_max_size = (
+        max(
+            min(n * die_w - margin, 8 * routes_margin + SNSPD_NTRON.size[0]),
+            dev_min_size[0],
+        ),
+        max(
+            min(m * die_w - margin, 2 * routes_margin + SNSPD_NTRON.size[1]),
+            dev_min_size[1],
+        ),
+    )
+
+    BORDER = utility.die_cell(
+        die_size=(n * die_w, m * die_w),
+        device_max_size=device_max_size,
+        pad_size=pad_size,
+        contact_w=die_contact_w,
+        contact_l=overlap_w,
+        ports={"N": 3, "E": 1, "W": 1, "S": 2},
+        ports_gnd=["S"],
+        text=f"SNSPD-NTRON\n{text}",
+        isolation=outline_die,
+        layer=die_layer,
+        pad_layer=pad_layer,
+        invert=True,
+        fill_pad_layer=fill_pad_layer,
+    )
+
+    # Route DIE and SNSPD-NTRON
+
+    # hyper tapers
+    dev_contact_w = min(4 * SNSPD_NTRON.ports["N1"].width, 0.8 * die_contact_w)
+    HT, device_ports = utility.add_hyptap_to_cell(
+        BORDER.get_ports(), overlap_w, dev_contact_w, device_layer
+    )
+    DEVICE << HT
+    DEVICE.ports = device_ports.ports
+
+    # routes
+    ROUTES = utility.route_to_dev(HT.get_ports(), SNSPD_NTRON.ports, device_layer)
+    DEVICE << ROUTES
+
+    DEVICE = pg.outline(DEVICE, outline_dev, precision=0.000001, open_ports=outline_dev)
+    DEVICE = pg.union(DEVICE, layer=device_layer)
+    DEVICE.name = f"SNSPD-NTRON({cell_text})"
+
+    DIE_SNSPD_NTRON << DEVICE
+    DIE_SNSPD_NTRON << BORDER
+
+    return DIE_SNSPD_NTRON
```

### Comparing `qnngds-2.4.1/src/qnngds/circuits.py` & `qnngds-2.5.0/src/qnngds/circuits.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,285 +1,285 @@
-"""Circuits module contains a library of QNN's circuits (e.g. snspd coupled to
-ntron, logic gates etc.)"""
-
-from phidl import Device
-import phidl.geometry as pg
-from typing import Tuple, Union
-import math
-
-import qnngds.devices as device
-
-
-def snspd_ntron(
-    w_snspd: float = 0.1,
-    pitch_snspd: float = 0.3,
-    size_snspd: Tuple[Union[int, float]] = (3, 3),
-    w_inductor: float = 0.3,
-    pitch_inductor: float = 0.6,
-    k_inductor13: Union[int, float] = 10,
-    k_inductor2: Union[int, float] = 4,
-    w_choke: float = 0.02,
-    w_channel: float = 0.12,
-    w_pad: Union[int, float] = 1,
-    layer: int = 0,
-) -> Device:
-    """Creates a SNSPD coupled to an NTRON, with 3 inductors in the circuit as:
-
-    >>> |        |
-    >>> L1       L3
-    >>> |        |
-    >>> |__L2__NTRON
-    >>> |        |
-    >>> SNSPD
-    >>> |
-
-    The length of L1, L2, and L3 (long nanowires) where scaled against the SNSPD:
-    L1 = L3 = k13 * L and L2 = k2 * L where L is the SNSPD kinetic inductance.
-
-    Parameters:
-        w_snspd (float): Width of the SNSPD.
-        pitch_snspd (float): Pitch of the SNSPD.
-        size_snspd (Tuple[Union[int, float]]): Size of the SNSPD.
-        w_inductor (float): Width of the inductors.
-        pitch_inductor (float): Pitch of the inductors.
-        k_inductor13 (Union[int, float]): The factor for scaling L1 and L3 relative to the SNSPD kinetic inductance.
-        k_inductor2 (Union[int, float]): The factor for scaling L2 relative to the SNSPD kinetic inductance.
-        w_choke (float): Width of the choke in the NTRON.
-        w_channel (float): Width of the channel in the NTRON.
-        w_pad (Union[int, float]): Width of the external connections to the cell.
-        layer (int): Layer of the device.
-
-    Returns:
-        Device: The created device.
-    """
-
-    def scale_inductors_to_snspd():
-
-        l_snspd = size_snspd[0] * size_snspd[1] / pitch_snspd
-        l_inductor13 = k_inductor13 * w_inductor / w_snspd * l_snspd
-        l_inductor2 = k_inductor2 * w_inductor / w_snspd * l_snspd
-
-        n_inductor13 = math.sqrt(l_inductor13 * pitch_inductor)
-        n_inductor2 = math.sqrt(l_inductor2 * pitch_inductor)
-
-        size_inductor13 = (n_inductor13, n_inductor13)
-        size_inductor2 = (n_inductor2, n_inductor2)
-
-        return size_inductor13, size_inductor2
-
-    def crossA():
-
-        D = Device()
-        tee = pg.tee(
-            (3 * w_inductor, w_inductor), (w_inductor, w_inductor), taper_type="fillet"
-        )
-        first_tee = D << tee.movey(-w_inductor / 2)
-        second_tee = D << tee
-        second_tee.rotate(180)
-
-        D = pg.union(D)
-        D.add_port(port=first_tee.ports[1], name="E")
-        D.add_port(port=first_tee.ports[2], name="W")
-        D.add_port(port=first_tee.ports[3], name="S")
-        D.add_port(port=second_tee.ports[3], name="N")
-
-        D.flatten()
-        return D
-
-    def crossB():
-
-        D = Device()
-        tee = pg.tee(
-            (3 * w_inductor, w_inductor), (w_inductor, w_inductor), taper_type="fillet"
-        )
-        first_tee = D << tee.movey(-w_inductor / 2)
-        first_tee.rotate(180)
-
-        D.add_port(port=first_tee.ports[1], name="W")
-        D.add_port(port=first_tee.ports[2], name="E")
-        D.add_port(port=first_tee.ports[3], name="N")
-
-        D.flatten()
-        return D
-
-    def crossC():
-
-        D = Device()
-        tee = pg.tee(
-            (3 * w_inductor, w_inductor), (w_inductor, w_inductor), taper_type="fillet"
-        )
-        first_tee = D << tee.movey(-w_inductor / 2)
-        first_tee.rotate(90)
-
-        D.add_port(port=first_tee.ports[1], name="N")
-        D.add_port(port=first_tee.ports[2], name="S")
-        D.add_port(port=first_tee.ports[3], name="E")
-
-        D.flatten()
-        return D
-
-    def create_snspd():
-        ## SNSPD
-        SNSPD = SNSPD_NTRON << device.snspd.basic(
-            wire_width=w_snspd,
-            wire_pitch=pitch_snspd,
-            size=size_snspd,
-            num_squares=None,
-            turn_ratio=4,
-            terminals_same_side=False,
-            layer=layer,
-        )
-        SNSPD.rotate(90)
-        # port 1 connected to gnd
-        route = ROUTES << pg.optimal_step(SNSPD.ports[1].width, w_pad, symmetric=True)
-        route.connect(route.ports[1], SNSPD.ports[1])
-        SNSPD_NTRON.add_port(port=route.ports[2], name="S1")
-        # port 2 connected to crossA south
-        route_step = ROUTES << pg.optimal_step(
-            SNSPD.ports[2].width, CROSSA.ports["S"].width, symmetric=True
-        )
-        route_step.connect(route_step.ports[1], SNSPD.ports[2])
-        route = ROUTES << pg.compass((w_inductor, w_pad / 2))
-        route.connect(route.ports["S"], route_step.ports[2])
-        CROSSA.connect(CROSSA.ports["S"], route.ports["N"])
-
-    def create_inductor1():
-        ## INDUCTOR1
-        INDUCTOR1 = SNSPD_NTRON << device.snspd.basic(
-            wire_width=w_inductor,
-            wire_pitch=pitch_inductor,
-            size=size_inductor13,
-            num_squares=None,
-            terminals_same_side=False,
-            layer=layer,
-        )
-        INDUCTOR1.rotate(90).mirror()
-        # port 1 connected to crossA north
-        route = ROUTES << pg.compass((w_inductor, w_pad / 2))
-        route.connect(route.ports["S"], CROSSA.ports["N"])
-        INDUCTOR1.connect(INDUCTOR1.ports[1], route.ports["N"])
-        # port 2 connected to pad
-        route = ROUTES << pg.optimal_step(
-            INDUCTOR1.ports[2].width, w_pad, symmetric=True
-        )
-        route.connect(route.ports[1], INDUCTOR1.ports[2])
-        SNSPD_NTRON.add_port(port=route.ports[2], name="N1")
-
-    def create_inductor2():
-        ## INDUCTOR2
-        INDUCTOR2 = SNSPD_NTRON << device.snspd.basic(
-            wire_width=w_inductor,
-            wire_pitch=pitch_inductor,
-            size=size_inductor2,
-            num_squares=None,
-            terminals_same_side=True,
-            layer=layer,
-        )
-        arcleft = ROUTES << pg.arc(radius=2 * w_inductor, width=w_inductor, theta=90)
-        arcright = ROUTES << pg.arc(radius=2 * w_inductor, width=w_inductor, theta=90)
-        # connect arcleft to crossA east
-        arcleft.mirror()
-        arcleft.connect(arcleft.ports[2], CROSSA.ports["E"])
-        # connect INDUCTOR2 to arcleft
-        INDUCTOR2.connect(INDUCTOR2.ports[1], arcleft.ports[1])
-        # connect arcright to INDUCTOR2
-        arcright.connect(arcright.ports[1], INDUCTOR2.ports[2])
-        # arcright's port 2 connected to crossB west
-        route = ROUTES << pg.compass((w_pad / 2, w_inductor))
-        route.connect(route.ports["W"], arcright.ports[2])
-        CROSSB.connect(CROSSB.ports["W"], route.ports["E"])
-
-    def create_ntron():
-        ## NTRON
-        NTRON = SNSPD_NTRON << device.ntron.smooth(
-            choke_w=w_choke,
-            gate_w=w_inductor,
-            channel_w=w_channel,
-            source_w=w_inductor,
-            drain_w=w_inductor,
-            choke_shift=-3 * w_channel,
-            layer=layer,
-        )
-        # port 3 connected to crossB east
-        route = ROUTES << pg.compass((w_pad / 2, w_inductor))
-        route.connect(route.ports["W"], CROSSB.ports["E"])
-        NTRON.connect(NTRON.ports[3], route.ports["E"])
-        # port 1 connected to crossC south
-        route = ROUTES << pg.compass((w_inductor, w_pad / 2))
-        route.connect(route.ports["S"], NTRON.ports[1])
-        CROSSC.connect(CROSSC.ports["S"], route.ports["N"])
-        # port 2 connected to gnd
-        route = ROUTES << pg.optimal_step(NTRON.ports[2].width, w_pad, symmetric=True)
-        route.connect(route.ports[1], NTRON.ports[2])
-        SNSPD_NTRON.add_port(port=route.ports[2], name="S2")
-
-    def create_inductor3():
-        ## INDUCTOR3
-        INDUCTOR3 = SNSPD_NTRON << device.snspd.basic(
-            wire_width=w_inductor,
-            wire_pitch=pitch_inductor,
-            size=size_inductor13,
-            num_squares=None,
-            terminals_same_side=False,
-            layer=layer,
-        )
-        INDUCTOR3.rotate(90)
-        # port 1 connected to crossC north
-        route = ROUTES << pg.compass((w_inductor, w_pad / 2))
-        route.connect(route.ports["S"], CROSSC.ports["N"])
-        INDUCTOR3.connect(INDUCTOR3.ports[1], route.ports["N"])
-        # port 2 connected to pad
-        route = ROUTES << pg.optimal_step(
-            INDUCTOR3.ports[2].width, w_pad, symmetric=True
-        )
-        route.connect(route.ports[1], INDUCTOR3.ports[2])
-        SNSPD_NTRON.add_port(port=route.ports[2], name="N3")
-
-    def create_probing_routes():
-        ## SNSPD PROBING PAD
-        step = ROUTES << pg.optimal_step(w_inductor, w_pad, symmetric=True)
-        step.connect(step.ports[1], CROSSA.ports["W"])
-        route = ROUTES << pg.compass((abs(SNSPD_NTRON.xmin - step.xmin), w_pad))
-        route.connect(route.ports["E"], step.ports[2])
-        SNSPD_NTRON.add_port(port=route.ports["W"], name="W1")
-
-        ## NTRON IN PROBING PAD
-        step = ROUTES << pg.optimal_step(w_inductor, w_pad, symmetric=True)
-        step.connect(step.ports[1], CROSSB.ports["N"])
-        route = ROUTES << pg.compass((w_pad, abs(SNSPD_NTRON.ymax - step.ymax)))
-        route.connect(route.ports["S"], step.ports[2])
-        SNSPD_NTRON.add_port(port=route.ports["N"], name="N2")
-
-        ## NTRON OUT PROBING PAD
-        step = ROUTES << pg.optimal_step(w_inductor, w_pad, symmetric=True)
-        step.connect(step.ports[1], CROSSC.ports["E"])
-        route = ROUTES << pg.compass((abs(SNSPD_NTRON.xmax - step.xmax), w_pad))
-        route.connect(route.ports["W"], step.ports[2])
-        SNSPD_NTRON.add_port(port=route.ports["E"], name="E1")
-
-    SNSPD_NTRON = Device(f"SNSPD NTRON {w_snspd} {w_choke} ")
-    ROUTES = Device("ROUTES")
-
-    size_inductor13, size_inductor2 = scale_inductors_to_snspd()
-
-    CROSSA = ROUTES << crossA()
-    CROSSB = ROUTES << crossB()
-    CROSSC = ROUTES << crossC()
-
-    create_snspd()
-    create_inductor1()
-    create_inductor2()
-    create_ntron()
-    create_inductor3()
-    create_probing_routes()
-
-    SNSPD_NTRON << ROUTES.flatten()
-    # SNSPD_NTRON.flatten()
-
-    # ports = SNSPD_NTRON.get_ports()
-    # SNSPD_NTRON = pg.union(SNSPD_NTRON, layer=layer)
-    # for port in ports:
-    #     SNSPD_NTRON.add_port(port)
-
-    SNSPD_NTRON.move(SNSPD_NTRON.center, (0, 0))
-    SNSPD_NTRON.name = f"SNSPD NTRON {w_snspd} {w_choke} "
-    return SNSPD_NTRON
+"""Circuits module contains a library of QNN's circuits (e.g. snspd coupled to
+ntron, logic gates etc.)"""
+
+from phidl import Device
+import phidl.geometry as pg
+from typing import Tuple, Union
+import math
+
+import qnngds.devices as device
+
+
+def snspd_ntron(
+    w_snspd: float = 0.1,
+    pitch_snspd: float = 0.3,
+    size_snspd: Tuple[Union[int, float]] = (3, 3),
+    w_inductor: float = 0.3,
+    pitch_inductor: float = 0.6,
+    k_inductor13: Union[int, float] = 10,
+    k_inductor2: Union[int, float] = 4,
+    w_choke: float = 0.02,
+    w_channel: float = 0.12,
+    w_pad: Union[int, float] = 1,
+    layer: int = 0,
+) -> Device:
+    """Creates a SNSPD coupled to an NTRON, with 3 inductors in the circuit as:
+
+    >>> |        |
+    >>> L1       L3
+    >>> |        |
+    >>> |__L2__NTRON
+    >>> |        |
+    >>> SNSPD
+    >>> |
+
+    The length of L1, L2, and L3 (long nanowires) where scaled against the SNSPD:
+    L1 = L3 = k13 * L and L2 = k2 * L where L is the SNSPD kinetic inductance.
+
+    Parameters:
+        w_snspd (float): Width of the SNSPD.
+        pitch_snspd (float): Pitch of the SNSPD.
+        size_snspd (Tuple[Union[int, float]]): Size of the SNSPD.
+        w_inductor (float): Width of the inductors.
+        pitch_inductor (float): Pitch of the inductors.
+        k_inductor13 (Union[int, float]): The factor for scaling L1 and L3 relative to the SNSPD kinetic inductance.
+        k_inductor2 (Union[int, float]): The factor for scaling L2 relative to the SNSPD kinetic inductance.
+        w_choke (float): Width of the choke in the NTRON.
+        w_channel (float): Width of the channel in the NTRON.
+        w_pad (Union[int, float]): Width of the external connections to the cell.
+        layer (int): Layer of the device.
+
+    Returns:
+        Device: The created device.
+    """
+
+    def scale_inductors_to_snspd():
+
+        l_snspd = size_snspd[0] * size_snspd[1] / pitch_snspd
+        l_inductor13 = k_inductor13 * w_inductor / w_snspd * l_snspd
+        l_inductor2 = k_inductor2 * w_inductor / w_snspd * l_snspd
+
+        n_inductor13 = math.sqrt(l_inductor13 * pitch_inductor)
+        n_inductor2 = math.sqrt(l_inductor2 * pitch_inductor)
+
+        size_inductor13 = (n_inductor13, n_inductor13)
+        size_inductor2 = (n_inductor2, n_inductor2)
+
+        return size_inductor13, size_inductor2
+
+    def crossA():
+
+        D = Device()
+        tee = pg.tee(
+            (3 * w_inductor, w_inductor), (w_inductor, w_inductor), taper_type="fillet"
+        )
+        first_tee = D << tee.movey(-w_inductor / 2)
+        second_tee = D << tee
+        second_tee.rotate(180)
+
+        D = pg.union(D)
+        D.add_port(port=first_tee.ports[1], name="E")
+        D.add_port(port=first_tee.ports[2], name="W")
+        D.add_port(port=first_tee.ports[3], name="S")
+        D.add_port(port=second_tee.ports[3], name="N")
+
+        D.flatten()
+        return D
+
+    def crossB():
+
+        D = Device()
+        tee = pg.tee(
+            (3 * w_inductor, w_inductor), (w_inductor, w_inductor), taper_type="fillet"
+        )
+        first_tee = D << tee.movey(-w_inductor / 2)
+        first_tee.rotate(180)
+
+        D.add_port(port=first_tee.ports[1], name="W")
+        D.add_port(port=first_tee.ports[2], name="E")
+        D.add_port(port=first_tee.ports[3], name="N")
+
+        D.flatten()
+        return D
+
+    def crossC():
+
+        D = Device()
+        tee = pg.tee(
+            (3 * w_inductor, w_inductor), (w_inductor, w_inductor), taper_type="fillet"
+        )
+        first_tee = D << tee.movey(-w_inductor / 2)
+        first_tee.rotate(90)
+
+        D.add_port(port=first_tee.ports[1], name="N")
+        D.add_port(port=first_tee.ports[2], name="S")
+        D.add_port(port=first_tee.ports[3], name="E")
+
+        D.flatten()
+        return D
+
+    def create_snspd():
+        ## SNSPD
+        SNSPD = SNSPD_NTRON << device.snspd.basic(
+            wire_width=w_snspd,
+            wire_pitch=pitch_snspd,
+            size=size_snspd,
+            num_squares=None,
+            turn_ratio=4,
+            terminals_same_side=False,
+            layer=layer,
+        )
+        SNSPD.rotate(90)
+        # port 1 connected to gnd
+        route = ROUTES << pg.optimal_step(SNSPD.ports[1].width, w_pad, symmetric=True)
+        route.connect(route.ports[1], SNSPD.ports[1])
+        SNSPD_NTRON.add_port(port=route.ports[2], name="S1")
+        # port 2 connected to crossA south
+        route_step = ROUTES << pg.optimal_step(
+            SNSPD.ports[2].width, CROSSA.ports["S"].width, symmetric=True
+        )
+        route_step.connect(route_step.ports[1], SNSPD.ports[2])
+        route = ROUTES << pg.compass((w_inductor, w_pad / 2))
+        route.connect(route.ports["S"], route_step.ports[2])
+        CROSSA.connect(CROSSA.ports["S"], route.ports["N"])
+
+    def create_inductor1():
+        ## INDUCTOR1
+        INDUCTOR1 = SNSPD_NTRON << device.snspd.basic(
+            wire_width=w_inductor,
+            wire_pitch=pitch_inductor,
+            size=size_inductor13,
+            num_squares=None,
+            terminals_same_side=False,
+            layer=layer,
+        )
+        INDUCTOR1.rotate(90).mirror()
+        # port 1 connected to crossA north
+        route = ROUTES << pg.compass((w_inductor, w_pad / 2))
+        route.connect(route.ports["S"], CROSSA.ports["N"])
+        INDUCTOR1.connect(INDUCTOR1.ports[1], route.ports["N"])
+        # port 2 connected to pad
+        route = ROUTES << pg.optimal_step(
+            INDUCTOR1.ports[2].width, w_pad, symmetric=True
+        )
+        route.connect(route.ports[1], INDUCTOR1.ports[2])
+        SNSPD_NTRON.add_port(port=route.ports[2], name="N1")
+
+    def create_inductor2():
+        ## INDUCTOR2
+        INDUCTOR2 = SNSPD_NTRON << device.snspd.basic(
+            wire_width=w_inductor,
+            wire_pitch=pitch_inductor,
+            size=size_inductor2,
+            num_squares=None,
+            terminals_same_side=True,
+            layer=layer,
+        )
+        arcleft = ROUTES << pg.arc(radius=2 * w_inductor, width=w_inductor, theta=90)
+        arcright = ROUTES << pg.arc(radius=2 * w_inductor, width=w_inductor, theta=90)
+        # connect arcleft to crossA east
+        arcleft.mirror()
+        arcleft.connect(arcleft.ports[2], CROSSA.ports["E"])
+        # connect INDUCTOR2 to arcleft
+        INDUCTOR2.connect(INDUCTOR2.ports[1], arcleft.ports[1])
+        # connect arcright to INDUCTOR2
+        arcright.connect(arcright.ports[1], INDUCTOR2.ports[2])
+        # arcright's port 2 connected to crossB west
+        route = ROUTES << pg.compass((w_pad / 2, w_inductor))
+        route.connect(route.ports["W"], arcright.ports[2])
+        CROSSB.connect(CROSSB.ports["W"], route.ports["E"])
+
+    def create_ntron():
+        ## NTRON
+        NTRON = SNSPD_NTRON << device.ntron.smooth(
+            choke_w=w_choke,
+            gate_w=w_inductor,
+            channel_w=w_channel,
+            source_w=w_inductor,
+            drain_w=w_inductor,
+            choke_shift=-3 * w_channel,
+            layer=layer,
+        )
+        # port 3 connected to crossB east
+        route = ROUTES << pg.compass((w_pad / 2, w_inductor))
+        route.connect(route.ports["W"], CROSSB.ports["E"])
+        NTRON.connect(NTRON.ports[3], route.ports["E"])
+        # port 1 connected to crossC south
+        route = ROUTES << pg.compass((w_inductor, w_pad / 2))
+        route.connect(route.ports["S"], NTRON.ports[1])
+        CROSSC.connect(CROSSC.ports["S"], route.ports["N"])
+        # port 2 connected to gnd
+        route = ROUTES << pg.optimal_step(NTRON.ports[2].width, w_pad, symmetric=True)
+        route.connect(route.ports[1], NTRON.ports[2])
+        SNSPD_NTRON.add_port(port=route.ports[2], name="S2")
+
+    def create_inductor3():
+        ## INDUCTOR3
+        INDUCTOR3 = SNSPD_NTRON << device.snspd.basic(
+            wire_width=w_inductor,
+            wire_pitch=pitch_inductor,
+            size=size_inductor13,
+            num_squares=None,
+            terminals_same_side=False,
+            layer=layer,
+        )
+        INDUCTOR3.rotate(90)
+        # port 1 connected to crossC north
+        route = ROUTES << pg.compass((w_inductor, w_pad / 2))
+        route.connect(route.ports["S"], CROSSC.ports["N"])
+        INDUCTOR3.connect(INDUCTOR3.ports[1], route.ports["N"])
+        # port 2 connected to pad
+        route = ROUTES << pg.optimal_step(
+            INDUCTOR3.ports[2].width, w_pad, symmetric=True
+        )
+        route.connect(route.ports[1], INDUCTOR3.ports[2])
+        SNSPD_NTRON.add_port(port=route.ports[2], name="N3")
+
+    def create_probing_routes():
+        ## SNSPD PROBING PAD
+        step = ROUTES << pg.optimal_step(w_inductor, w_pad, symmetric=True)
+        step.connect(step.ports[1], CROSSA.ports["W"])
+        route = ROUTES << pg.compass((abs(SNSPD_NTRON.xmin - step.xmin), w_pad))
+        route.connect(route.ports["E"], step.ports[2])
+        SNSPD_NTRON.add_port(port=route.ports["W"], name="W1")
+
+        ## NTRON IN PROBING PAD
+        step = ROUTES << pg.optimal_step(w_inductor, w_pad, symmetric=True)
+        step.connect(step.ports[1], CROSSB.ports["N"])
+        route = ROUTES << pg.compass((w_pad, abs(SNSPD_NTRON.ymax - step.ymax)))
+        route.connect(route.ports["S"], step.ports[2])
+        SNSPD_NTRON.add_port(port=route.ports["N"], name="N2")
+
+        ## NTRON OUT PROBING PAD
+        step = ROUTES << pg.optimal_step(w_inductor, w_pad, symmetric=True)
+        step.connect(step.ports[1], CROSSC.ports["E"])
+        route = ROUTES << pg.compass((abs(SNSPD_NTRON.xmax - step.xmax), w_pad))
+        route.connect(route.ports["W"], step.ports[2])
+        SNSPD_NTRON.add_port(port=route.ports["E"], name="E1")
+
+    SNSPD_NTRON = Device(f"SNSPD NTRON {w_snspd} {w_choke} ")
+    ROUTES = Device("ROUTES")
+
+    size_inductor13, size_inductor2 = scale_inductors_to_snspd()
+
+    CROSSA = ROUTES << crossA()
+    CROSSB = ROUTES << crossB()
+    CROSSC = ROUTES << crossC()
+
+    create_snspd()
+    create_inductor1()
+    create_inductor2()
+    create_ntron()
+    create_inductor3()
+    create_probing_routes()
+
+    SNSPD_NTRON << ROUTES.flatten()
+    # SNSPD_NTRON.flatten()
+
+    # ports = SNSPD_NTRON.get_ports()
+    # SNSPD_NTRON = pg.union(SNSPD_NTRON, layer=layer)
+    # for port in ports:
+    #     SNSPD_NTRON.add_port(port)
+
+    SNSPD_NTRON.move(SNSPD_NTRON.center, (0, 0))
+    SNSPD_NTRON.name = f"SNSPD NTRON {w_snspd} {w_choke} "
+    return SNSPD_NTRON
```

### Comparing `qnngds-2.4.1/src/qnngds/design.py` & `qnngds-2.5.0/src/qnngds/design.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,774 +1,772 @@
-"""Design's module is though for users to be able to access pre-built cells
-that are made of circuits, devices or test structures already integrated in a
-die cell.
-
-It is a module that is sufficient in itself to build an entire new
-design.
-"""
-
-from phidl import Device
-import phidl.geometry as pg
-from typing import Tuple, List, Union, Optional
-import os
-
-import qnngds.cells as cell
-import qnngds._default_param as dflt
-
-Free = True
-Occupied = False
-
-
-def create_chip(
-    chip_w: Union[int, float] = dflt.chip_w,
-    margin: Union[int, float] = dflt.chip_margin,
-    N_dies: int = dflt.N_dies,
-    die_w: Union[None, int, float] = dflt.auto_param,
-    annotations_layer: int = dflt.layers["annotation"],
-    unpack_chip_map: bool = True,
-    create_devices_map_txt: Union[bool, str] = False,
-) -> Union[
-    Tuple[Device, Union[int, float], List[List[bool]], str],
-    Tuple[Device, Union[int, float], str],
-    Tuple[Device, Union[int, float], List[List[bool]]],
-    Tuple[Device, Union[int, float]],
-]:
-    """Creates a chip map in the annotations layer.
-
-    If unpack_chip_map is set to True, creates a map (2D array) to monitor the
-    states of each cell of the chip. The user should input N_dies xor die_w.
-
-    Parameters:
-        chip_w (int or float): The overall width (in um) of the chip.
-        margin (int or float): The width (in um) of the outline of the chip where no device should be placed.
-        N_dies (int): Number of dies/units to be placed by row and column.
-        die_w (None, int, or float): If specified, the width of each die/unit to be placed by row and column.
-        annotations_layer (int or array-like[2]): The layer where to put the device.
-        unpack_chip_map (bool): If True, the function returns a map (2D array) of states to be filled later (e.g., with place_on_chip()).
-        create_devices_map_txt (bool or string): If True or string, the function creates a txt file that will map the devices.
-
-    Returns:
-        Tuple[Device, float, List[List[bool]], str]: A tuple containing from 2 to 4 elements, depending on what needs to be extracted (parameters dependent):
-
-        - **CHIP** (*Device*): The chip map.
-        - **die_w** (*float*): The width of each die. (returned if die_w was None)
-        - **N_dies** (*float*): The number of dies/units on each row and column. (returned if die_w was not None)
-        - **chip_map** (*array-like[N_dies][N_dies] of bool*): A 2D array filled with "Free" (=True) states. (returned if unpack_chip_map is True)
-        - **file_name** (*str*): The name of the created devices map text file. (returned if create_devices_map_txt is not False)
-    """
-
-    CHIP = Device("CHIP ")
-    CHIP.add_polygon(
-        [(0, 0), (chip_w, 0), (chip_w, chip_w), (0, chip_w)], layer=annotations_layer
-    )
-
-    useful_w = chip_w - margin * 2
-    useful_area = CHIP.add_polygon(
-        [(0, 0), (useful_w, 0), (useful_w, useful_w), (0, useful_w)],
-        layer=annotations_layer,
-    )
-    useful_area.move((margin, margin))
-
-    if die_w is not None:
-        N_dies = int(useful_w / die_w)
-        return_N_or_w = N_dies
-    else:
-        die_w = useful_w / N_dies
-        return_N_or_w = die_w
-    CELL = pg.rectangle([die_w, die_w], layer=annotations_layer)
-    array = CHIP.add_array(CELL, columns=N_dies, rows=N_dies, spacing=(die_w, die_w))
-    array.move((0, 0), (margin, margin))
-
-    CHIP.flatten()
-    CHIP.move((margin, margin), (0, 0))
-
-    if create_devices_map_txt:
-        ## create a devices map ...
-        if create_devices_map_txt == True:
-            file_name = "devices map"
-        else:
-            file_name = f"{create_devices_map_txt}"
-
-        # check that file does not already exist, in which case it will add a int to its name:
-        i = 0
-        file_to_find = file_name
-        while True:
-            if i != 0:
-                file_to_find = file_name + f"({i})"
-            file_already_exists = os.path.exists(f"{file_to_find}.txt")
-            i += 1
-            if not file_already_exists:
-                file_name = file_to_find
-                break
-        with open(f"{file_name}.txt", "a") as file:
-            file.write("Devices placed on the chip: \n\n")
-            file.write("(row, col) : device.name\n\n")
-
-        ## ... and return the devices map filename in the outputs
-        if unpack_chip_map:
-            chip_map = [[Free for _ in range(N_dies)] for _ in range(N_dies)]
-            return CHIP, return_N_or_w, chip_map, file_name
-        else:
-            return CHIP, return_N_or_w, file_name
-    else:
-        if unpack_chip_map:
-            chip_map = [[Free for _ in range(N_dies)] for _ in range(N_dies)]
-            return CHIP, return_N_or_w, chip_map
-        else:
-            return CHIP, return_N_or_w
-
-
-def place_on_chip(
-    cell: Device,
-    coordinates: Tuple[int, int],
-    chip_map: List[List[bool]],
-    die_w: Union[int, float],
-    devices_map_txt: Union[None, str] = None,
-) -> bool:
-    """Moves the chip to the coordinates specified.
-
-    Update the chip map with Occupied states where the device has been placed.
-
-    NB: The cell is aligned from its bottom left corner to the coordinates.
-
-    Parameters:
-        cell (Device): Device to be moved.
-        coordinates (tuple of int): (i, j) indices of the chip grid, where to place the cell.
-            Note that the indices start at 0.
-        chip_map (2D array): The 2D array mapping the free cells in the chip map.
-        die_w (int or float): The width of a die/unit in the chip map.
-        devices_map_txt (str or None): Name of the devices map text file to write placement information.
-            If None, no file will be written.
-
-    Returns:
-        bool: False, if the Device falls out of the chip map, prints an error
-        message and does not place the device. True, otherwise.
-
-    Raises:
-        Warning: Prints a warning if the Device is overlapping with already occupied coordinates.
-    """
-
-    # update the chip's availabilities
-    n_cell = round(cell.xsize / die_w)
-    m_cell = round(cell.ysize / die_w)
-    for n in range(n_cell):
-        for m in range(m_cell):
-            cell_name = cell.name.replace("\n", "")
-            try:
-                if chip_map[coordinates[1] + m][coordinates[0] + n] == Occupied:
-                    print(
-                        f"Warning, placing Device {cell_name} "
-                        + f"in an occupied state ({coordinates[1]+m}, {coordinates[0]+n})"
-                    )
-                else:
-                    chip_map[coordinates[1] + m][coordinates[0] + n] = Occupied
-            except IndexError:
-                print(
-                    f"Error, Device {cell_name} "
-                    + f"falls out of the chip map ({coordinates[1]+m}, {coordinates[0]+n})"
-                )
-                return False
-
-    # move the cell
-    cell_bottom_left = (
-        -n_cell * 0.5 * die_w,
-        -m_cell * 0.5 * die_w,
-    )
-    cell.move(cell_bottom_left, ((coordinates[0]) * die_w, (coordinates[1]) * die_w))
-
-    # write the cell's place on the devices map text file
-    if devices_map_txt is not None:
-        with open(f"{devices_map_txt}.txt", "a") as file:
-            try:
-                name = cell.name.replace("\n", "")
-            except AttributeError:
-                name = "unnamed"
-            file.write(f"({coordinates[0]}, {coordinates[1]}) : {name}\n")
-
-    return True
-
-
-def place_remaining_devices(
-    devices_to_place: List[Device],
-    chip_map: List[List[bool]],
-    die_w: Union[int, float],
-    write_devices_map_txt: Union[bool, str] = False,
-) -> Optional[None]:
-    """Go through the chip map and place the devices given, where the chip map
-    is Free.
-
-    Parameters:
-        devices_to_place (list of Device objects): The devices to be placed.
-        chip_map (2D array): The 2D array mapping the free cells in the chip map.
-        die_w (int or float): The width of a die/unit in the chip map.
-        write_devices_map_txt (bool or str): If True, write a .txt file mapping the devices that were placed.
-            If str, specifies the filename of the .txt file.
-
-    Note:
-        The list of devices is not re-ordered to fit as many of them as possible.
-        Some edges of the chip may remain empty because the list contained 2-units long devices (for e.g.).
-    """
-
-    # name and create the file if no file was given
-    if write_devices_map_txt == True:
-
-        file_name = "remaining_cells_map"
-        with open(f"{file_name}.txt", "a") as file:
-            file.write("Remaining devices placed on the chip:\n\n")
-            file.write("(row, col) : device.name\n\n")
-    # use the file's name is a file was given
-    elif write_devices_map_txt:
-        file_name = write_devices_map_txt
-    # pass false if no txt file should be created
-    else:
-        file_name = None
-
-    for row_i, row in enumerate(chip_map):
-        for col_i, status in enumerate(row):
-            if status == Free and devices_to_place:
-                if place_on_chip(
-                    devices_to_place[0], (col_i, row_i), chip_map, die_w, file_name
-                ):
-                    devices_to_place.pop(0)
-
-    if devices_to_place:
-        print(
-            "Some devices are still to be placed, " + "no place remaining on the chip."
-        )
-
-
-class Design:
-    """A class for a design on a single layer of superconducting material, and
-    additional contact pads.
-
-    It is though for a process like:
-
-    - exposing the superconductiong material using e-beam lithography. Two
-      exposures at low and high currents are possible by distinguishing two
-      layers: device layer and die layer. Equivalently, the shapes outlines
-      (though for positive tone resist) have two different widths for the device
-      and die layers.
-    - exposing the pads layer using photolithography.
-
-    Args:
-        name (str): The name of the design.
-        chip_w (int or float): The overall width of the chip.
-        chip_margin (int or float): The width of the outline of the chip where
-            no device should be placed.
-        N_dies (int): Number of dies/units to be placed by row and column.
-        die_w (int or float, optional): Width of a unit die/cell in the design
-            (the output device will be an integer number of unit cells).
-        pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
-        device_outline (int or float): The width of the device's outline.
-        die_outline (int or float): The width of the pads outline.
-        ebeam_overlap (int or float): Extra length of the routes above the die's
-            ports to assure alignment with the device (useful for ebeam
-            lithography).
-        annotation_layer (int): The layer where to put the annotations.
-        device_layer (int or array-like[2]): The layer where the device is placed.
-        die_layer (int or array-like[2]): The layer where the die is placed.
-        pad_layer (int or array-like[2]): The layer where the pads are placed.
-        fill_pad_layer (bool): If True, the space reserved for pads in the
-            die_cell in filled in pad's layer.
-
-    Example:
-        Here is an example of how to create the class.
-
-        >>> # Choose some design parameters, let the others to default
-        >>> chip_w = 10000
-        >>> N_dies = 11
-        >>> device_outline = 0.3
-        >>> die_outline = 10
-
-        >>> # Create the design and initialize the chip
-        >>> demo_project = Design(name="demo design",
-        >>>                       chip_w=chip_w,
-        >>>                       N_dies=N_dies,
-        >>>                       device_outline=device_outline,
-        >>>                       die_outline=die_outline)
-        >>> demo_project.create_chip()
-
-        >>> # Quickplot the chip skeletton!
-        >>> qp(demo_project.CHIP)
-    """
-
-    def __init__(
-        self,
-        name="new_design",
-        chip_w=dflt.chip_w,
-        chip_margin=dflt.chip_margin,
-        N_dies=dflt.auto_param,
-        die_w=dflt.die_w,
-        pad_size=dflt.pad_size,
-        device_outline=dflt.device_outline,
-        die_outline=dflt.die_outline,
-        ebeam_overlap=dflt.ebeam_overlap,
-        annotation_layer=dflt.layers["annotation"],
-        device_layer=dflt.layers["device"],
-        die_layer=dflt.layers["die"],
-        pad_layer=dflt.layers["pad"],
-        fill_pad_layer=False,
-    ):
-        """
-        Args:
-            name (str): The name of the design.
-            chip_w (int or float): The overall width of the chip.
-            chip_margin (int or float): The width of the outline of the chip where no device should be placed.
-            N_dies (int): Number of dies/units to be placed by row and column.
-            die_w (int or float, optional): Width of a unit die/cell in the
-                design (the output device will be an integer number of unit cells).
-            pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
-            device_outline (int or float): The width of the device's outline.
-            die_outline (int or float): The width of the pads outline.
-            ebeam_overlap (int or float): Extra length of the routes above the
-                die's ports to assure alignment with the device (useful for ebeam
-                lithography).
-            annotation_layer (int): The layer where to put the annotations.
-            device_layer (int or array-like[2]): The layer where the device is placed.
-            die_layer (int or array-like[2]): The layer where the die is placed.
-            pad_layer (int or array-like[2]): The layer where the pads are placed.
-            fill_pad_layer (bool): If True, the space reserved for pads in the
-                die_cell in filled in pad's layer.
-        """
-
-        self.name = name
-
-        self.chip_w = chip_w
-        self.chip_margin = chip_margin
-        self.N_dies = N_dies
-        self.die_w = die_w
-
-        self.pad_size = pad_size
-        self.device_outline = device_outline
-        self.die_outline = die_outline
-        self.ebeam_overlap = ebeam_overlap
-
-        self.layers = {
-            "annotation": annotation_layer,
-            "device": device_layer,
-            "die": die_layer,
-            "pad": pad_layer,
-        }
-
-        self.fill_pad_layer = fill_pad_layer
-
-    # help building a design
-
-    def create_chip(self, create_devices_map_txt: Union[bool, str] = True) -> Device:
-        """Creates the chip, with unit cells.
-
-        The CHIP created will be the foundation of the design, the Device to add
-        all references to. The function creates a chip_map (2D array) to help placing
-        the cells on the chip (aligned with the unit cells). The function also generates
-        a txt file if create_devices_map_txt is True to follow the devices placements
-        on the chip.
-
-        Parameters:
-            create_devices_map_txt (bool or str): If True, generates a text file
-                to follow the devices placements on the chip. If string, the text file
-                is named after the string.
-
-        Returns:
-            CHIP (Device): The chip map, in the annotations layer
-        """
-        if create_devices_map_txt:
-            if create_devices_map_txt == True:
-                create_devices_map_txt = f"{self.name} devices map"
-            else:
-                create_devices_map_txt = f"{create_devices_map_txt}"
-            self.CHIP, N_or_w, self.chip_map, self.devices_map_txt = create_chip(
-                chip_w=self.chip_w,
-                margin=self.chip_margin,
-                N_dies=self.N_dies,
-                die_w=self.die_w,
-                annotations_layer=self.layers["annotation"],
-                unpack_chip_map=True,
-                create_devices_map_txt=create_devices_map_txt,
-            )
-        else:
-            self.devices_map_txt = None
-            create_devices_map_txt = False
-            self.CHIP, N_or_w, self.chip_map = create_chip(
-                chip_w=self.chip_w,
-                margin=self.chip_margin,
-                N_dies=self.N_dies,
-                die_w=self.die_w,
-                annotations_layer=self.layers["annotation"],
-                unpack_chip_map=True,
-                create_devices_map_txt=create_devices_map_txt,
-            )
-
-        if self.die_w is not None:
-            self.N_dies = N_or_w
-        else:
-            self.die_w = N_or_w
-
-        return self.CHIP
-
-    def place_on_chip(
-        self, cell: Device, coordinates: Tuple[int, int], add_to_chip: bool = True
-    ) -> bool:
-        """Moves the chip to the coordinates specified. Update the chip map
-        with Occupied states where the device has been placed.
-
-        NB: the cell is aligned from its bottom left corner to the coordinates.
-
-        Parameters:
-            cell (Device): Device to be moved.
-            coordinates (tuple of int): (i, j) indices of the chip grid, where to place the cell.
-                Note that the indices start at 0.
-
-        Returns:
-            bool: False, if the Device falls out of the chip map, prints an error message and does not place the device. True, otherwise.
-
-        Raises:
-            Warning: Prints a warning if the Device is overlapping with already occupied coordinates.
-
-        Examples:
-            Here is an example of placing alignment cells on two given positions of the chip.
-
-            >>> align_left  = demo_project.create_alignment_cell(layers_to_align=[2, 3])
-            >>> align_right = demo_project.create_alignment_cell(layers_to_align=[2, 3])
-            >>> demo_project.place_on_chip(cell=align_left,  coordinates=(0, 5))
-            >>> demo_project.place_on_chip(cell=align_right, coordinates=(10, 5))
-        """
-
-        if add_to_chip:
-            self.CHIP << cell
-        return place_on_chip(
-            cell=cell,
-            coordinates=coordinates,
-            chip_map=self.chip_map,
-            die_w=self.die_w,
-            devices_map_txt=self.devices_map_txt,
-        )
-
-    def place_remaining_devices(
-        self,
-        devices_to_place: List[Device],
-        add_to_chip: bool = True,
-        write_remaining_devices_map_txt: Union[bool, str] = False,
-    ) -> Optional[None]:
-        """Go through the chip map and place the devices given, where the chip
-        map is Free.
-
-        Parameters:
-            devices_to_place (list of Device objects): The devices to be placed.
-            add_to_chip (bool): Add the devices provided to the Design's CHIP.
-            write_remaining_devices_map_txt (bool or string): If True, write a .txt
-                file mapping the devices that were placed. If string, the filename is
-                the given string, except if a file has already been created.
-
-        Note:
-            The list of devices is not re-ordered to fit as many of them as possible.
-            Some edges of the chip may remain empty because the list contained 2-units long devices (for e.g.).
-
-        Examples:
-            Here is a typical example of why this function is useful and how to
-            use it. If design is a Design class initalized, and the
-            create_chip() function has previously been executed.
-
-            >>> channels_w = [0.5, 0.75, 1, 1.25, 1.5]
-            >>> ntrons_to_place = []
-            >>> for channel_w in channels_w:
-            >>>     ntron = design.create_ntron_cell(choke_w=0.05, channel_w=channel_w)
-            >>>     ntrons_to_place.append(ntron)
-            >>> design.place_remaining_cells(ntrons_to_place)
-        """
-        if self.devices_map_txt is not None:
-            # the decision taken when creating the chip overwrites this one
-            write_devices_map_txt = self.devices_map_txt
-        else:
-            # a devices map can still be created, as decided when calling this function
-            write_devices_map_txt = write_remaining_devices_map_txt
-
-        if add_to_chip:
-            self.CHIP << devices_to_place
-        place_remaining_devices(
-            devices_to_place=devices_to_place,
-            chip_map=self.chip_map,
-            die_w=self.die_w,
-            write_devices_map_txt=write_devices_map_txt,
-        )
-
-    def write_gds(self, text: Union[None, str] = dflt.text) -> Union[None, str]:
-        """Write a GDS file.
-
-        Args:
-            text (str or None): The filename for the GDS file.
-                If None, the name of the Design will be used.
-
-        Returns:
-            str or None: The filename of the written GDS file, or None if no file was written.
-        """
-        if text is None:
-            text = self.name
-        return self.CHIP.write_gds(filename=f"{text}.gds", max_cellname_length=32000)
-
-    # basics:
-
-    def alignment_cell(
-        self, layers_to_align: List[int], text: Union[None, str] = dflt.text
-    ) -> Device:
-        """Creates alignment marks in an integer number of unit cells.
-
-        Parameters:
-            layers_to_align (List[int]): Layers to align.
-            text (str, optional): If None, the text is f"lay={layers_to_align}".
-
-        Returns:
-            Device: A device that centers the alignment marks in an n*m unit cell.
-        """
-        return cell.alignment(
-            die_w=self.die_w,
-            layers_to_align=layers_to_align,
-            outline_die=self.die_outline,
-            die_layer=self.layers["die"],
-            text=text,
-        )
-
-    def vdp_cell(
-        self,
-        layers_to_probe: List[int],
-        layers_to_outline: Union[List[int], None] = dflt.auto_param,
-        text: Union[None, str] = dflt.text,
-    ) -> Device:
-        r"""Creates a cell containing a Van Der Pauw structure between 4 contact
-        pads.
-
-        Parameters:
-            layers_to_probe (List[int]): The layers on which to place the VDP structure.
-            layers_to_outline (List[int]): Among the VDP layers, the ones for which structure must not be filled but outlined.
-            text (str, optional): If None, the text is f"lay={layers_to_probe}".
-
-        Returns:
-            Device: The created device.
-        """
-
-        return cell.vdp(
-            die_w=self.die_w,
-            pad_size=self.pad_size,
-            layers_to_probe=layers_to_probe,
-            layers_to_outline=layers_to_outline,
-            outline=self.die_outline,
-            die_layer=self.layers["die"],
-            pad_layer=self.layers["pad"],
-            text=text,
-        )
-
-    def etch_test_cell(
-        self, layers_to_etch: List[List[int]], text: Union[None, str] = dflt.text
-    ) -> Device:
-        """Creates etch test structures in an integer number of unit cells.
-
-        These test structures are thought to be used by probing on pads (with a simple multimeter)
-        that should be isolated one from another if the etching is complete.
-
-        Parameters:
-            layers_to_etch (List[List[int]]): Each element of the list corresponds to one test point,
-                to put on the list of layers specified. Example: [[1, 2], [1], [2]].
-            text (str, optional): If None, the text is f"lay={layers_to_etch}".
-
-        Returns:
-            Device: A device (with size n*m of unit cells) with etch tests in its center.
-        """
-
-        return cell.etch_test(
-            die_w=self.die_w,
-            layers_to_etch=layers_to_etch,
-            outline_die=self.die_outline,
-            die_layer=self.layers["die"],
-            text=text,
-        )
-
-    def resolution_test_cell(
-        self,
-        layer_to_resolve: int,
-        resolutions_to_test: List[float] = [
-            0.025,
-            0.05,
-            0.075,
-            0.1,
-            0.25,
-            0.5,
-            1,
-            1.5,
-            2,
-        ],
-        text: Union[None, str] = dflt.text,
-    ) -> Device:
-        r"""Creates a cell containing a resolution test.
-
-        Parameters:
-            layer_to_resolve (int): The layer to put the resolution test on.
-            resolutions_to_test (List[float]): The resolutions to test in µm.
-            text (str, optional): If None, the text is f"lay={layer_to_resolve}".
-
-        Returns:
-            Device: The created device.
-        """
-
-        return cell.resolution_test(
-            die_w=self.die_w,
-            layer_to_resolve=layer_to_resolve,
-            resolutions_to_test=resolutions_to_test,
-            outline=self.die_outline,
-            die_layer=self.layers["die"],
-            text=text,
-        )
-
-    # devices:
-
-    def nanowires_cell(
-        self,
-        channels_sources_w: List[Tuple[float, float]],
-        text: Union[None, str] = dflt.text,
-    ) -> Device:
-        """Creates a cell containing several nanowires of given channel and
-        source.
-
-        Parameters:
-            channels_sources_w (List[Tuple[float, float]]): The list of
-                (channel_w, source_w) of the nanowires to create.
-            text (str, optional): If None, the text is f"w={channels_w}".
-
-        Returns:
-            Device: A device containing the nanowires, the border of the die
-            (created with die_cell function), and the connections between the
-            nanowires and pads.
-        """
-
-        return cell.nanowires(
-            die_w=self.die_w,
-            pad_size=self.pad_size,
-            channels_sources_w=channels_sources_w,
-            overlap_w=self.ebeam_overlap,
-            outline_die=self.die_outline,
-            outline_dev=self.device_outline,
-            device_layer=self.layers["device"],
-            die_layer=self.layers["die"],
-            pad_layer=self.layers["pad"],
-            text=text,
-            fill_pad_layer=self.fill_pad_layer,
-        )
-
-    def ntron_cell(
-        self,
-        choke_w: float,
-        channel_w: float,
-        gate_w: Union[float, None] = dflt.auto_param,
-        source_w: Union[float, None] = dflt.auto_param,
-        drain_w: Union[float, None] = dflt.auto_param,
-        choke_shift: Union[float, None] = dflt.auto_param,
-        text: Union[str, None] = dflt.text,
-    ) -> Device:
-        r"""Creates a standardized cell specifically for a single ntron.
-
-        Unless specified, scales the ntron parameters as:
-        gate_w = drain_w = source_w = 3*channel_w
-        choke_shift = -3*channel_w
-
-        Parameters:
-            choke_w (int or float): The width of the ntron's choke in µm.
-            channel_w (int or float): The width of the ntron's channel in µm.
-            gate_w (int or float, optional): If None, gate width is 3 times the channel width.
-            source_w (int or float, optional): If None, source width is 3 times the channel width.
-            drain_w (int or float, optional): If None, drain width is 3 times the channel width.
-            choke_shift (int or float, optional): If None, choke shift is -3 times the channel width.
-            text (str, optional): If None, the text is f"chk: {choke_w} \\nchnl: {channel_w}".
-
-        Returns:
-            Device: A device containing the ntron, the border of the die (created with die_cell function),
-            and the connections between the ports.
-        """
-
-        return cell.ntron(
-            die_w=self.die_w,
-            pad_size=self.pad_size,
-            choke_w=choke_w,
-            channel_w=channel_w,
-            gate_w=gate_w,
-            source_w=source_w,
-            drain_w=drain_w,
-            choke_shift=choke_shift,
-            overlap_w=self.ebeam_overlap,
-            outline_die=self.die_outline,
-            outline_dev=self.device_outline,
-            device_layer=self.layers["device"],
-            die_layer=self.layers["die"],
-            pad_layer=self.layers["pad"],
-            text=text,
-            fill_pad_layer=self.fill_pad_layer,
-        )
-
-    def snspd_cell(
-        self,
-        snspd_width: float = 0.2,
-        snspd_pitch: float = 0.6,
-        snspd_size: Tuple[Union[int, float], Union[int, float]] = (100, 100),
-        snspd_num_squares: Optional[int] = None,
-        text: Union[None, str] = dflt.text,
-    ) -> Device:
-        """Creates a cell that contains a vertical superconducting nanowire
-        single-photon detector (SNSPD).
-
-        Parameters:
-            snspd_width (float): Width of the nanowire.
-            snspd_pitch (float): Pitch of the nanowire.
-            snspd_size (tuple of int or float): Size of the detector in squares (width, height).
-            snspd_num_squares (Optional[int]): Number of squares in the detector.
-            text (string, optional): If None, the text is f"w={snspd_width}".
-
-        Returns:
-            Device: A cell (of size n*m unit die_cells) containing the SNSPD.
-        """
-
-        return cell.snspd(
-            die_w=self.die_w,
-            pad_size=self.pad_size,
-            snspd_width=snspd_width,
-            snspd_pitch=snspd_pitch,
-            snspd_size=snspd_size,
-            snspd_num_squares=snspd_num_squares,
-            overlap_w=self.ebeam_overlap,
-            outline_die=self.die_outline,
-            outline_dev=self.device_outline,
-            device_layer=self.layers["device"],
-            die_layer=self.layers["die"],
-            pad_layer=self.layers["pad"],
-            text=text,
-            fill_pad_layer=self.fill_pad_layer,
-        )
-
-    def snspd_ntron_cell(
-        self,
-        w_choke: float,
-        w_snspd: Union[float, None] = dflt.auto_param,
-        text: Union[str, None] = dflt.text,
-    ) -> Device:
-        """Creates a cell that contains an SNSPD coupled to an NTRON. The
-        device's parameters are sized according to the SNSPD's width and the
-        NTRON's choke.
-
-        Parameters:
-            w_choke (int or float): The width of the NTRON choke in µm.
-            w_snspd (int or float, optional): The width of the SNSPD nanowire in µm. If None, scaled to 5*w_choke.
-            text (string, optional): If None, the text is f"w={w_snspd}, {w_choke}".
-
-        Returns:
-            Device: A cell containing a die in die_layer, pads in pad layer, and an SNSPD-NTRON properly routed in the device layer.
-        """
-
-        return cell.snspd_ntron(
-            die_w=self.die_w,
-            pad_size=self.pad_size,
-            w_choke=w_choke,
-            w_snspd=w_snspd,
-            overlap_w=self.ebeam_overlap,
-            outline_die=self.die_outline,
-            outline_dev=self.device_outline,
-            device_layer=self.layers["device"],
-            die_layer=self.layers["die"],
-            pad_layer=self.layers["pad"],
-            text=text,
-            fill_pad_layer=self.fill_pad_layer,
-        )
+"""Design's module is though for users to be able to access pre-built cells
+that are made of circuits, devices or test structures already integrated in a
+die cell.
+
+It is a module that is sufficient in itself to build an entire new
+design.
+"""
+
+from phidl import Device
+import phidl.geometry as pg
+from typing import Tuple, List, Union, Optional
+import os
+
+import qnngds.cells as cell
+import qnngds._default_param as dflt
+
+Free = True
+Occupied = False
+
+
+def create_chip(
+    chip_w: Union[int, float] = dflt.chip_w,
+    margin: Union[int, float] = dflt.chip_margin,
+    N_dies: int = dflt.N_dies,
+    die_w: Union[None, int, float] = dflt.auto_param,
+    annotations_layer: int = dflt.layers["annotation"],
+    unpack_chip_map: bool = True,
+    create_devices_map_txt: Union[bool, str] = False,
+) -> Union[
+    Tuple[Device, Union[int, float], List[List[bool]], str],
+    Tuple[Device, Union[int, float], str],
+    Tuple[Device, Union[int, float], List[List[bool]]],
+    Tuple[Device, Union[int, float]],
+]:
+    """Creates a chip map in the annotations layer.
+
+    If unpack_chip_map is set to True, creates a map (2D array) to monitor the
+    states of each cell of the chip. The user should input N_dies xor die_w.
+
+    Parameters:
+        chip_w (int or float): The overall width (in um) of the chip.
+        margin (int or float): The width (in um) of the outline of the chip where no device should be placed.
+        N_dies (int): Number of dies/units to be placed by row and column.
+        die_w (None, int, or float): If specified, the width of each die/unit to be placed by row and column.
+        annotations_layer (int or array-like[2]): The layer where to put the device.
+        unpack_chip_map (bool): If True, the function returns a map (2D array) of states to be filled later (e.g., with place_on_chip()).
+        create_devices_map_txt (bool or string): If True or string, the function creates a txt file that will map the devices.
+
+    Returns:
+        Tuple[Device, float, List[List[bool]], str]: A tuple containing from 2 to 4 elements, depending on what needs to be extracted (parameters dependent):
+
+        - **CHIP** (*Device*): The chip map.
+        - **die_w** (*float*): The width of each die. (returned if die_w was None)
+        - **N_dies** (*float*): The number of dies/units on each row and column. (returned if die_w was not None)
+        - **chip_map** (*array-like[N_dies][N_dies] of bool*): A 2D array filled with "Free" (=True) states. (returned if unpack_chip_map is True)
+        - **file_name** (*str*): The name of the created devices map text file. (returned if create_devices_map_txt is not False)
+    """
+
+    CHIP = Device("CHIP ")
+    CHIP.add_polygon(
+        [(0, 0), (chip_w, 0), (chip_w, chip_w), (0, chip_w)], layer=annotations_layer
+    )
+
+    useful_w = chip_w - margin * 2
+    useful_area = CHIP.add_polygon(
+        [(0, 0), (useful_w, 0), (useful_w, useful_w), (0, useful_w)],
+        layer=annotations_layer,
+    )
+    useful_area.move((margin, margin))
+
+    if die_w is not None:
+        N_dies = int(useful_w / die_w)
+        return_N_or_w = N_dies
+    else:
+        die_w = useful_w / N_dies
+        return_N_or_w = die_w
+    CELL = pg.rectangle([die_w, die_w], layer=annotations_layer)
+    array = CHIP.add_array(CELL, columns=N_dies, rows=N_dies, spacing=(die_w, die_w))
+    array.move((0, 0), (margin, margin))
+
+    CHIP.flatten()
+    CHIP.move((margin, margin), (0, 0))
+
+    if create_devices_map_txt:
+        ## create a devices map ...
+        if create_devices_map_txt == True:
+            file_name = "devices map"
+        else:
+            file_name = f"{create_devices_map_txt}"
+
+        # check that file does not already exist, in which case it will add a int to its name:
+        i = 0
+        file_to_find = file_name
+        while True:
+            if i != 0:
+                file_to_find = file_name + f"({i})"
+            file_already_exists = os.path.exists(f"{file_to_find}.txt")
+            i += 1
+            if not file_already_exists:
+                file_name = file_to_find
+                break
+        with open(f"{file_name}.txt", "a") as file:
+            file.write("Devices placed on the chip: \n\n")
+            file.write("(row, col) : device.name\n\n")
+
+        ## ... and return the devices map filename in the outputs
+        if unpack_chip_map:
+            chip_map = [[Free for _ in range(N_dies)] for _ in range(N_dies)]
+            return CHIP, return_N_or_w, chip_map, file_name
+        else:
+            return CHIP, return_N_or_w, file_name
+    else:
+        if unpack_chip_map:
+            chip_map = [[Free for _ in range(N_dies)] for _ in range(N_dies)]
+            return CHIP, return_N_or_w, chip_map
+        else:
+            return CHIP, return_N_or_w
+
+
+def place_on_chip(
+    cell: Device,
+    coordinates: Tuple[int, int],
+    chip_map: List[List[bool]],
+    die_w: Union[int, float],
+    devices_map_txt: Union[None, str] = None,
+) -> bool:
+    """Moves the chip to the coordinates specified.
+
+    Update the chip map with Occupied states where the device has been placed.
+
+    NB: The cell is aligned from its bottom left corner to the coordinates.
+
+    Parameters:
+        cell (Device): Device to be moved.
+        coordinates (tuple of int): (i, j) indices of the chip grid, where to place the cell.
+            Note that the indices start at 0.
+        chip_map (2D array): The 2D array mapping the free cells in the chip map.
+        die_w (int or float): The width of a die/unit in the chip map.
+        devices_map_txt (str or None): Name of the devices map text file to write placement information.
+            If None, no file will be written.
+
+    Returns:
+        bool: False, if the Device falls out of the chip map, prints an error
+        message and does not place the device. True, otherwise.
+
+    Raises:
+        Warning: Prints a warning if the Device is overlapping with already occupied coordinates.
+    """
+
+    # update the chip's availabilities
+    n_cell = round(cell.xsize / die_w)
+    m_cell = round(cell.ysize / die_w)
+    for n in range(n_cell):
+        for m in range(m_cell):
+            cell_name = cell.name.replace("\n", "")
+            try:
+                if chip_map[coordinates[1] + m][coordinates[0] + n] == Occupied:
+                    print(
+                        f"Warning, placing Device {cell_name} "
+                        + f"in an occupied state ({coordinates[1]+m}, {coordinates[0]+n})"
+                    )
+                else:
+                    chip_map[coordinates[1] + m][coordinates[0] + n] = Occupied
+            except IndexError:
+                print(
+                    f"Error, Device {cell_name} "
+                    + f"falls out of the chip map ({coordinates[1]+m}, {coordinates[0]+n})"
+                )
+                return False
+
+    # move the cell
+    cell_bottom_left = (
+        -n_cell * 0.5 * die_w,
+        -m_cell * 0.5 * die_w,
+    )
+    cell.move(cell_bottom_left, ((coordinates[0]) * die_w, (coordinates[1]) * die_w))
+
+    # write the cell's place on the devices map text file
+    if devices_map_txt is not None:
+        with open(f"{devices_map_txt}.txt", "a") as file:
+            try:
+                name = cell.name.replace("\n", "")
+            except AttributeError:
+                name = "unnamed"
+            file.write(f"({coordinates[0]}, {coordinates[1]}) : {name}\n")
+
+    return True
+
+
+def place_remaining_devices(
+    devices_to_place: List[Device],
+    chip_map: List[List[bool]],
+    die_w: Union[int, float],
+    write_devices_map_txt: Union[bool, str] = False,
+) -> Optional[None]:
+    """Go through the chip map and place the devices given, where the chip map
+    is Free.
+
+    Parameters:
+        devices_to_place (list of Device objects): The devices to be placed.
+        chip_map (2D array): The 2D array mapping the free cells in the chip map.
+        die_w (int or float): The width of a die/unit in the chip map.
+        write_devices_map_txt (bool or str): If True, write a .txt file mapping the devices that were placed.
+            If str, specifies the filename of the .txt file.
+
+    Note:
+        The list of devices is not re-ordered to fit as many of them as possible.
+        Some edges of the chip may remain empty because the list contained 2-units long devices (for e.g.).
+    """
+
+    # name and create the file if no file was given
+    if write_devices_map_txt == True:
+
+        file_name = "remaining_cells_map"
+        with open(f"{file_name}.txt", "a") as file:
+            file.write("Remaining devices placed on the chip:\n\n")
+            file.write("(row, col) : device.name\n\n")
+    # use the file's name is a file was given
+    elif write_devices_map_txt:
+        file_name = write_devices_map_txt
+    # pass false if no txt file should be created
+    else:
+        file_name = None
+
+    for row_i, row in enumerate(chip_map):
+        for col_i, status in enumerate(row):
+            if status == Free and devices_to_place:
+                if place_on_chip(
+                    devices_to_place[0], (col_i, row_i), chip_map, die_w, file_name
+                ):
+                    devices_to_place.pop(0)
+
+    if devices_to_place:
+        print(
+            "Some devices are still to be placed, " + "no place remaining on the chip."
+        )
+
+
+class Design:
+    """A class for a design on a single layer of superconducting material, and
+    additional contact pads.
+
+    It is though for a process like:
+
+    - exposing the superconductiong material using e-beam lithography. Two
+      exposures at low and high currents are possible by distinguishing two
+      layers: device layer and die layer. Equivalently, the shapes outlines
+      (though for positive tone resist) have two different widths for the device
+      and die layers.
+    - exposing the pads layer using photolithography.
+
+    Args:
+        name (str): The name of the design.
+        chip_w (int or float): The overall width of the chip.
+        chip_margin (int or float): The width of the outline of the chip where
+            no device should be placed.
+        N_dies (int): Number of dies/units to be placed by row and column.
+        die_w (int or float, optional): Width of a unit die/cell in the design
+            (the output device will be an integer number of unit cells).
+        pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
+        device_outline (int or float): The width of the device's outline.
+        die_outline (int or float): The width of the pads outline.
+        ebeam_overlap (int or float): Extra length of the routes above the die's
+            ports to assure alignment with the device (useful for ebeam
+            lithography).
+        annotation_layer (int): The layer where to put the annotations.
+        device_layer (int or array-like[2]): The layer where the device is placed.
+        die_layer (int or array-like[2]): The layer where the die is placed.
+        pad_layer (int or array-like[2]): The layer where the pads are placed.
+        fill_pad_layer (bool): If True, the space reserved for pads in the
+            die_cell in filled in pad's layer.
+
+    Example:
+        Here is an example of how to create the class.
+
+        >>> # Choose some design parameters, let the others to default
+        >>> chip_w = 10000
+        >>> N_dies = 11
+        >>> device_outline = 0.3
+        >>> die_outline = 10
+
+        >>> # Create the design and initialize the chip
+        >>> demo_project = Design(name="demo design",
+        >>>                       chip_w=chip_w,
+        >>>                       N_dies=N_dies,
+        >>>                       device_outline=device_outline,
+        >>>                       die_outline=die_outline)
+        >>> demo_project.create_chip()
+
+        >>> # Quickplot the chip skeletton!
+        >>> qp(demo_project.CHIP)
+    """
+
+    def __init__(
+        self,
+        name="new_design",
+        chip_w=dflt.chip_w,
+        chip_margin=dflt.chip_margin,
+        N_dies=dflt.auto_param,
+        die_w=dflt.die_w,
+        pad_size=dflt.pad_size,
+        device_outline=dflt.device_outline,
+        die_outline=dflt.die_outline,
+        ebeam_overlap=dflt.ebeam_overlap,
+        annotation_layer=dflt.layers["annotation"],
+        device_layer=dflt.layers["device"],
+        die_layer=dflt.layers["die"],
+        pad_layer=dflt.layers["pad"],
+        fill_pad_layer=False,
+    ):
+        """
+        Args:
+            name (str): The name of the design.
+            chip_w (int or float): The overall width of the chip.
+            chip_margin (int or float): The width of the outline of the chip where no device should be placed.
+            N_dies (int): Number of dies/units to be placed by row and column.
+            die_w (int or float, optional): Width of a unit die/cell in the
+                design (the output device will be an integer number of unit cells).
+            pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
+            device_outline (int or float): The width of the device's outline.
+            die_outline (int or float): The width of the pads outline.
+            ebeam_overlap (int or float): Extra length of the routes above the
+                die's ports to assure alignment with the device (useful for ebeam
+                lithography).
+            annotation_layer (int): The layer where to put the annotations.
+            device_layer (int or array-like[2]): The layer where the device is placed.
+            die_layer (int or array-like[2]): The layer where the die is placed.
+            pad_layer (int or array-like[2]): The layer where the pads are placed.
+            fill_pad_layer (bool): If True, the space reserved for pads in the
+                die_cell in filled in pad's layer.
+        """
+
+        self.name = name
+
+        self.chip_w = chip_w
+        self.chip_margin = chip_margin
+        self.N_dies = N_dies
+        self.die_w = die_w
+
+        self.pad_size = pad_size
+        self.device_outline = device_outline
+        self.die_outline = die_outline
+        self.ebeam_overlap = ebeam_overlap
+
+        self.layers = {
+            "annotation": annotation_layer,
+            "device": device_layer,
+            "die": die_layer,
+            "pad": pad_layer,
+        }
+
+        self.fill_pad_layer = fill_pad_layer
+
+    # help building a design
+
+    def create_chip(self, create_devices_map_txt: Union[bool, str] = True) -> Device:
+        """Creates the chip, with unit cells.
+
+        The CHIP created will be the foundation of the design, the Device to add
+        all references to. The function creates a chip_map (2D array) to help placing
+        the cells on the chip (aligned with the unit cells). The function also generates
+        a txt file if create_devices_map_txt is True to follow the devices placements
+        on the chip.
+
+        Parameters:
+            create_devices_map_txt (bool or str): If True, generates a text file
+                to follow the devices placements on the chip. If string, the text file
+                is named after the string.
+
+        Returns:
+            CHIP (Device): The chip map, in the annotations layer
+        """
+        if create_devices_map_txt:
+            if create_devices_map_txt == True:
+                create_devices_map_txt = f"{self.name} devices map"
+            else:
+                create_devices_map_txt = f"{create_devices_map_txt}"
+            self.CHIP, N_or_w, self.chip_map, self.devices_map_txt = create_chip(
+                chip_w=self.chip_w,
+                margin=self.chip_margin,
+                N_dies=self.N_dies,
+                die_w=self.die_w,
+                annotations_layer=self.layers["annotation"],
+                unpack_chip_map=True,
+                create_devices_map_txt=create_devices_map_txt,
+            )
+        else:
+            self.devices_map_txt = None
+            create_devices_map_txt = False
+            self.CHIP, N_or_w, self.chip_map = create_chip(
+                chip_w=self.chip_w,
+                margin=self.chip_margin,
+                N_dies=self.N_dies,
+                die_w=self.die_w,
+                annotations_layer=self.layers["annotation"],
+                unpack_chip_map=True,
+                create_devices_map_txt=create_devices_map_txt,
+            )
+
+        if self.die_w is not None:
+            self.N_dies = N_or_w
+        else:
+            self.die_w = N_or_w
+
+        return self.CHIP
+
+    def place_on_chip(
+        self, cell: Device, coordinates: Tuple[int, int], add_to_chip: bool = True
+    ) -> bool:
+        """Moves the chip to the coordinates specified. Update the chip map
+        with Occupied states where the device has been placed.
+
+        NB: the cell is aligned from its bottom left corner to the coordinates.
+
+        Parameters:
+            cell (Device): Device to be moved.
+            coordinates (tuple of int): (i, j) indices of the chip grid, where to place the cell.
+                Note that the indices start at 0.
+
+        Returns:
+            bool: False, if the Device falls out of the chip map, prints an error message and does not place the device. True, otherwise.
+
+        Raises:
+            Warning: Prints a warning if the Device is overlapping with already occupied coordinates.
+
+        Examples:
+            Here is an example of placing alignment cells on two given positions of the chip.
+
+            >>> align_left  = demo_project.create_alignment_cell(layers_to_align=[2, 3])
+            >>> align_right = demo_project.create_alignment_cell(layers_to_align=[2, 3])
+            >>> demo_project.place_on_chip(cell=align_left,  coordinates=(0, 5))
+            >>> demo_project.place_on_chip(cell=align_right, coordinates=(10, 5))
+        """
+
+        if add_to_chip:
+            self.CHIP << cell
+        return place_on_chip(
+            cell=cell,
+            coordinates=coordinates,
+            chip_map=self.chip_map,
+            die_w=self.die_w,
+            devices_map_txt=self.devices_map_txt,
+        )
+
+    def place_remaining_devices(
+        self,
+        devices_to_place: List[Device],
+        add_to_chip: bool = True,
+        write_remaining_devices_map_txt: Union[bool, str] = False,
+    ) -> Optional[None]:
+        """Go through the chip map and place the devices given, where the chip
+        map is Free.
+
+        Parameters:
+            devices_to_place (list of Device objects): The devices to be placed.
+            add_to_chip (bool): Add the devices provided to the Design's CHIP.
+            write_remaining_devices_map_txt (bool or string): If True, write a .txt
+                file mapping the devices that were placed. If string, the filename is
+                the given string, except if a file has already been created.
+
+        Note:
+            The list of devices is not re-ordered to fit as many of them as possible.
+            Some edges of the chip may remain empty because the list contained 2-units long devices (for e.g.).
+
+        Examples:
+            Here is a typical example of why this function is useful and how to
+            use it. If design is a Design class initalized, and the
+            create_chip() function has previously been executed.
+
+            >>> channels_w = [0.5, 0.75, 1, 1.25, 1.5]
+            >>> ntrons_to_place = []
+            >>> for channel_w in channels_w:
+            >>>     ntron = design.create_ntron_cell(choke_w=0.05, channel_w=channel_w)
+            >>>     ntrons_to_place.append(ntron)
+            >>> design.place_remaining_cells(ntrons_to_place)
+        """
+        if self.devices_map_txt is not None:
+            # the decision taken when creating the chip overwrites this one
+            write_devices_map_txt = self.devices_map_txt
+        else:
+            # a devices map can still be created, as decided when calling this function
+            write_devices_map_txt = write_remaining_devices_map_txt
+
+        if add_to_chip:
+            self.CHIP << devices_to_place
+        place_remaining_devices(
+            devices_to_place=devices_to_place,
+            chip_map=self.chip_map,
+            die_w=self.die_w,
+            write_devices_map_txt=write_devices_map_txt,
+        )
+
+    def write_gds(self, text: Union[None, str] = dflt.text) -> Union[None, str]:
+        """Write a GDS file.
+
+        Args:
+            text (str or None): The filename for the GDS file.
+                If None, the name of the Design will be used.
+
+        Returns:
+            str or None: The filename of the written GDS file, or None if no file was written.
+        """
+        if text is None:
+            text = self.name
+        return self.CHIP.write_gds(filename=f"{text}.gds", max_cellname_length=32000)
+
+    # basics:
+
+    def alignment_cell(
+        self, layers_to_align: List[int], text: Union[None, str] = dflt.text
+    ) -> Device:
+        """Creates alignment marks in an integer number of unit cells.
+
+        Parameters:
+            layers_to_align (List[int]): Layers to align.
+            text (str, optional): If None, the text is f"lay={layers_to_align}".
+
+        Returns:
+            Device: A device that centers the alignment marks in an n*m unit cell.
+        """
+        return cell.alignment(
+            die_w=self.die_w,
+            layers_to_align=layers_to_align,
+            outline_die=self.die_outline,
+            die_layer=self.layers["die"],
+            text=text,
+        )
+
+    def vdp_cell(
+        self,
+        layers_to_probe: List[int],
+        layers_to_outline: Union[List[int], None] = dflt.auto_param,
+        text: Union[None, str] = dflt.text,
+    ) -> Device:
+        r"""Creates a cell containing a Van Der Pauw structure between 4 contact
+        pads.
+
+        Parameters:
+            layers_to_probe (List[int]): The layers on which to place the VDP structure.
+            layers_to_outline (List[int]): Among the VDP layers, the ones for which structure must not be filled but outlined.
+            text (str, optional): If None, the text is f"lay={layers_to_probe}".
+
+        Returns:
+            Device: The created device.
+        """
+
+        return cell.vdp(
+            die_w=self.die_w,
+            pad_size=self.pad_size,
+            layers_to_probe=layers_to_probe,
+            layers_to_outline=layers_to_outline,
+            outline=self.die_outline,
+            die_layer=self.layers["die"],
+            pad_layer=self.layers["pad"],
+            text=text,
+        )
+
+    def etch_test_cell(
+        self, layers_to_etch: List[List[int]], text: Union[None, str] = dflt.text
+    ) -> Device:
+        """Creates etch test structures in an integer number of unit cells.
+
+        These test structures are thought to be used by probing on pads (with a simple multimeter)
+        that should be isolated one from another if the etching is complete.
+
+        Parameters:
+            layers_to_etch (List[List[int]]): Each element of the list corresponds to one test point,
+                to put on the list of layers specified. Example: [[1, 2], [1], [2]].
+            text (str, optional): If None, the text is f"lay={layers_to_etch}".
+
+        Returns:
+            Device: A device (with size n*m of unit cells) with etch tests in its center.
+        """
+
+        return cell.etch_test(
+            die_w=self.die_w,
+            layers_to_etch=layers_to_etch,
+            outline_die=self.die_outline,
+            die_layer=self.layers["die"],
+            text=text,
+        )
+
+    def resolution_test_cell(
+        self,
+        layer_to_resolve: int,
+        resolutions_to_test: List[float] = [
+            0.025,
+            0.05,
+            0.075,
+            0.1,
+            0.25,
+            0.5,
+            1,
+            1.5,
+            2,
+        ],
+        text: Union[None, str] = dflt.text,
+    ) -> Device:
+        r"""Creates a cell containing a resolution test.
+
+        Parameters:
+            layer_to_resolve (int): The layer to put the resolution test on.
+            resolutions_to_test (List[float]): The resolutions to test in µm.
+            text (str, optional): If None, the text is f"lay={layer_to_resolve}".
+
+        Returns:
+            Device: The created device.
+        """
+
+        return cell.resolution_test(
+            die_w=self.die_w,
+            layer_to_resolve=layer_to_resolve,
+            resolutions_to_test=resolutions_to_test,
+            outline=self.die_outline,
+            die_layer=self.layers["die"],
+            text=text,
+        )
+
+    # devices:
+
+    def nanowires_cell(
+        self,
+        channels_sources_w: List[Tuple[float, float]],
+        text: Union[None, str] = dflt.text,
+    ) -> Device:
+        """Creates a cell containing several nanowires of given channel and
+        source.
+
+        Parameters:
+            channels_sources_w (List[Tuple[float, float]]): The list of
+                (channel_w, source_w) of the nanowires to create.
+            text (str, optional): If None, the text is f"w={channels_w}".
+
+        Returns:
+            Device: A device containing the nanowires, the border of the die
+            (created with die_cell function), and the connections between the
+            nanowires and pads.
+        """
+
+        return cell.nanowires(
+            die_w=self.die_w,
+            pad_size=self.pad_size,
+            channels_sources_w=channels_sources_w,
+            overlap_w=self.ebeam_overlap,
+            outline_die=self.die_outline,
+            outline_dev=self.device_outline,
+            device_layer=self.layers["device"],
+            die_layer=self.layers["die"],
+            pad_layer=self.layers["pad"],
+            text=text,
+            fill_pad_layer=self.fill_pad_layer,
+        )
+
+    def ntron_cell(
+        self,
+        choke_w: float,
+        channel_w: float,
+        gate_w: Union[float, None] = dflt.auto_param,
+        source_w: Union[float, None] = dflt.auto_param,
+        drain_w: Union[float, None] = dflt.auto_param,
+        choke_shift: Union[float, None] = dflt.auto_param,
+        text: Union[str, None] = dflt.text,
+    ) -> Device:
+        r"""Creates a standardized cell specifically for a single ntron.
+
+        Unless specified, scales the ntron parameters as:
+        gate_w = drain_w = source_w = 3*channel_w
+        choke_shift = -3*channel_w
+
+        Parameters:
+            choke_w (int or float): The width of the ntron's choke in µm.
+            channel_w (int or float): The width of the ntron's channel in µm.
+            gate_w (int or float, optional): If None, gate width is 3 times the channel width.
+            source_w (int or float, optional): If None, source width is 3 times the channel width.
+            drain_w (int or float, optional): If None, drain width is 3 times the channel width.
+            choke_shift (int or float, optional): If None, choke shift is -3 times the channel width.
+            text (str, optional): If None, the text is f"chk: {choke_w} \\nchnl: {channel_w}".
+
+        Returns:
+            Device: A device containing the ntron, the border of the die (created with die_cell function),
+            and the connections between the ports.
+        """
+
+        return cell.ntron(
+            die_w=self.die_w,
+            pad_size=self.pad_size,
+            choke_w=choke_w,
+            channel_w=channel_w,
+            gate_w=gate_w,
+            source_w=source_w,
+            drain_w=drain_w,
+            choke_shift=choke_shift,
+            overlap_w=self.ebeam_overlap,
+            outline_die=self.die_outline,
+            outline_dev=self.device_outline,
+            device_layer=self.layers["device"],
+            die_layer=self.layers["die"],
+            pad_layer=self.layers["pad"],
+            text=text,
+            fill_pad_layer=self.fill_pad_layer,
+        )
+
+    def snspds_cell(
+        self,
+        snspds_width_pitch: List[Tuple[float, float]] = [(0.2, 0.6)],
+        snspd_size: Tuple[Union[int, float], Union[int, float]] = (100, 100),
+        snspd_num_squares: Optional[int] = None,
+        text: Union[None, str] = dflt.text,
+    ) -> Device:
+        """Creates a cell that contains vertical superconducting nanowire
+        single-photon detectors (SNSPD).
+
+        Parameters:
+
+            snspds_width_pitch (list of tuple of float): list of (width, pitch) of the nanowires.
+            snspd_size (tuple of int or float): Size of the detectors in squares (width, height).
+            snspd_num_squares (Optional[int]): Number of squares in the detectors.
+            text (string, optional): If None, the text is f"w={snspds_width}".
+
+        Returns:
+            Device: A cell (of size n*m unit die_cells) containing the SNSPDs.
+        """
+
+        return cell.snspds(
+            die_w=self.die_w,
+            pad_size=self.pad_size,
+            snspds_width_pitch=snspds_width_pitch,
+            snspd_size=snspd_size,
+            snspd_num_squares=snspd_num_squares,
+            overlap_w=self.ebeam_overlap,
+            outline_die=self.die_outline,
+            outline_dev=self.device_outline,
+            device_layer=self.layers["device"],
+            die_layer=self.layers["die"],
+            pad_layer=self.layers["pad"],
+            text=text,
+            fill_pad_layer=self.fill_pad_layer,
+        )
+
+    def snspd_ntron_cell(
+        self,
+        w_choke: float,
+        w_snspd: Union[float, None] = dflt.auto_param,
+        text: Union[str, None] = dflt.text,
+    ) -> Device:
+        """Creates a cell that contains an SNSPD coupled to an NTRON. The
+        device's parameters are sized according to the SNSPD's width and the
+        NTRON's choke.
+
+        Parameters:
+            w_choke (int or float): The width of the NTRON choke in µm.
+            w_snspd (int or float, optional): The width of the SNSPD nanowire in µm. If None, scaled to 5*w_choke.
+            text (string, optional): If None, the text is f"w={w_snspd}, {w_choke}".
+
+        Returns:
+            Device: A cell containing a die in die_layer, pads in pad layer, and an SNSPD-NTRON properly routed in the device layer.
+        """
+
+        return cell.snspd_ntron(
+            die_w=self.die_w,
+            pad_size=self.pad_size,
+            w_choke=w_choke,
+            w_snspd=w_snspd,
+            overlap_w=self.ebeam_overlap,
+            outline_die=self.die_outline,
+            outline_dev=self.device_outline,
+            device_layer=self.layers["device"],
+            die_layer=self.layers["die"],
+            pad_layer=self.layers["pad"],
+            text=text,
+            fill_pad_layer=self.fill_pad_layer,
+        )
```

### Comparing `qnngds-2.4.1/src/qnngds/devices/nanowire.py` & `qnngds-2.5.0/src/qnngds/devices/nanowire.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-"""Single nanowire constriction."""
-
-from phidl import Device
-
-import phidl.geometry as pg
-from typing import Tuple, Optional
-import qnngds._default_param as dflt
-
-
-def spot(
-    channel_w: float = 0.1,
-    source_w: float = 0.3,
-    layer: int = dflt.layers["device"],
-    num_pts: int = 100,
-) -> Device:
-    """Creates a single wire, made of two optimal steps from channel_w to
-    source_w.
-
-    Args:
-        channel_w (int or float): The width of the channel (at the hot-spot location).
-        source_w (int or float): The width of the nanowire's "source".
-        layer (int): The layer where to put the device.
-        num_pts (int): The number of points comprising the optimal_steps geometries.
-
-    Returns:
-        Device: A device containing 2 optimal steps joined at their channel_w end.
-    """
-
-    NANOWIRE = Device()
-    wire = pg.optimal_step(channel_w, source_w, symmetric=True, num_pts=num_pts)
-    source = NANOWIRE << wire
-    gnd = NANOWIRE << wire
-    source.connect(source.ports[1], gnd.ports[1])
-
-    NANOWIRE = pg.union(NANOWIRE, layer=layer)
-    NANOWIRE.add_port(name=1, port=source.ports[2])
-    NANOWIRE.add_port(name=2, port=gnd.ports[2])
-    NANOWIRE.rotate(-90)
-    NANOWIRE.move(NANOWIRE.center, (0, 0))
-    NANOWIRE.name = f"NANOWIRE.SPOT(w={channel_w})"
-
-    return NANOWIRE
+"""Single nanowire constriction."""
+
+from phidl import Device
+
+import phidl.geometry as pg
+from typing import Tuple, Optional
+import qnngds._default_param as dflt
+
+
+def spot(
+    channel_w: float = 0.1,
+    source_w: float = 0.3,
+    layer: int = dflt.layers["device"],
+    num_pts: int = 100,
+) -> Device:
+    """Creates a single wire, made of two optimal steps from channel_w to
+    source_w.
+
+    Args:
+        channel_w (int or float): The width of the channel (at the hot-spot location).
+        source_w (int or float): The width of the nanowire's "source".
+        layer (int): The layer where to put the device.
+        num_pts (int): The number of points comprising the optimal_steps geometries.
+
+    Returns:
+        Device: A device containing 2 optimal steps joined at their channel_w end.
+    """
+
+    NANOWIRE = Device()
+    wire = pg.optimal_step(channel_w, source_w, symmetric=True, num_pts=num_pts)
+    source = NANOWIRE << wire
+    gnd = NANOWIRE << wire
+    source.connect(source.ports[1], gnd.ports[1])
+
+    NANOWIRE = pg.union(NANOWIRE, layer=layer)
+    NANOWIRE.add_port(name=1, port=source.ports[2])
+    NANOWIRE.add_port(name=2, port=gnd.ports[2])
+    NANOWIRE.rotate(-90)
+    NANOWIRE.move(NANOWIRE.center, (0, 0))
+    NANOWIRE.name = f"NANOWIRE.SPOT(w={channel_w})"
+
+    return NANOWIRE
```

### Comparing `qnngds-2.4.1/src/qnngds/devices/ntron.py` & `qnngds-2.5.0/src/qnngds/devices/ntron.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-"""Nanocryotron `[1] <https://doi.org/10.1021/nl502629x>`_ variants."""
-
-from phidl import Device
-
-import phidl.geometry as pg
-from typing import Tuple, Optional
-import qnngds._default_param as dflt
-
-
-def smooth(
-    choke_w: float = 0.03,
-    gate_w: float = 0.2,
-    channel_w: float = 0.1,
-    source_w: float = 0.3,
-    drain_w: float = 0.3,
-    choke_shift: float = -0.3,
-    layer: int = dflt.layers["device"],
-) -> Device:
-    """Creates a ntron device.
-
-    Args:
-        choke_w (float): Width of the choke region.
-        gate_w (float): Width of the gate region.
-        channel_w (float): Width of the channel region.
-        source_w (float): Width of the source region.
-        drain_w (float): Width of the drain region.
-        choke_shift (float): Shift of the choke region.
-        layer (int): Layer for the device to be created on.
-
-    Returns:
-        Device: The ntron device.
-    """
-
-    D = Device()
-
-    choke = pg.optimal_step(gate_w, choke_w, symmetric=True, num_pts=100)
-    k = D << choke
-
-    channel = pg.compass(size=(channel_w, choke_w))
-    c = D << channel
-    c.connect(channel.ports["W"], choke.ports[2])
-
-    drain = pg.optimal_step(drain_w, channel_w)
-    d = D << drain
-    d.connect(drain.ports[2], c.ports["N"])
-
-    source = pg.optimal_step(channel_w, source_w)
-    s = D << source
-    s.connect(source.ports[1], c.ports["S"])
-
-    k.movey(choke_shift)
-
-    D = pg.union(D)
-    D.flatten(single_layer=layer)
-    D.add_port(name=3, port=k.ports[1])
-    D.add_port(name=1, port=d.ports[1])
-    D.add_port(name=2, port=s.ports[2])
-    D.name = f"NTRON.SMOOTH(choke_w={choke_w}, channel_w={channel_w})"
-    D.info = locals()
-
-    return D
-
-
-def sharp(
-    choke_w: float = 0.03,
-    choke_l: float = 0.5,
-    gate_w: float = 0.2,
-    channel_w: float = 0.1,
-    source_w: float = 0.3,
-    drain_w: float = 0.3,
-    layer: int = dflt.layers["device"],
-) -> Device:
-    """Creates a sharp ntron device.
-
-    Args:
-        choke_w (float): Width of the choke region.
-        choke_l (float): Length of the choke region.
-        gate_w (float): Width of the gate region.
-        channel_w (float): Width of the channel region.
-        source_w (float): Width of the source region.
-        drain_w (float): Width of the drain region.
-        layer (int): Layer for the device to be created on.
-
-    Returns:
-        Device: The sharp ntron device.
-    """
-
-    D = Device()
-
-    choke = pg.taper(choke_l, gate_w, choke_w)
-    k = D << choke
-
-    channel = pg.compass(size=(channel_w, choke_w / 10))
-    c = D << channel
-    c.connect(channel.ports["W"], choke.ports[2])
-
-    drain = pg.taper(channel_w * 6, drain_w, channel_w)
-    d = D << drain
-    d.connect(drain.ports[2], c.ports["N"])
-
-    source = pg.taper(channel_w * 6, channel_w, source_w)
-    s = D << source
-    s.connect(source.ports[1], c.ports["S"])
-
-    D = pg.union(D)
-    D.flatten(single_layer=layer)
-    D.add_port(name="g", port=k.ports[1])
-    D.add_port(name="d", port=d.ports[1])
-    D.add_port(name="s", port=s.ports[2])
-    D.name = f"NTRON.SHARP(choke_w={choke_w}, channel_w={channel_w})"
-    D.info = locals()
-    return D
+"""Nanocryotron `[1] <https://doi.org/10.1021/nl502629x>`_ variants."""
+
+from phidl import Device
+
+import phidl.geometry as pg
+from typing import Tuple, Optional
+import qnngds._default_param as dflt
+
+
+def smooth(
+    choke_w: float = 0.03,
+    gate_w: float = 0.2,
+    channel_w: float = 0.1,
+    source_w: float = 0.3,
+    drain_w: float = 0.3,
+    choke_shift: float = -0.3,
+    layer: int = dflt.layers["device"],
+) -> Device:
+    """Creates a ntron device.
+
+    Args:
+        choke_w (float): Width of the choke region.
+        gate_w (float): Width of the gate region.
+        channel_w (float): Width of the channel region.
+        source_w (float): Width of the source region.
+        drain_w (float): Width of the drain region.
+        choke_shift (float): Shift of the choke region.
+        layer (int): Layer for the device to be created on.
+
+    Returns:
+        Device: The ntron device.
+    """
+
+    D = Device()
+
+    choke = pg.optimal_step(gate_w, choke_w, symmetric=True, num_pts=100)
+    k = D << choke
+
+    channel = pg.compass(size=(channel_w, choke_w))
+    c = D << channel
+    c.connect(channel.ports["W"], choke.ports[2])
+
+    drain = pg.optimal_step(drain_w, channel_w)
+    d = D << drain
+    d.connect(drain.ports[2], c.ports["N"])
+
+    source = pg.optimal_step(channel_w, source_w)
+    s = D << source
+    s.connect(source.ports[1], c.ports["S"])
+
+    k.movey(choke_shift)
+
+    D = pg.union(D)
+    D.flatten(single_layer=layer)
+    D.add_port(name=3, port=k.ports[1])
+    D.add_port(name=1, port=d.ports[1])
+    D.add_port(name=2, port=s.ports[2])
+    D.name = f"NTRON.SMOOTH(choke_w={choke_w}, channel_w={channel_w})"
+    D.info = locals()
+
+    return D
+
+
+def sharp(
+    choke_w: float = 0.03,
+    choke_l: float = 0.5,
+    gate_w: float = 0.2,
+    channel_w: float = 0.1,
+    source_w: float = 0.3,
+    drain_w: float = 0.3,
+    layer: int = dflt.layers["device"],
+) -> Device:
+    """Creates a sharp ntron device.
+
+    Args:
+        choke_w (float): Width of the choke region.
+        choke_l (float): Length of the choke region.
+        gate_w (float): Width of the gate region.
+        channel_w (float): Width of the channel region.
+        source_w (float): Width of the source region.
+        drain_w (float): Width of the drain region.
+        layer (int): Layer for the device to be created on.
+
+    Returns:
+        Device: The sharp ntron device.
+    """
+
+    D = Device()
+
+    choke = pg.taper(choke_l, gate_w, choke_w)
+    k = D << choke
+
+    channel = pg.compass(size=(channel_w, choke_w / 10))
+    c = D << channel
+    c.connect(channel.ports["W"], choke.ports[2])
+
+    drain = pg.taper(channel_w * 6, drain_w, channel_w)
+    d = D << drain
+    d.connect(drain.ports[2], c.ports["N"])
+
+    source = pg.taper(channel_w * 6, channel_w, source_w)
+    s = D << source
+    s.connect(source.ports[1], c.ports["S"])
+
+    D = pg.union(D)
+    D.flatten(single_layer=layer)
+    D.add_port(name="g", port=k.ports[1])
+    D.add_port(name="d", port=d.ports[1])
+    D.add_port(name="s", port=s.ports[2])
+    D.name = f"NTRON.SHARP(choke_w={choke_w}, channel_w={channel_w})"
+    D.info = locals()
+    return D
```

### Comparing `qnngds-2.4.1/src/qnngds/geometries.py` & `qnngds-2.5.0/src/qnngds/geometries.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-"""Geometries contains useful shapes/tools that are not available in phidl's
-geometry library."""
-
-from phidl import Device
-import numpy as np
-import qnngds._default_param as dflt
-
-
-def hyper_taper(
-    length=10, wide_section=50, narrow_section=5, layer=dflt.layers["device"]
-):
-    """Hyperbolic taper (solid). Designed by colang.
-
-    Args:
-        length (float): Length of taper.
-        wide_section (float): Wide width dimension.
-        narrow_section (float): Narrow width dimension.
-        layer (int): Layer for device to be created on.
-
-    Returns:
-        Device: The hyper taper.
-    """
-
-    taper_length = length
-    wide = wide_section
-    zero = 0
-    narrow = narrow_section
-    x_list = np.arange(0, taper_length + 0.1, 0.1)
-    x_list2 = np.arange(taper_length, -0.1, -0.1)
-    pts = []
-
-    a = np.arccosh(wide / narrow) / taper_length
-
-    for x in x_list:
-        pts.append((x, np.cosh(a * x) * narrow / 2))
-    for y in x_list2:
-        pts.append((y, -np.cosh(a * y) * narrow / 2))
-        HT = Device("hyper_taper")
-        hyper_taper = HT.add_polygon(pts)
-        HT.add_port(name=1, midpoint=[0, 0], width=narrow, orientation=180)
-        HT.add_port(name=2, midpoint=[taper_length, 0], width=wide, orientation=0)
-        HT.flatten(single_layer=layer)
-    return HT
+"""Geometries contains useful shapes/tools that are not available in phidl's
+geometry library."""
+
+from phidl import Device
+import numpy as np
+import qnngds._default_param as dflt
+
+
+def hyper_taper(
+    length=10, wide_section=50, narrow_section=5, layer=dflt.layers["device"]
+):
+    """Hyperbolic taper (solid). Designed by colang.
+
+    Args:
+        length (float): Length of taper.
+        wide_section (float): Wide width dimension.
+        narrow_section (float): Narrow width dimension.
+        layer (int): Layer for device to be created on.
+
+    Returns:
+        Device: The hyper taper.
+    """
+
+    taper_length = length
+    wide = wide_section
+    zero = 0
+    narrow = narrow_section
+    x_list = np.arange(0, taper_length + 0.1, 0.1)
+    x_list2 = np.arange(taper_length, -0.1, -0.1)
+    pts = []
+
+    a = np.arccosh(wide / narrow) / taper_length
+
+    for x in x_list:
+        pts.append((x, np.cosh(a * x) * narrow / 2))
+    for y in x_list2:
+        pts.append((y, -np.cosh(a * y) * narrow / 2))
+        HT = Device("hyper_taper")
+        hyper_taper = HT.add_polygon(pts)
+        HT.add_port(name=1, midpoint=[0, 0], width=narrow, orientation=180)
+        HT.add_port(name=2, midpoint=[taper_length, 0], width=wide, orientation=0)
+        HT.flatten(single_layer=layer)
+    return HT
```

### Comparing `qnngds-2.4.1/src/qnngds/tests.py` & `qnngds-2.5.0/src/qnngds/tests.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,266 +1,266 @@
-"""Tests contains common test structures for following/characterizing a
-fabrication process and its effect on the materials."""
-
-from phidl import Device
-import phidl.geometry as pg
-from typing import List, Union
-import qnngds._default_param as dflt
-
-
-def alignment_mark(layers: List[int] = [1, 2, 3, 4]) -> Device:
-    """Creates an alignment mark for each photolithography.
-
-    Args:
-        layers (List[int]): An array of layers.
-
-    Returns:
-        Device: A device containing the alignment marks on each layer.
-    """
-
-    def create_marker(layer1, layer2):
-
-        MARK = Device()
-
-        # central part with cross
-
-        CROSS = Device("CROSS")
-        cross = CROSS << pg.union(pg.cross(length=190, width=20), layer=layer1)
-        rect = pg.rectangle((65, 65), layer=layer2)
-        window = CROSS.add_array(rect, 2, 2, (125, 125))
-        window.move(window.center, cross.center)
-        MARK << CROSS.flatten()
-
-        # combs
-        def create_comb(pitch1=500, pitch2=100, layer1=1, layer2=2):
-
-            COMB = Device()
-
-            # middle comb (made of layer1), pitch = 10
-            rect1 = pg.rectangle((5, 30), layer=layer1)
-            middle_comb = COMB.add_array(rect1, 21, 1, spacing=(10, 0))
-            middle_comb.move(COMB.center, (0, 0))
-
-            # top and bottom combs (made of layer2), pitchs = 10+pitch1, 10+pitch2
-            rect2 = pg.rectangle((5, 30), layer=layer2)
-            top_comb = COMB.add_array(rect2, 21, 1, spacing=(10 + pitch1 / 1000, 0))
-            top_comb.move(
-                top_comb.center, (middle_comb.center[0], middle_comb.center[1] + 30)
-            )
-            top_text = COMB.add_ref(pg.text(f"{pitch1}NM", size=10, layer=layer2))
-            top_text.move(top_text.center, (140, 30))
-
-            bottom_comb = COMB.add_array(rect2, 21, 1, spacing=(10 + pitch2 / 1000, 0))
-            bottom_comb.move(
-                bottom_comb.center, (middle_comb.center[0], middle_comb.center[1] - 30)
-            )
-            bottom_text = COMB.add_ref(pg.text(f"{pitch2}NM", size=10, layer=layer2))
-            bottom_text.move(bottom_text.center, (140, -30))
-
-            # additional markers (made of layer1), for clarity
-            rect1a = pg.rectangle((5, 20), layer=layer1)
-            marksa = COMB.add_array(rect1a, 3, 2, spacing=(100, 110))
-            marksa.move(marksa.center, middle_comb.center)
-
-            rect1b = pg.rectangle((5, 10), layer=layer1)
-            marksb = COMB.add_array(rect1b, 2, 2, spacing=(100, 100))
-            marksb.move(marksb.center, middle_comb.center)
-
-            return COMB
-
-        VERNIER = Device("VERNIER(500, 200, 100, 50)")
-        comb51 = create_comb(pitch1=500, pitch2=100, layer1=layer1, layer2=layer2)
-
-        top = VERNIER.add_ref(comb51)
-        top.move((0, 0), (0, 200))
-
-        left = VERNIER.add_ref(comb51)
-        left.rotate(90)
-        left.move((0, 0), (-200, 0))
-
-        comb205 = create_comb(pitch1=200, pitch2=50, layer1=layer1, layer2=layer2)
-
-        bottom = VERNIER.add_ref(comb205)
-        bottom.rotate(180)
-        bottom.move((0, 0), (0, -200))
-
-        right = VERNIER.add_ref(comb205)
-        right.rotate(-90)
-        right.move((0, 0), (200, 0))
-        MARK << VERNIER.flatten()
-
-        MARK.move(MARK.center, (0, 0))
-
-        # text
-        TEXT = Device(f"TEXT({layer2} ON {layer1})")
-        text1 = TEXT << pg.text(str(layer2), size=50, layer={layer1, layer2})
-        text1.move(text1.center, (220, 200))
-        text2 = TEXT << pg.text(f"{layer2} ON {layer1}", size=10, layer=layer2)
-        text2.move(text2.center, (220, 240))
-        MARK << TEXT.flatten()
-
-        MARK.name = f"ALIGN {layer2} ON {layer1}"
-        return MARK
-
-    ALIGN = Device("ALIGN ")
-    markers_pitch = 600
-    for i, layer1 in enumerate(layers):
-        n = len(layers) - i - 1
-        if n != 0:
-            for j, layer2 in enumerate(layers[-n:]):
-                MARK = create_marker(layer1, layer2)
-                MARK.move((j * markers_pitch, i * markers_pitch))
-                ALIGN << MARK
-            text = pg.text(str(layer1), size=160, layer=layer1)
-            text.name = f"TEXT({str(layer1)})"
-            text.move(text.center, (-340, i * markers_pitch))
-            ALIGN << text
-
-    num_layers = len(layers)
-    offset = -(num_layers - 2) * markers_pitch / 2
-    ALIGN.move((0, 0), (offset, offset))
-    return ALIGN
-
-
-def resolution_test(
-    resolutions: List[float] = [0.8, 1, 1.2, 1.4, 1.6, 1.8, 2.0],
-    inverted: Union[bool, float] = False,
-    layer: int = dflt.layers["device"],
-) -> Device:
-    """Creates test structures for determining a process resolution.
-
-    Args:
-        resolutions (List[float]): List of resolutions (in µm) to be tested.
-        inverted (Union[bool, float]): If True, invert the device. If float, outline the device by this width.
-        layer (int): Layer to put the device on.
-
-    Returns:
-        Device: The test structures, in the specified layer.
-    """
-
-    def create_3L(res=1):
-
-        LLL = Device()
-
-        def create_L(w, spacing):
-
-            L = Device()
-
-            bar = pg.rectangle((min(100 * w, 100), w))
-            bars = Device()
-            bars.add_array(bar, 1, 5, spacing=(0, spacing))
-            v_bars = L << bars
-            h_bars = L << bars
-            h_bars.rotate(90)
-
-            L.align("all", "xmin")
-            L.move((L.xmin, L.ymin), (0, 0))
-            return L
-
-        grid_spacing = (13 * res, 13 * res)
-
-        space = [0.8, 1, 1.2]
-        for i, percent in enumerate(space):
-            lll = LLL << create_L(percent * res, 2 * res)
-            lll.move([i * space for space in grid_spacing])
-
-        text = LLL << pg.text(str(res), size=20)
-        text.move(
-            text.get_bounding_box()[0], [(i + 1) * space for space in grid_spacing]
-        )
-
-        LLL.flatten(single_layer=layer)
-        LLL.name = f"3L({space} x {res})"
-        return LLL
-
-    def create_waffle(res=1):
-
-        WAFFLE = Device()
-        W = pg.rectangle(size=(res * 80, res * 80))
-
-        pattern = [(res * x, res * 80) for x in [2, 1, 1, 2, 3, 5, 8, 13, 21, 15]]
-        WOut = pg.gridsweep(
-            function=pg.rectangle, param_x={"size": pattern}, param_y={}, spacing=res
-        )
-
-        WOut.move(WOut.center, W.center)
-        W1 = pg.boolean(W, WOut, "A-B")
-
-        WOut.rotate(90, center=WOut.center)
-        W2 = pg.boolean(W, WOut, "A-B")
-
-        WAFFLE << W1
-        WAFFLE << W2
-        text = WAFFLE << pg.text(str(res), size=20)
-        text.move(
-            (text.get_bounding_box()[0][0], text.get_bounding_box()[1][1]),
-            (2 * res, -2 * res),
-        )
-
-        WAFFLE.flatten(single_layer=layer)
-        WAFFLE.name = f"WAFFLE({res})"
-        return WAFFLE
-
-    RES_TEST1 = pg.gridsweep(
-        function=create_3L,
-        param_x={"res": resolutions},
-        param_y={},
-        spacing=10,
-        align_y="ymin",
-        label_layer=None,
-    )
-    RES_TEST1.name = "3Ls"
-    RES_TEST2 = pg.gridsweep(
-        function=create_waffle,
-        param_x={"res": resolutions},
-        param_y={},
-        spacing=10,
-        align_y="ymax",
-        label_layer=None,
-    )
-    RES_TEST2.name = "WAFFLES"
-    RES_TEST = pg.grid(
-        device_list=[[RES_TEST1], [RES_TEST2]],
-        spacing=20,
-        align_x="xmin",
-    )
-
-    if inverted:
-        if inverted == True:
-            RES_TEST = pg.invert(RES_TEST, border=5, precision=0.0000001, layer=layer)
-        else:
-            RES_TEST = pg.outline(RES_TEST, inverted, layer=layer)
-        res_test_name = "RESOLUTION TEST INVERTED "
-    else:
-        res_test_name = "RESOLUTION TEST "
-
-    RES_TEST.move(RES_TEST.center, (0, 0))
-    RES_TEST.name = res_test_name
-    return RES_TEST
-
-
-def vdp(l: float = 400, w: float = 40, layer: int = dflt.layers["device"]) -> Device:
-    """Creates a Van der Pauw (VDP) device with specified dimensions.
-
-    Args:
-        l (float): Length of the VDP device, overall maximum dimension, in µm.
-        w (float): Width of the contact points (width of the ports), in µm.
-        layer (int): Layer to put the device on.
-
-    Returns:
-        Device: VDP device object.
-    """
-    VDP = pg.Device("VAN DER PAUW")
-
-    xpts = [-w / 2, w / 2, l / 2, l / 2, w / 2, -w / 2, -l / 2, -l / 2]
-    ypts = [l / 2, l / 2, w / 2, -w / 2, -l / 2, -l / 2, -w / 2, w / 2]
-
-    polygon = pg.polygon_ports(xpts=xpts, ypts=ypts, layer=layer)
-    VDP << polygon
-    VDP.flatten()
-
-    VDP.add_port(port=polygon.ports["1"], name="N1")
-    VDP.add_port(port=polygon.ports["3"], name="E1")
-    VDP.add_port(port=polygon.ports["5"], name="S1")
-    VDP.add_port(port=polygon.ports["7"], name="W1")
-
-    return VDP
+"""Tests contains common test structures for following/characterizing a
+fabrication process and its effect on the materials."""
+
+from phidl import Device
+import phidl.geometry as pg
+from typing import List, Union
+import qnngds._default_param as dflt
+
+
+def alignment_mark(layers: List[int] = [1, 2, 3, 4]) -> Device:
+    """Creates an alignment mark for each photolithography.
+
+    Args:
+        layers (List[int]): An array of layers.
+
+    Returns:
+        Device: A device containing the alignment marks on each layer.
+    """
+
+    def create_marker(layer1, layer2):
+
+        MARK = Device()
+
+        # central part with cross
+
+        CROSS = Device("CROSS")
+        cross = CROSS << pg.union(pg.cross(length=190, width=20), layer=layer1)
+        rect = pg.rectangle((65, 65), layer=layer2)
+        window = CROSS.add_array(rect, 2, 2, (125, 125))
+        window.move(window.center, cross.center)
+        MARK << CROSS.flatten()
+
+        # combs
+        def create_comb(pitch1=500, pitch2=100, layer1=1, layer2=2):
+
+            COMB = Device()
+
+            # middle comb (made of layer1), pitch = 10
+            rect1 = pg.rectangle((5, 30), layer=layer1)
+            middle_comb = COMB.add_array(rect1, 21, 1, spacing=(10, 0))
+            middle_comb.move(COMB.center, (0, 0))
+
+            # top and bottom combs (made of layer2), pitchs = 10+pitch1, 10+pitch2
+            rect2 = pg.rectangle((5, 30), layer=layer2)
+            top_comb = COMB.add_array(rect2, 21, 1, spacing=(10 + pitch1 / 1000, 0))
+            top_comb.move(
+                top_comb.center, (middle_comb.center[0], middle_comb.center[1] + 30)
+            )
+            top_text = COMB.add_ref(pg.text(f"{pitch1}NM", size=10, layer=layer2))
+            top_text.move(top_text.center, (140, 30))
+
+            bottom_comb = COMB.add_array(rect2, 21, 1, spacing=(10 + pitch2 / 1000, 0))
+            bottom_comb.move(
+                bottom_comb.center, (middle_comb.center[0], middle_comb.center[1] - 30)
+            )
+            bottom_text = COMB.add_ref(pg.text(f"{pitch2}NM", size=10, layer=layer2))
+            bottom_text.move(bottom_text.center, (140, -30))
+
+            # additional markers (made of layer1), for clarity
+            rect1a = pg.rectangle((5, 20), layer=layer1)
+            marksa = COMB.add_array(rect1a, 3, 2, spacing=(100, 110))
+            marksa.move(marksa.center, middle_comb.center)
+
+            rect1b = pg.rectangle((5, 10), layer=layer1)
+            marksb = COMB.add_array(rect1b, 2, 2, spacing=(100, 100))
+            marksb.move(marksb.center, middle_comb.center)
+
+            return COMB
+
+        VERNIER = Device("VERNIER(500, 200, 100, 50)")
+        comb51 = create_comb(pitch1=500, pitch2=100, layer1=layer1, layer2=layer2)
+
+        top = VERNIER.add_ref(comb51)
+        top.move((0, 0), (0, 200))
+
+        left = VERNIER.add_ref(comb51)
+        left.rotate(90)
+        left.move((0, 0), (-200, 0))
+
+        comb205 = create_comb(pitch1=200, pitch2=50, layer1=layer1, layer2=layer2)
+
+        bottom = VERNIER.add_ref(comb205)
+        bottom.rotate(180)
+        bottom.move((0, 0), (0, -200))
+
+        right = VERNIER.add_ref(comb205)
+        right.rotate(-90)
+        right.move((0, 0), (200, 0))
+        MARK << VERNIER.flatten()
+
+        MARK.move(MARK.center, (0, 0))
+
+        # text
+        TEXT = Device(f"TEXT({layer2} ON {layer1})")
+        text1 = TEXT << pg.text(str(layer2), size=50, layer={layer1, layer2})
+        text1.move(text1.center, (220, 200))
+        text2 = TEXT << pg.text(f"{layer2} ON {layer1}", size=10, layer=layer2)
+        text2.move(text2.center, (220, 240))
+        MARK << TEXT.flatten()
+
+        MARK.name = f"ALIGN {layer2} ON {layer1}"
+        return MARK
+
+    ALIGN = Device("ALIGN ")
+    markers_pitch = 600
+    for i, layer1 in enumerate(layers):
+        n = len(layers) - i - 1
+        if n != 0:
+            for j, layer2 in enumerate(layers[-n:]):
+                MARK = create_marker(layer1, layer2)
+                MARK.move((j * markers_pitch, i * markers_pitch))
+                ALIGN << MARK
+            text = pg.text(str(layer1), size=160, layer=layer1)
+            text.name = f"TEXT({str(layer1)})"
+            text.move(text.center, (-340, i * markers_pitch))
+            ALIGN << text
+
+    num_layers = len(layers)
+    offset = -(num_layers - 2) * markers_pitch / 2
+    ALIGN.move((0, 0), (offset, offset))
+    return ALIGN
+
+
+def resolution_test(
+    resolutions: List[float] = [0.8, 1, 1.2, 1.4, 1.6, 1.8, 2.0],
+    inverted: Union[bool, float] = False,
+    layer: int = dflt.layers["device"],
+) -> Device:
+    """Creates test structures for determining a process resolution.
+
+    Args:
+        resolutions (List[float]): List of resolutions (in µm) to be tested.
+        inverted (Union[bool, float]): If True, invert the device. If float, outline the device by this width.
+        layer (int): Layer to put the device on.
+
+    Returns:
+        Device: The test structures, in the specified layer.
+    """
+
+    def create_3L(res=1):
+
+        LLL = Device()
+
+        def create_L(w, spacing):
+
+            L = Device()
+
+            bar = pg.rectangle((min(100 * w, 100), w))
+            bars = Device()
+            bars.add_array(bar, 1, 5, spacing=(0, spacing))
+            v_bars = L << bars
+            h_bars = L << bars
+            h_bars.rotate(90)
+
+            L.align("all", "xmin")
+            L.move((L.xmin, L.ymin), (0, 0))
+            return L
+
+        grid_spacing = (13 * res, 13 * res)
+
+        space = [0.8, 1, 1.2]
+        for i, percent in enumerate(space):
+            lll = LLL << create_L(percent * res, 2 * res)
+            lll.move([i * space for space in grid_spacing])
+
+        text = LLL << pg.text(str(res), size=20)
+        text.move(
+            text.get_bounding_box()[0], [(i + 1) * space for space in grid_spacing]
+        )
+
+        LLL.flatten(single_layer=layer)
+        LLL.name = f"3L({space} x {res})"
+        return LLL
+
+    def create_waffle(res=1):
+
+        WAFFLE = Device()
+        W = pg.rectangle(size=(res * 80, res * 80))
+
+        pattern = [(res * x, res * 80) for x in [2, 1, 1, 2, 3, 5, 8, 13, 21, 15]]
+        WOut = pg.gridsweep(
+            function=pg.rectangle, param_x={"size": pattern}, param_y={}, spacing=res
+        )
+
+        WOut.move(WOut.center, W.center)
+        W1 = pg.boolean(W, WOut, "A-B")
+
+        WOut.rotate(90, center=WOut.center)
+        W2 = pg.boolean(W, WOut, "A-B")
+
+        WAFFLE << W1
+        WAFFLE << W2
+        text = WAFFLE << pg.text(str(res), size=20)
+        text.move(
+            (text.get_bounding_box()[0][0], text.get_bounding_box()[1][1]),
+            (2 * res, -2 * res),
+        )
+
+        WAFFLE.flatten(single_layer=layer)
+        WAFFLE.name = f"WAFFLE({res})"
+        return WAFFLE
+
+    RES_TEST1 = pg.gridsweep(
+        function=create_3L,
+        param_x={"res": resolutions},
+        param_y={},
+        spacing=10,
+        align_y="ymin",
+        label_layer=None,
+    )
+    RES_TEST1.name = "3Ls"
+    RES_TEST2 = pg.gridsweep(
+        function=create_waffle,
+        param_x={"res": resolutions},
+        param_y={},
+        spacing=10,
+        align_y="ymax",
+        label_layer=None,
+    )
+    RES_TEST2.name = "WAFFLES"
+    RES_TEST = pg.grid(
+        device_list=[[RES_TEST1], [RES_TEST2]],
+        spacing=20,
+        align_x="xmin",
+    )
+
+    if inverted:
+        if inverted == True:
+            RES_TEST = pg.invert(RES_TEST, border=5, precision=0.0000001, layer=layer)
+        else:
+            RES_TEST = pg.outline(RES_TEST, inverted, layer=layer)
+        res_test_name = "RESOLUTION TEST INVERTED "
+    else:
+        res_test_name = "RESOLUTION TEST "
+
+    RES_TEST.move(RES_TEST.center, (0, 0))
+    RES_TEST.name = res_test_name
+    return RES_TEST
+
+
+def vdp(l: float = 400, w: float = 40, layer: int = dflt.layers["device"]) -> Device:
+    """Creates a Van der Pauw (VDP) device with specified dimensions.
+
+    Args:
+        l (float): Length of the VDP device, overall maximum dimension, in µm.
+        w (float): Width of the contact points (width of the ports), in µm.
+        layer (int): Layer to put the device on.
+
+    Returns:
+        Device: VDP device object.
+    """
+    VDP = pg.Device("VAN DER PAUW")
+
+    xpts = [-w / 2, w / 2, l / 2, l / 2, w / 2, -w / 2, -l / 2, -l / 2]
+    ypts = [l / 2, l / 2, w / 2, -w / 2, -l / 2, -l / 2, -w / 2, w / 2]
+
+    polygon = pg.polygon_ports(xpts=xpts, ypts=ypts, layer=layer)
+    VDP << polygon
+    VDP.flatten()
+
+    VDP.add_port(port=polygon.ports["1"], name="N1")
+    VDP.add_port(port=polygon.ports["3"], name="E1")
+    VDP.add_port(port=polygon.ports["5"], name="S1")
+    VDP.add_port(port=polygon.ports["7"], name="W1")
+
+    return VDP
```

### Comparing `qnngds-2.4.1/src/qnngds/utilities.py` & `qnngds-2.5.0/src/qnngds/utilities.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,779 +1,828 @@
-"""Utilies is used for building cells in design.
-
-Cells are made of devices
-(found in utilities) and a die_cell border, wich contains pads, text etc... The
-device and its die are linked thanks to functions present in this module.
-"""
-
-from phidl import Device, Port
-import phidl.geometry as pg
-import phidl.routing as pr
-from typing import Tuple, List, Union, Dict, Set
-from phidl.device_layout import (
-    Device,
-    Port,
-)
-import qnngds.geometries as geometry
-import qnngds._default_param as dflt
-
-die_cell_border = dflt.die_cell_border
-
-
-def die_cell(
-    die_size: Tuple[Union[int, float], Union[int, float]] = (dflt.die_w, dflt.die_w),
-    device_max_size: Tuple[Union[int, float], Union[int, float]] = (
-        round(dflt.die_w / 3),
-        round(dflt.die_w / 3),
-    ),
-    pad_size: Tuple[Union[int, float], Union[int, float]] = dflt.pad_size,
-    contact_w: Union[int, float] = 50,
-    contact_l: Union[int, float] = dflt.ebeam_overlap,
-    ports: Dict[str, int] = {"N": 1, "E": 1, "W": 1, "S": 1},
-    ports_gnd: List[str] = ["E", "S"],
-    isolation: Union[int, float] = dflt.die_outline,
-    text: str = "",
-    text_size: Union[int, float] = die_cell_border / 2,
-    layer: int = dflt.layers["die"],
-    pad_layer: int = dflt.layers["pad"],
-    invert: bool = False,
-    fill_pad_layer: bool = False,
-) -> Device:
-    """Creates a die cell with dicing marks, text, and pads to connect to a
-    device.
-
-    Parameters:
-        die_size (tuple of int or float): Overall size of the cell (width, height).
-        device_max_size (tuple of int or float): Max dimensions of the device
-            inside the cell (width, height).
-        pad_size (tuple of int or float): Dimensions of the cell's pads (width, height).
-        contact_w (int or float): Width of the ports and route to be connected
-            to a device.
-        contact_l (int or float): Extra length of the routes above the ports to
-            assure alignment with the device (useful for ebeam lithography).
-        ports (dict): The ports of the device, format must be {'N':m, 'E':n, 'W':p, 'S':q}.
-        ports_gnd (list of string): The ports connected to ground.
-        isolation (int or float): The width of the pads outline.
-        text (string): The text to be displayed on the cell.
-        text_size (int or float): Size of text, corresponds to phidl geometry std.
-        layer (int or array-like[2]): The layer where to put the cell.
-        pad_layer (int or array-like[2]): The layer where to put the contact pads.
-        invert (bool): If True, the cell is inverted (useful for positive tone
-            resists exposure).
-        fill_pad_layer (bool): If True, the space reserved for pads in the
-            die_cell is filled in pad's layer.
-
-    Returns:
-        DIE (Device): The cell, with ports of width contact_w positioned around a device_max_size area.
-    """
-
-    def offset(overlap_port):
-        port_name = overlap_port.name[0]
-        if port_name == "N":
-            overlap_port.midpoint[1] += -contact_l
-        elif port_name == "S":
-            overlap_port.midpoint[1] += contact_l
-        elif port_name == "W":
-            overlap_port.midpoint[0] += contact_l
-        elif port_name == "E":
-            overlap_port.midpoint[0] += -contact_l
-
-    die_name = text.replace("\n", "")
-    DIE = Device(f"DIE {die_name} ")
-
-    border = pg.rectangle(die_size)
-    border.move(border.center, (0, 0))
-
-    borderOut = Device()
-
-    ## Make the routes and pads
-    padOut = Device()
-
-    pad_block_size = (
-        die_size[0] - 2 * pad_size[1] - 4 * isolation,
-        die_size[1] - 2 * pad_size[1] - 4 * isolation,
-    )
-    inner_block = pg.compass_multi(device_max_size, ports)
-    outer_block = pg.compass_multi(pad_block_size, ports)
-    inner_ports = list(inner_block.ports.values())
-
-    for i, port in enumerate(list(outer_block.ports.values())):
-
-        CONNECT = Device()
-        port.rotate(180)
-
-        # create the pad
-        pad = pg.rectangle(pad_size, layer={layer, pad_layer})
-        pad.add_port(
-            "1", midpoint=(pad_size[0] / 2, 0), width=pad_size[0], orientation=90
-        )
-        pad_ref = CONNECT << pad
-        pad_ref.connect(pad.ports["1"], port)
-
-        # create the route from pad to contact
-        port.width = pad_size[0]
-        inner_ports[i].width = contact_w
-        CONNECT << pr.route_quad(port, inner_ports[i], layer=layer)
-
-        # create the route from contact to overlap
-        overlap_port = CONNECT.add_port(port=inner_ports[i])
-        offset(overlap_port)
-        overlap_port.rotate(180)
-        CONNECT << pr.route_quad(inner_ports[i], overlap_port, layer=layer)
-
-        # isolate the pads that are not grounded
-        port_grounded = any(port.name[0] == P for P in ports_gnd)
-        if not port_grounded:
-            padOut << pg.outline(
-                CONNECT, distance=isolation, join="round", open_ports=2 * isolation
-            )
-
-        # add the port to the die
-        DIE.add_port(port=inner_ports[i].rotate(180))
-        DIE << CONNECT
-
-    borderOut << padOut
-
-    ## Add the die markers
-
-    # mark the corners
-    cornersOut = Device()
-
-    corners_coord = [
-        (
-            -die_size[0] / 2 + die_cell_border / 2,
-            -die_size[1] / 2 + die_cell_border / 2,
-        ),
-        (die_size[0] / 2 - die_cell_border / 2, -die_size[1] / 2 + die_cell_border / 2),
-        (die_size[0] / 2 - die_cell_border / 2, die_size[1] / 2 - die_cell_border / 2),
-        (-die_size[0] / 2 + die_cell_border / 2, die_size[1] / 2 - die_cell_border / 2),
-    ]
-    for corner_coord in corners_coord:
-        corner = pg.rectangle(
-            (die_cell_border - isolation, die_cell_border - isolation)
-        )
-        corner = pg.outline(corner, -1 * isolation)
-        corner.move(corner.center, corner_coord)
-        cornersOut << corner
-
-    borderOut << cornersOut
-
-    # label the cell
-    label = pg.text(text, size=text_size, layer=layer)
-    label.move((label.xmin, label.ymin), (0, 0))
-    pos = [x + 2 * isolation + 10 for x in (-die_size[0] / 2, -die_size[1] / 2)]
-    label.move(pos)
-    DIE << label
-    labelOut = pg.outline(label, isolation)
-
-    borderOut << labelOut
-
-    border = pg.boolean(border, borderOut, "A-B", layer=layer)
-    DIE << border
-
-    if fill_pad_layer:
-        border_filled = pg.rectangle(die_size)
-        center = pg.rectangle(device_max_size)
-        border_filled.move(border_filled.center, (0, 0))
-        center.move(center.center, (0, 0))
-        border_filled = pg.boolean(border_filled, center, "A-B")
-
-        border_filled = pg.boolean(border_filled, borderOut, "A-B", layer=pad_layer)
-        DIE << border_filled
-
-    DIE.flatten()
-    ports = DIE.get_ports()
-    DIE = pg.union(DIE, by_layer=True)
-    if invert:
-        PADS = pg.deepcopy(DIE)
-        PADS.remove_layers([layer])
-        PADS.name = "pads"
-        DIE = pg.invert(DIE, border=0, layer=layer)
-        DIE << PADS
-    for port in ports:
-        DIE.add_port(port)
-
-    DIE.name = f"DIE {die_name}"
-    return DIE
-
-
-def calculate_available_space_for_dev(
-    die_size: Tuple[Union[int, float], Union[int, float]] = (dflt.die_w, dflt.die_w),
-    pad_size: Tuple[Union[int, float], Union[int, float]] = dflt.pad_size,
-    contact_l: Union[int, float] = dflt.ebeam_overlap,
-    isolation: Union[int, float] = dflt.die_outline,
-) -> Tuple[float, float]:
-    """Calculates the maximum space available for a device in a die_cell.
-
-    Note that the device should be even smaller than this function's output, as
-    it does not account for routing from the device to the die's ports.
-
-    Parameters:
-        die_size (tuple of int or float): Overall size of the cell (width, height).
-        pad_size (tuple of int or float): Dimensions of the cell's pads (width, height).
-        contact_l (int or float): Extra length of the routes above the ports to
-            assure alignment with the device (useful for ebeam lithography).
-        isolation (int or float): The width of the pads outline.
-
-    Returns:
-        Tuple[float, float]: A tuple containing the width and height of space
-        available for a device in a die_cell
-    """
-
-    dev_max_size = [
-        2 * (die_w / 2 - 3 * isolation - pad_size[1] - 2 * contact_l)
-        for die_w in die_size
-    ]
-    return dev_max_size[0], dev_max_size[1]
-
-
-def calculate_contact_w(
-    circuit_ports: List[Port] = [Port(width=50)],
-    overlap_w: Union[int, float] = dflt.ebeam_overlap,
-) -> Union[int, float]:
-    """Calculate the minimal width acceptable for the contact from the die_cell
-    to the circuit/experiment.
-
-    The conditions are that the contact width should be bigger than (1) the
-    biggest port of the circuit, (2) the overlap_w (to avoid a short).
-
-    Parameters:
-        circuit_ports (list of Port): The ports of the circuit to be placed in the
-            cell (use .get_ports()).
-        overlap_w (int or float): The overlap width in µm (accounts for
-            misalignment between 1st and 2nd ebeam exposures).
-
-    Returns:
-        (int or float): the suggested contact_w to input in the die_cell of the
-        given circuit
-    """
-    max_circuit_port_width = max([port.width for port in circuit_ports])
-    return max(max_circuit_port_width, overlap_w)
-
-
-def add_optimalstep_to_dev(
-    DEVICE: Device, ratio: Union[int, float] = 10, layer: int = dflt.layers["device"]
-) -> Device:
-    """Add an optimal step to the device's ports.
-
-    Note that the subports of the input Device are ignored but still conserved
-    in the returned device.
-
-    Parameters:
-        DEVICE (Device): The Phidl Device to add the optimal steps to.
-        ratio (int or float): the ratio between the width at the end of the step
-            and the width of the device's ports.
-        layer (int or array-like[2]): the layer to place the optimal steps into.
-
-    Returns:
-        (Device): The given Device, with additional steps on its ports. The
-        ports of the returned device have the same name than the ports of the
-        input device and correspond to the steps extremities.
-    """
-    DEV_STP = Device(DEVICE.name)
-
-    DEV_STP << DEVICE
-    for port in DEVICE.flatten().get_ports():
-        STP = pg.optimal_step(
-            port.width, port.width * ratio, symmetric=True, layer=layer
-        )
-        STP.name = f"optimal step x{ratio} "
-        stp = DEV_STP << STP
-        stp.connect(port=1, destination=port)
-        DEV_STP.add_port(port=stp.ports[2], name=port.name)
-
-    return DEV_STP
-
-
-def find_num_diecells_for_dev(
-    device_max_size: Tuple[Union[int, float], Union[int, float]] = (
-        dflt.die_w,
-        dflt.die_w,
-    ),
-    die_size: Tuple[Union[int, float], Union[int, float]] = (dflt.die_w, dflt.die_w),
-    pad_size: Tuple[Union[int, float], Union[int, float]] = dflt.pad_size,
-    contact_l: Union[int, float] = dflt.ebeam_overlap,
-    isolation: Union[int, float] = dflt.die_outline,
-) -> Tuple[float, float]:
-    """Finds the number of die cells that can accommodate a device.
-
-    Parameters:
-        device_max_size(tuple of int or float, optional): Max dimensions of the
-            device inside the cell (width, height).
-        die_size(tuple of int or float, optional): Overall size of the cell (width,
-            height).
-        pad_size(tuple of int or float, optional): Dimensions of the cell's pads
-            (width, height).
-        contact_l (Union[int, float], optional): Extra length of the routes
-            above the ports to assure alignment with the device (useful for
-            ebeam lithography).
-        isolation (Union[int, float], optional): The width of the pads outline.
-
-    Returns:
-        Tuple[float, float]: A tuple containing the number of die cells in width
-        and height required to accommodate the device
-    """
-    n = 1
-    dev_x_bigger = True
-
-    while dev_x_bigger:
-        available_space_for_dev = calculate_available_space_for_dev(
-            (n * die_size[0], die_size[1]), pad_size, contact_l, isolation
-        )
-
-        if device_max_size[0] > available_space_for_dev[0]:
-            n += 1
-        else:
-            break
-
-    m = 1
-    dev_y_bigger = True
-
-    while dev_y_bigger:
-        available_space_for_dev = calculate_available_space_for_dev(
-            (n * die_size[0], m * die_size[1]), pad_size, contact_l, isolation
-        )
-
-        if device_max_size[1] > available_space_for_dev[1]:
-            m += 1
-        else:
-            break
-
-    return n, m
-
-
-def rename_ports_to_compass(DEVICE: Device) -> Device:
-    """Rename ports of a Device based on compass directions.
-
-    Parameters:
-        DEVICE (Device): The Phidl Device object whose ports are to be renamed.
-
-    Returns:
-        Device: A new Phidl Device object with ports renamed to compass directions.
-    """
-    # Create a new Device object to store renamed ports
-    DEV_COMPASS = Device(DEVICE.name)
-
-    # Copy ports from the original device to the new device
-    DEV_COMPASS << DEVICE.flatten()
-
-    # Initialize counters for each direction
-    E_count = 1
-    N_count = 1
-    W_count = 1
-    S_count = 1
-
-    # Iterate through each port in the original device
-    for port in DEVICE.get_ports():
-        # Determine the orientation of the port and rename it accordingly
-        if port.orientation % 360 == 0:
-            DEV_COMPASS.add_port(port=port, name=f"E{E_count}")
-            E_count += 1
-        elif port.orientation % 360 == 90:
-            DEV_COMPASS.add_port(port=port, name=f"N{N_count}")
-            N_count += 1
-        elif port.orientation % 360 == 180:
-            DEV_COMPASS.add_port(port=port, name=f"W{W_count}")
-            W_count += 1
-        elif port.orientation % 360 == 270:
-            DEV_COMPASS.add_port(port=port, name=f"S{S_count}")
-            S_count += 1
-
-    return DEV_COMPASS
-
-
-def add_hyptap_to_cell(
-    die_ports: List[Port],
-    overlap_w: Union[int, float] = dflt.ebeam_overlap,
-    contact_w: Union[int, float] = 5,
-    layer: int = dflt.layers["device"],
-) -> Tuple[Device, Device]:
-    """Takes the cell and adds hyper taper at its ports.
-
-    Parameters:
-        die_ports (list of Port): The ports of the die cell (use .get_ports()).
-        overlap_w (int or float): The overlap width in µm (accounts for
-            misalignment between 1st and 2nd ebeam exposures).
-        contact_w (int or float): The width of the contact with the device's
-            route in µm (width of hyper taper's end).
-        layer (int or array-like[2]): The layer on which to place the device.
-
-    Returns:
-        Tuple[Device, Device]: a tuple containing:
-
-        - **HT** (*Device*): The hyper tapers, positioned at the die's ports.
-          Ports of the same name as the die's ports are added to the output of
-          the tapers.
-        - **device_ports** (*Device*): A device containing only the input ports
-          of the tapers, named as the die's ports.
-    """
-
-    HT = Device("HYPER TAPERS ")
-    device_ports = Device()
-
-    for port in die_ports:
-        ht_w = port.width + 2 * overlap_w
-        ht = HT << geometry.hyper_taper(overlap_w, ht_w, contact_w)
-        ht.connect(ht.ports[2], port)
-        HT.add_port(port=ht.ports[1], name=port.name)
-        device_ports.add_port(port=ht.ports[2], name=port.name)
-
-    HT.flatten(single_layer=layer)
-    return HT, device_ports
-
-
-def route_to_dev(
-    ext_ports: List[Port], dev_ports: Set[Port], layer: int = dflt.layers["device"]
-) -> Device:
-    """Creates smooth routes from external ports to the device's ports. If
-    route_smooth is not working, routes quad.
-
-    Parameters:
-        ext_ports (list of Port): The external ports, e.g., of the die or hyper tapers (use .get_ports()).
-        dev_ports (set of Port): The device's ports, should be named as the external ports (use .ports).
-        layer (int or array-like[2]): The layer to put the routes on.
-
-    Returns:
-        ROUTES (Device): The routes from ports to ports, on the specified layer.
-    """
-
-    ROUTES = Device("ROUTES ")
-
-    for port in ext_ports:
-        dev_port = dev_ports[port.name]
-        try:
-            radius = port.width
-            length1 = 2 * radius
-            length2 = 2 * radius
-            ROUTES << pr.route_smooth(
-                port, dev_port, radius, path_type="Z", length1=length1, length2=length2
-            )
-        except ValueError:
-            try:
-                radius = dev_port.width
-                length1 = radius
-                length2 = radius
-                ROUTES << pr.route_smooth(
-                    port,
-                    dev_port,
-                    radius,
-                    path_type="Z",
-                    length1=length1,
-                    length2=length2,
-                )
-            except ValueError:
-                ROUTES << pr.route_quad(port, dev_port)
-    ROUTES.flatten(single_layer=layer)
-    return ROUTES
-
-
-# from previous qnngds: to be tested...
-
-# def outline(elements, distance = 1, precision = 1e-4, num_divisions = [1, 1],
-#             join = 'miter', tolerance = 2, join_first = True,
-#             max_points = 4000, layer = 0, open_ports=-1, rotate_ports=False):
-#     """ Creates an outline around all the polygons passed in the `elements`
-#     argument. `elements` may be a Device, Polygon, or list of Devices.
-#     Parameters
-#     ----------
-#     elements : Device(/Reference), list of Device(/Reference), or Polygon
-#         Polygons to outline or Device containing polygons to outline.
-#     distance : int or float
-#         Distance to offset polygons. Positive values expand, negative shrink.
-#     precision : float
-#         Desired precision for rounding vertex coordinates.
-#     num_divisions : array-like[2] of int
-#         The number of divisions with which the geometry is divided into
-#         multiple rectangular regions. This allows for each region to be
-#         processed sequentially, which is more computationally efficient.
-#     join : {'miter', 'bevel', 'round'}
-#         Type of join used to create the offset polygon.
-#     tolerance : int or float
-#         For miter joints, this number must be at least 2 and it represents the
-#         maximal distance in multiples of offset between new vertices and their
-#         original position before beveling to avoid spikes at acute joints. For
-#         round joints, it indicates the curvature resolution in number of
-#         points per full circle.
-#     join_first : bool
-#         Join all paths before offsetting to avoid unnecessary joins in
-#         adjacent polygon sides.
-#     max_points : int
-#         The maximum number of vertices within the resulting polygon.
-#     layer : int, array-like[2], or set
-#         Specific layer(s) to put polygon geometry on.
-#   open_ports : int or float
-#       Trims the outline at each port of the element. The value of open_port
-#       scales the length of the trim gemoetry (must be positive).
-#       Useful for positive tone layouts.
-#     Returns
-#     -------
-#     D : Device
-#         A Device containing the outlined polygon(s).
-#     """
-#     D = Device('outline')
-#     if type(elements) is not list: elements = [elements]
-#     for e in elements:
-#         if isinstance(e, Device): D.add_ref(e)
-#         else: D.add(e)
-#     gds_layer, gds_datatype = _parse_layer(layer)
-#     D_bloated = pg.offset(D, distance = distance, join_first = join_first,
-#                        num_divisions = num_divisions, precision = precision,
-#                        max_points = max_points, join = join,
-#                        tolerance = tolerance, layer = layer)
-#     Outline = pg.boolean(A = D_bloated, B = D, operation = 'A-B',
-#                       num_divisions = num_divisions, max_points = max_points,
-#                       precision = precision, layer = layer)
-#     if open_ports>=0:
-#       for i in e.ports:
-#           trim = pg.rectangle(size=(distance, e.ports[i].width+open_ports*distance))
-
-#           trim.rotate(e.ports[i].orientation)
-#           trim.move(trim.center, destination=e.ports[i].midpoint)
-#           if rotate_ports:
-#               trim.movex(-np.cos(e.ports[i].orientation/180*np.pi)*distance/2)
-#               trim.movey(-np.sin(e.ports[i].orientation/180*np.pi)*distance/2)
-#           else:
-#               trim.movex(np.cos(e.ports[i].orientation/180*np.pi)*distance/2)
-#               trim.movey(np.sin(e.ports[i].orientation/180*np.pi)*distance/2)
-
-#           Outline = pg.boolean(A = Outline, B = trim, operation = 'A-B',
-#                      num_divisions = num_divisions, max_points = max_points,
-#                      precision = precision, layer = layer)
-#       for i in e.ports: Outline.add_port(port=e.ports[i])
-#     return Outline
-
-# def assign_ids(device_list, ids):
-#     """
-#     Attach device ID to device list.
-
-#     Parameters
-#     ----------
-#     device_list : LIST
-#         List of phidl device objects.
-#     ids : LIST
-#         list of identification strings.
-#         typically generated from packer_rect/text_labels.
-
-#     Returns
-#     -------
-#     None.
-
-#     """
-#     device_list = list(filter(None,device_list))
-#     for i in range(len(device_list)):
-#         device_list[i].name = ids[i]
-
-# def packer(D_list,
-#            text_letter,
-#            text_pos=(0,-70),
-#            text_layer=1,
-#            text_height=50,
-#            spacing = 100,
-#            aspect_ratio = (1,1),
-#            max_size = (None,750),
-#            sort_by_area = False,
-#            density = 1.1,
-#            precision = 1e-2,
-#            verbose = False):
-#     """
-#     Returns Device "p" with references from D_list. Names, or index, of each device is assigned and can be called from p.references[i].parent.name
-
-
-#     Parameters
-#     ----------
-#     D_list : TYPE
-#         DESCRIPTION.
-#     text_letter : TYPE
-#         DESCRIPTION.
-#     text_pos : TYPE, optional
-#         DESCRIPTION. The default is None.
-#     text_layer : TYPE, optional
-#         DESCRIPTION. The default is 1.
-#     text_height : TYPE, optional
-#         DESCRIPTION. The default is 50.
-#     spacing : TYPE, optional
-#         DESCRIPTION. The default is 10.
-#     aspect_ratio : TYPE, optional
-#         DESCRIPTION. The default is (1,1).
-#     max_size : TYPE, optional
-#         DESCRIPTION. The default is (None,None).
-#     sort_by_area : TYPE, optional
-#         DESCRIPTION. The default is True.
-#     density : TYPE, optional
-#         DESCRIPTION. The default is 1.1.
-#     precision : TYPE, optional
-#         DESCRIPTION. The default is 1e-2.
-#     verbose : TYPE, optional
-#         DESCRIPTION. The default is False.
-#      : TYPE
-#         DESCRIPTION.
-
-#     Returns
-#     -------
-#     TYPE
-#         DESCRIPTION.
-
-#     """
-
-#     p = pg.packer(D_list,
-#         spacing = spacing,
-#         aspect_ratio = aspect_ratio,
-#         max_size = max_size,
-#         sort_by_area = sort_by_area,
-#         density = density,
-#         precision = precision,
-#         verbose = verbose,
-#         )
-
-
-#     for i in range(len(p[0].references)):
-#         device_text = text_letter+str(i)
-#         text_object = pg.text(text=device_text, size = text_height, justify='left', layer=text_layer)
-#         t = p[0].references[i].parent.add_ref(text_object)
-#         t.move(origin=text_object.bbox[0], destination= (text_pos[0], text_pos[1]))
-
-#         p[0].references[i].parent.name = device_text
-
-#     p = p[0]
-#     p.name = text_letter
-#     p._internal_name = text_letter
-#     # p.flatten() # do not flatten.
-
-#     return p
-
-# def packer_rect(device_list, dimensions, spacing, text_pos=None, text_size = 50, text_layer = 1):
-#     """
-#     This function distributes devices from a list onto a rectangular grid. The aspect ratio (dimensions) and spacing must be specified.
-#     If specified, text can be added automatically in a A1, B2, C3, style. The text will start with A0 in the NW corner.
-
-#     Parameters
-#     ----------
-#     device_list : LIST
-#         LIST OF PHIDL DEVICE OBJECTS
-#     dimensions : TUPLE
-#         (X,Y) X BY Y GRID POINTS
-#     spacing : TUPLE
-#         (dX,dY) SPACING BETWEEN GRID POINTS
-#     text_pos : TUPLE, optional
-#         IF SPECIFIED THE GENERATED TEXT IS LOCATED AT (dX,dY) FROM SW CORNER. The default is None.
-#     text_size : INT, optional
-#         SIZE OF TEXT LABEL. The default is 50.
-#     text_layer : INT, optional
-#         LAYER TO ADD TEXT LABEL TO The default is 1.
-
-#     Returns
-#     -------
-#     D : DEVICE
-#         PHIDL device object. List is entered and a single device is returned with labels.
-#     text_list : LIST
-#         LIST of strings of device labels.
-
-#     """
-
-#     letters = list(string.ascii_uppercase)
-
-#     while len(device_list) < np.product(dimensions):
-#         device_list.append(None)
-
-#     new_shape = np.reshape(device_list,dimensions)
-#     text_list=[]
-#     D = Device('return')
-#     for i in range(dimensions[0]):
-#         for j in range(dimensions[1]):
-#             if not new_shape[i][j] == None:
-#                 moved_device = new_shape[i][j].move(origin=new_shape[i][j].bbox[0], destination=(i*spacing[0], -j*spacing[1]))
-#                 D.add_ref(moved_device)
-#                 if text_pos:
-#                     device_text = letters[i]+str(j)
-#                     text_list.append(device_text)
-#                     text_object = pg.text(text=device_text, size = text_size, justify='left', layer=text_layer)
-#                     text_object.move(destination= (i*spacing[0]+text_pos[0], -j*spacing[1]+text_pos[1]))
-#                     D.add_ref(text_object)
-
-#     return D, text_list
-
-# def packer_doc(D_pack_list):
-#     """
-#     This function creates a text document to be referenced during meansurement.
-#     Its primary purpose is to serve as a reference for device specifications on chip.
-#     For instance, "A2 is a 3um device."
-
-#     Currently. This function really only works with D_pack_list from packer().
-#     It looks at each reference and grabs the device parameters (which are hard coded).
-#     'line.append(str(D_pack_list[i].references[j].parent.width))'
-#     It would be great to have this as a dynamical property that can be expounded for every kind of device/parameter.
-
-#     'create_device_doc' predated this function and took every np.array parameter in the parameter-dict and wrote it to a .txt file.
-#     The main problem with this function is that the device name is not associated in the parameter-dict.
-
-#     Inputs
-#     ----------
-#     sample: STRING
-#         enter a sample name "SPX000". The file path will be generated on the NAS and the .txt file will be saved there.
-
-#     Parameters
-#     ----------
-#     D_pack_list : LIST
-#         List containing PHIDL Device objects.
-
-#     Returns
-#     -------
-#     None.
-
-#     """
-
-#     """ Safety net for writing to the correct location"""
-
-#     sample = input('enter a sample name: ')
-#     if sample == '':
-#         print('Doc not created')
-#         return
-#     else:
-#         path = os.path.join('S:\SC\Measurements',sample)
-#         os.makedirs(path, exist_ok=True)
-
-#         path = os.path.join('S:\SC\Measurements',sample, sample+'_device_doc.txt')
-
-#         file = open(path, "w")
-
-#         tab = ',\t'
-#         string_list=[]
-#         headers = ['ID', 'WIDTH', 'AREA', 'SQUARES']
-#         headers.append('\n----------------------------------\n')
-
-#         for i in range(len(D_pack_list)):
-#             for j in range(len(D_pack_list[i].references)):
-#                 line = []
-#                 line.append(str(D_pack_list[i].references[j].parent.name))
-#                 line.append(str(D_pack_list[i].references[j].parent.width))
-#                 line.append(str(D_pack_list[i].references[j].parent.area))
-#                 line.append(str(D_pack_list[i].references[j].parent.squares))
-
-#                 line.append('\n')
-#                 string_list.append(tab.join(line))
-#                 string_list.append('. . . . . . . . . . . . . . . . \n')
-#             string_list.append('\\-----------------------------------\\ \n')
-
-#         file.write(tab.join(headers))
-#         file.writelines(string_list)
-#         file.close()
-
-# def assign_ids(device_list, ids):
-#     """
-#     Attach device ID to device list.
-
-#     Parameters
-#     ----------
-#     device_list : LIST
-#         List of phidl device objects.
-#     ids : LIST
-#         list of identification strings.
-#         typically generated from packer_rect/text_labels.
-
-#     Returns
-#     -------
-#     None.
-
-#     """
-#     device_list = list(filter(None,device_list))
-#     for i in range(len(device_list)):
-#         device_list[i].name = ids[i]
+"""Utilies is used for building cells in design.
+
+Cells are made of devices
+(found in utilities) and a die_cell border, wich contains pads, text etc... The
+device and its die are linked thanks to functions present in this module.
+"""
+
+from phidl import Device, Port
+import phidl.geometry as pg
+import phidl.routing as pr
+from typing import Tuple, List, Union, Dict, Set
+from phidl.device_layout import (
+    Device,
+    Port,
+)
+import qnngds.geometries as geometry
+import qnngds._default_param as dflt
+
+die_cell_border = dflt.die_cell_border
+
+
+def die_cell(
+    die_size: Tuple[Union[int, float], Union[int, float]] = (dflt.die_w, dflt.die_w),
+    device_max_size: Tuple[Union[int, float], Union[int, float]] = (
+        round(dflt.die_w / 3),
+        round(dflt.die_w / 3),
+    ),
+    pad_size: Tuple[Union[int, float], Union[int, float]] = dflt.pad_size,
+    contact_w: Union[int, float] = 50,
+    contact_l: Union[int, float] = dflt.ebeam_overlap,
+    ports: Dict[str, int] = {"N": 1, "E": 1, "W": 1, "S": 1},
+    ports_gnd: List[str] = ["E", "S"],
+    isolation: Union[int, float] = dflt.die_outline,
+    text: str = "",
+    text_size: Union[int, float] = die_cell_border / 2,
+    layer: int = dflt.layers["die"],
+    pad_layer: int = dflt.layers["pad"],
+    invert: bool = False,
+    fill_pad_layer: bool = False,
+) -> Device:
+    """Creates a die cell with dicing marks, text, and pads to connect to a
+    device.
+
+    Parameters:
+        die_size (tuple of int or float): Overall size of the cell (width, height).
+        device_max_size (tuple of int or float): Max dimensions of the device
+            inside the cell (width, height).
+        pad_size (tuple of int or float): Dimensions of the cell's pads (width, height).
+        contact_w (int or float): Width of the ports and route to be connected
+            to a device.
+        contact_l (int or float): Extra length of the routes above the ports to
+            assure alignment with the device (useful for ebeam lithography).
+        ports (dict): The ports of the device, format must be {'N':m, 'E':n, 'W':p, 'S':q}.
+        ports_gnd (list of string): The ports connected to ground.
+        isolation (int or float): The width of the pads outline.
+        text (string): The text to be displayed on the cell.
+        text_size (int or float): Size of text, corresponds to phidl geometry std.
+        layer (int or array-like[2]): The layer where to put the cell.
+        pad_layer (int or array-like[2]): The layer where to put the contact pads.
+        invert (bool): If True, the cell is inverted (useful for positive tone
+            resists exposure).
+        fill_pad_layer (bool): If True, the space reserved for pads in the
+            die_cell is filled in pad's layer.
+
+    Returns:
+        DIE (Device): The cell, with ports of width contact_w positioned around a device_max_size area.
+    """
+
+    def offset(overlap_port):
+        port_name = overlap_port.name[0]
+        if port_name == "N":
+            overlap_port.midpoint[1] += -contact_l
+        elif port_name == "S":
+            overlap_port.midpoint[1] += contact_l
+        elif port_name == "W":
+            overlap_port.midpoint[0] += contact_l
+        elif port_name == "E":
+            overlap_port.midpoint[0] += -contact_l
+
+    die_name = text.replace("\n", "")
+    DIE = Device(f"DIE {die_name} ")
+
+    border = pg.rectangle(die_size)
+    border.move(border.center, (0, 0))
+
+    borderOut = Device()
+
+    ## Make the routes and pads
+    padOut = Device()
+
+    pad_block_size = (
+        die_size[0] - 2 * pad_size[1] - 4 * isolation,
+        die_size[1] - 2 * pad_size[1] - 4 * isolation,
+    )
+    inner_block = pg.compass_multi(device_max_size, ports)
+    outer_block = pg.compass_multi(pad_block_size, ports)
+    inner_ports = list(inner_block.ports.values())
+
+    for i, port in enumerate(list(outer_block.ports.values())):
+
+        CONNECT = Device()
+        port.rotate(180)
+
+        # create the pad
+        pad = pg.rectangle(pad_size, layer={layer, pad_layer})
+        pad.add_port(
+            "1", midpoint=(pad_size[0] / 2, 0), width=pad_size[0], orientation=90
+        )
+        pad_ref = CONNECT << pad
+        pad_ref.connect(pad.ports["1"], port)
+
+        # create the route from pad to contact
+        port.width = pad_size[0]
+        inner_ports[i].width = contact_w
+        CONNECT << pr.route_quad(port, inner_ports[i], layer=layer)
+
+        # create the route from contact to overlap
+        overlap_port = CONNECT.add_port(port=inner_ports[i])
+        offset(overlap_port)
+        overlap_port.rotate(180)
+        CONNECT << pr.route_quad(inner_ports[i], overlap_port, layer=layer)
+
+        # isolate the pads that are not grounded
+        port_grounded = any(port.name[0] == P for P in ports_gnd)
+        if not port_grounded:
+            padOut << pg.outline(
+                CONNECT, distance=isolation, join="round", open_ports=2 * isolation
+            )
+
+        # add the port to the die
+        DIE.add_port(port=inner_ports[i].rotate(180))
+        DIE << CONNECT
+
+    borderOut << padOut
+
+    ## Add the die markers
+
+    # mark the corners
+    cornersOut = Device()
+
+    corners_coord = [
+        (
+            -die_size[0] / 2 + die_cell_border / 2,
+            -die_size[1] / 2 + die_cell_border / 2,
+        ),
+        (die_size[0] / 2 - die_cell_border / 2, -die_size[1] / 2 + die_cell_border / 2),
+        (die_size[0] / 2 - die_cell_border / 2, die_size[1] / 2 - die_cell_border / 2),
+        (-die_size[0] / 2 + die_cell_border / 2, die_size[1] / 2 - die_cell_border / 2),
+    ]
+    for corner_coord in corners_coord:
+        corner = pg.rectangle(
+            (die_cell_border - isolation, die_cell_border - isolation)
+        )
+        corner = pg.outline(corner, -1 * isolation)
+        corner.move(corner.center, corner_coord)
+        cornersOut << corner
+
+    borderOut << cornersOut
+
+    # label the cell
+    label = pg.text(text, size=text_size, layer=layer)
+    label.move((label.xmin, label.ymin), (0, 0))
+    pos = [x + 2 * isolation + 10 for x in (-die_size[0] / 2, -die_size[1] / 2)]
+    label.move(pos)
+    DIE << label
+    labelOut = pg.outline(label, isolation)
+
+    borderOut << labelOut
+
+    border = pg.boolean(border, borderOut, "A-B", layer=layer)
+    DIE << border
+
+    if fill_pad_layer:
+        border_filled = pg.rectangle(die_size)
+        center = pg.rectangle(device_max_size)
+        border_filled.move(border_filled.center, (0, 0))
+        center.move(center.center, (0, 0))
+        border_filled = pg.boolean(border_filled, center, "A-B")
+
+        border_filled = pg.boolean(border_filled, borderOut, "A-B", layer=pad_layer)
+        DIE << border_filled
+
+    DIE.flatten()
+    ports = DIE.get_ports()
+    DIE = pg.union(DIE, by_layer=True)
+    if invert:
+        PADS = pg.deepcopy(DIE)
+        PADS.remove_layers([layer])
+        PADS.name = "pads"
+        DIE = pg.invert(DIE, border=0, layer=layer)
+        DIE << PADS
+    for port in ports:
+        DIE.add_port(port)
+
+    DIE.name = f"DIE {die_name}"
+    return DIE
+
+
+def calculate_available_space_for_dev(
+    die_size: Tuple[Union[int, float], Union[int, float]] = (dflt.die_w, dflt.die_w),
+    pad_size: Tuple[Union[int, float], Union[int, float]] = dflt.pad_size,
+    contact_l: Union[int, float] = dflt.ebeam_overlap,
+    isolation: Union[int, float] = dflt.die_outline,
+    device_ports: List[str] = ["N", "W", "S", "E"],
+) -> Tuple[float, float]:
+    """Calculates the maximum space available for a device in a die_cell.
+
+    Note that the device should be even smaller than this function's output, as
+    it does not account for routing from the device to the die's ports.
+
+    Parameters:
+        die_size (tuple of int or float): Overall size of the cell (width, height).
+        pad_size (tuple of int or float): Dimensions of the cell's pads (width, height).
+        contact_l (int or float): Extra length of the routes above the ports to
+            assure alignment with the device (useful for ebeam lithography).
+        isolation (int or float): The width of the pads outline.
+        device_ports (List of string): a list of existing ports in the device.
+            E.g.: the device has 2 ports North and 1 South, device_ports = ["N", "S"].
+
+    Returns:
+        Tuple[float, float]: A tuple containing the width and height of space
+        available for a device in a die_cell
+    """
+
+    num_pads_y = 0
+    num_pads_x = 0
+    if "N" in device_ports:
+        num_pads_y += 1
+    if "S" in device_ports:
+        num_pads_y += 1
+    if "E" in device_ports:
+        num_pads_x += 1
+    if "W" in device_ports:
+        num_pads_x += 1
+
+    dev_max_x = (
+        die_size[0]
+        - 2 * isolation
+        - max(
+            2 * die_cell_border,
+            num_pads_x * (2 * isolation + pad_size[1] + 2 * contact_l),
+        )
+    )
+    dev_max_y = (
+        die_size[1]
+        - 2 * isolation
+        - max(
+            2 * die_cell_border,
+            num_pads_y * (2 * isolation + pad_size[1] + 2 * contact_l),
+        )
+    )
+    return dev_max_x, dev_max_y
+
+
+def calculate_contact_w(
+    circuit_ports: List[Port] = [Port(width=50)],
+    overlap_w: Union[int, float] = dflt.ebeam_overlap,
+) -> Union[int, float]:
+    """Calculate the minimal width acceptable for the contact from the die_cell
+    to the circuit/experiment.
+
+    The conditions are that the contact width should be bigger than (1) the
+    biggest port of the circuit, (2) the overlap_w (to avoid a short).
+
+    Parameters:
+        circuit_ports (list of Port): The ports of the circuit to be placed in the
+            cell (use .get_ports()).
+        overlap_w (int or float): The overlap width in µm (accounts for
+            misalignment between 1st and 2nd ebeam exposures).
+
+    Returns:
+        (int or float): the suggested contact_w to input in the die_cell of the
+        given circuit
+    """
+    max_circuit_port_width = max([port.width for port in circuit_ports])
+    return max(max_circuit_port_width, overlap_w)
+
+
+def add_optimalstep_to_dev(
+    DEVICE: Device, ratio: Union[int, float] = 10, layer: int = dflt.layers["device"]
+) -> Device:
+    """Add an optimal step to the device's ports.
+
+    Note that the subports of the input Device are ignored but still conserved
+    in the returned device.
+
+    Parameters:
+        DEVICE (Device): The Phidl Device to add the optimal steps to.
+        ratio (int or float): the ratio between the width at the end of the step
+            and the width of the device's ports.
+        layer (int or array-like[2]): the layer to place the optimal steps into.
+
+    Returns:
+        (Device): The given Device, with additional steps on its ports. The
+        ports of the returned device have the same name than the ports of the
+        input device and correspond to the steps extremities.
+    """
+    DEV_STP = Device(DEVICE.name)
+
+    DEV_STP << DEVICE
+    for port in DEVICE.flatten().get_ports():
+        STP = pg.optimal_step(
+            port.width, port.width * ratio, symmetric=True, layer=layer
+        )
+        STP.name = f"optimal step x{ratio} "
+        stp = DEV_STP << STP
+        stp.connect(port=1, destination=port)
+        DEV_STP.add_port(port=stp.ports[2], name=port.name)
+
+    return DEV_STP
+
+
+def find_num_diecells_for_dev(
+    device_max_size: Tuple[Union[int, float], Union[int, float]] = (
+        dflt.die_w,
+        dflt.die_w,
+    ),
+    device_ports: Dict[str, int] = {"N": 1, "E": 1, "W": 1, "S": 1},
+    die_size: Tuple[Union[int, float], Union[int, float]] = (dflt.die_w, dflt.die_w),
+    pad_size: Tuple[Union[int, float], Union[int, float]] = dflt.pad_size,
+    contact_l: Union[int, float] = dflt.ebeam_overlap,
+    isolation: Union[int, float] = dflt.die_outline,
+) -> Tuple[float, float]:
+    """Finds the number of die cells that can accommodate a device.
+
+    Parameters:
+        device_max_size (tuple of int or float, optional): Max dimensions of the
+            device inside the cell (width, height).
+        device_ports (dict): The ports of the device, format must be {'N':m, 'E':n, 'W':p, 'S':q}.
+        die_size (tuple of int or float, optional): Overall size of the cell (width,
+            height).
+        pad_size(tuple of int or float, optional): Dimensions of the cell's pads
+            (width, height).
+        contact_l (Union[int, float], optional): Extra length of the routes
+            above the ports to assure alignment with the device (useful for
+            ebeam lithography).
+        isolation (Union[int, float], optional): The width of the pads outline.
+
+    Returns:
+        Tuple[float, float]: A tuple containing the number of die cells in width
+        and height required to accommodate the device
+    """
+
+    max_num_ports_y = max(device_ports.get("E", 0), device_ports.get("W", 0))
+    max_num_ports_x = max(device_ports.get("N", 0), device_ports.get("S", 0))
+
+    max_x = max(
+        device_max_size[0], max_num_ports_x * 1.5 * pad_size[0] + 2 * die_cell_border
+    )
+    max_y = max(
+        device_max_size[1], max_num_ports_y * 1.5 * pad_size[0] + 2 * die_cell_border
+    )
+    compass_ports = [W for W in ["N", "E", "S", "W"] if device_ports.get(W, 0) != 0]
+
+    n = 1
+    dev_x_bigger = True
+
+    while dev_x_bigger:
+        available_space_for_dev = calculate_available_space_for_dev(
+            (n * die_size[0], die_size[1]),
+            pad_size,
+            contact_l,
+            isolation,
+            compass_ports,
+        )
+        if max_x > available_space_for_dev[0]:
+            n += 1
+        else:
+            break
+
+    m = 1
+    dev_y_bigger = True
+
+    while dev_y_bigger:
+        available_space_for_dev = calculate_available_space_for_dev(
+            (n * die_size[0], m * die_size[1]),
+            pad_size,
+            contact_l,
+            isolation,
+            compass_ports,
+        )
+
+        if device_max_size[1] > available_space_for_dev[1]:
+            m += 1
+        else:
+            break
+
+    return n, m
+
+
+def rename_ports_to_compass(DEVICE: Device, depth: Union[int, None] = 0) -> Device:
+    """Rename ports of a Device based on compass directions.
+
+    Parameters:
+        DEVICE (Device): The Phidl Device object whose ports are to be renamed.
+
+    Returns:
+        Device: A new Phidl Device object with ports renamed to compass directions.
+    """
+
+    ports = DEVICE.get_ports(depth=depth)
+    # Create a new Device object to store renamed ports
+    DEV_COMPASS = Device(DEVICE.name)
+
+    # Copy ports from the original device to the new device
+    DEV_COMPASS << DEVICE
+
+    # Initialize counters for each direction
+    E_count = 1
+    N_count = 1
+    W_count = 1
+    S_count = 1
+
+    # Iterate through each port in the original device
+    for port in ports:
+        # Determine the orientation of the port and rename it accordingly
+        if port.orientation % 360 == 0:
+            DEV_COMPASS.add_port(port=port, name=f"E{E_count}")
+            E_count += 1
+        elif port.orientation % 360 == 90:
+            DEV_COMPASS.add_port(port=port, name=f"N{N_count}")
+            N_count += 1
+        elif port.orientation % 360 == 180:
+            DEV_COMPASS.add_port(port=port, name=f"W{W_count}")
+            W_count += 1
+        elif port.orientation % 360 == 270:
+            DEV_COMPASS.add_port(port=port, name=f"S{S_count}")
+            S_count += 1
+
+    return DEV_COMPASS
+
+
+def add_hyptap_to_cell(
+    die_ports: List[Port],
+    overlap_w: Union[int, float] = dflt.ebeam_overlap,
+    contact_w: Union[int, float] = 5,
+    layer: int = dflt.layers["device"],
+) -> Tuple[Device, Device]:
+    """Takes the cell and adds hyper taper at its ports.
+
+    Parameters:
+        die_ports (list of Port): The ports of the die cell (use .get_ports()).
+        overlap_w (int or float): The overlap width in µm (accounts for
+            misalignment between 1st and 2nd ebeam exposures).
+        contact_w (int or float): The width of the contact with the device's
+            route in µm (width of hyper taper's end).
+        layer (int or array-like[2]): The layer on which to place the device.
+
+    Returns:
+        Tuple[Device, Device]: a tuple containing:
+
+        - **HT** (*Device*): The hyper tapers, positioned at the die's ports.
+          Ports of the same name as the die's ports are added to the output of
+          the tapers.
+        - **device_ports** (*Device*): A device containing only the input ports
+          of the tapers, named as the die's ports.
+    """
+
+    HT = Device("HYPER TAPERS ")
+    device_ports = Device()
+
+    for port in die_ports:
+        ht_w = port.width + 2 * overlap_w
+        ht = HT << geometry.hyper_taper(overlap_w, ht_w, contact_w)
+        ht.connect(ht.ports[2], port)
+        HT.add_port(port=ht.ports[1], name=port.name)
+        device_ports.add_port(port=ht.ports[2], name=port.name)
+
+    HT.flatten(single_layer=layer)
+    return HT, device_ports
+
+
+def route_to_dev(
+    ext_ports: List[Port], dev_ports: Set[Port], layer: int = dflt.layers["device"]
+) -> Device:
+    """Creates smooth routes from external ports to the device's ports. If
+    route_smooth is not working, routes quad.
+
+    Parameters:
+        ext_ports (list of Port): The external ports, e.g., of the die or hyper tapers (use .get_ports()).
+        dev_ports (set of Port): The device's ports, should be named as the external ports (use .ports).
+        layer (int or array-like[2]): The layer to put the routes on.
+
+    Returns:
+        ROUTES (Device): The routes from ports to ports, on the specified layer.
+    """
+
+    ROUTES = Device("ROUTES ")
+
+    for port in ext_ports:
+        dev_port = dev_ports[port.name]
+        try:
+            radius = port.width
+            length1 = 2 * radius
+            length2 = 2 * radius
+            ROUTES << pr.route_smooth(
+                port, dev_port, radius, path_type="Z", length1=length1, length2=length2
+            )
+        except ValueError:
+            try:
+                radius = dev_port.width
+                length1 = radius
+                length2 = radius
+                ROUTES << pr.route_smooth(
+                    port,
+                    dev_port,
+                    radius,
+                    path_type="Z",
+                    length1=length1,
+                    length2=length2,
+                )
+            except ValueError:
+                ROUTES << pr.route_quad(port, dev_port)
+    ROUTES.flatten(single_layer=layer)
+    return ROUTES
+
+
+# from previous qnngds: to be tested...
+
+# def outline(elements, distance = 1, precision = 1e-4, num_divisions = [1, 1],
+#             join = 'miter', tolerance = 2, join_first = True,
+#             max_points = 4000, layer = 0, open_ports=-1, rotate_ports=False):
+#     """ Creates an outline around all the polygons passed in the `elements`
+#     argument. `elements` may be a Device, Polygon, or list of Devices.
+#     Parameters
+#     ----------
+#     elements : Device(/Reference), list of Device(/Reference), or Polygon
+#         Polygons to outline or Device containing polygons to outline.
+#     distance : int or float
+#         Distance to offset polygons. Positive values expand, negative shrink.
+#     precision : float
+#         Desired precision for rounding vertex coordinates.
+#     num_divisions : array-like[2] of int
+#         The number of divisions with which the geometry is divided into
+#         multiple rectangular regions. This allows for each region to be
+#         processed sequentially, which is more computationally efficient.
+#     join : {'miter', 'bevel', 'round'}
+#         Type of join used to create the offset polygon.
+#     tolerance : int or float
+#         For miter joints, this number must be at least 2 and it represents the
+#         maximal distance in multiples of offset between new vertices and their
+#         original position before beveling to avoid spikes at acute joints. For
+#         round joints, it indicates the curvature resolution in number of
+#         points per full circle.
+#     join_first : bool
+#         Join all paths before offsetting to avoid unnecessary joins in
+#         adjacent polygon sides.
+#     max_points : int
+#         The maximum number of vertices within the resulting polygon.
+#     layer : int, array-like[2], or set
+#         Specific layer(s) to put polygon geometry on.
+#   open_ports : int or float
+#       Trims the outline at each port of the element. The value of open_port
+#       scales the length of the trim gemoetry (must be positive).
+#       Useful for positive tone layouts.
+#     Returns
+#     -------
+#     D : Device
+#         A Device containing the outlined polygon(s).
+#     """
+#     D = Device('outline')
+#     if type(elements) is not list: elements = [elements]
+#     for e in elements:
+#         if isinstance(e, Device): D.add_ref(e)
+#         else: D.add(e)
+#     gds_layer, gds_datatype = _parse_layer(layer)
+#     D_bloated = pg.offset(D, distance = distance, join_first = join_first,
+#                        num_divisions = num_divisions, precision = precision,
+#                        max_points = max_points, join = join,
+#                        tolerance = tolerance, layer = layer)
+#     Outline = pg.boolean(A = D_bloated, B = D, operation = 'A-B',
+#                       num_divisions = num_divisions, max_points = max_points,
+#                       precision = precision, layer = layer)
+#     if open_ports>=0:
+#       for i in e.ports:
+#           trim = pg.rectangle(size=(distance, e.ports[i].width+open_ports*distance))
+
+#           trim.rotate(e.ports[i].orientation)
+#           trim.move(trim.center, destination=e.ports[i].midpoint)
+#           if rotate_ports:
+#               trim.movex(-np.cos(e.ports[i].orientation/180*np.pi)*distance/2)
+#               trim.movey(-np.sin(e.ports[i].orientation/180*np.pi)*distance/2)
+#           else:
+#               trim.movex(np.cos(e.ports[i].orientation/180*np.pi)*distance/2)
+#               trim.movey(np.sin(e.ports[i].orientation/180*np.pi)*distance/2)
+
+#           Outline = pg.boolean(A = Outline, B = trim, operation = 'A-B',
+#                      num_divisions = num_divisions, max_points = max_points,
+#                      precision = precision, layer = layer)
+#       for i in e.ports: Outline.add_port(port=e.ports[i])
+#     return Outline
+
+# def assign_ids(device_list, ids):
+#     """
+#     Attach device ID to device list.
+
+#     Parameters
+#     ----------
+#     device_list : LIST
+#         List of phidl device objects.
+#     ids : LIST
+#         list of identification strings.
+#         typically generated from packer_rect/text_labels.
+
+#     Returns
+#     -------
+#     None.
+
+#     """
+#     device_list = list(filter(None,device_list))
+#     for i in range(len(device_list)):
+#         device_list[i].name = ids[i]
+
+# def packer(D_list,
+#            text_letter,
+#            text_pos=(0,-70),
+#            text_layer=1,
+#            text_height=50,
+#            spacing = 100,
+#            aspect_ratio = (1,1),
+#            max_size = (None,750),
+#            sort_by_area = False,
+#            density = 1.1,
+#            precision = 1e-2,
+#            verbose = False):
+#     """
+#     Returns Device "p" with references from D_list. Names, or index, of each device is assigned and can be called from p.references[i].parent.name
+
+
+#     Parameters
+#     ----------
+#     D_list : TYPE
+#         DESCRIPTION.
+#     text_letter : TYPE
+#         DESCRIPTION.
+#     text_pos : TYPE, optional
+#         DESCRIPTION. The default is None.
+#     text_layer : TYPE, optional
+#         DESCRIPTION. The default is 1.
+#     text_height : TYPE, optional
+#         DESCRIPTION. The default is 50.
+#     spacing : TYPE, optional
+#         DESCRIPTION. The default is 10.
+#     aspect_ratio : TYPE, optional
+#         DESCRIPTION. The default is (1,1).
+#     max_size : TYPE, optional
+#         DESCRIPTION. The default is (None,None).
+#     sort_by_area : TYPE, optional
+#         DESCRIPTION. The default is True.
+#     density : TYPE, optional
+#         DESCRIPTION. The default is 1.1.
+#     precision : TYPE, optional
+#         DESCRIPTION. The default is 1e-2.
+#     verbose : TYPE, optional
+#         DESCRIPTION. The default is False.
+#      : TYPE
+#         DESCRIPTION.
+
+#     Returns
+#     -------
+#     TYPE
+#         DESCRIPTION.
+
+#     """
+
+#     p = pg.packer(D_list,
+#         spacing = spacing,
+#         aspect_ratio = aspect_ratio,
+#         max_size = max_size,
+#         sort_by_area = sort_by_area,
+#         density = density,
+#         precision = precision,
+#         verbose = verbose,
+#         )
+
+
+#     for i in range(len(p[0].references)):
+#         device_text = text_letter+str(i)
+#         text_object = pg.text(text=device_text, size = text_height, justify='left', layer=text_layer)
+#         t = p[0].references[i].parent.add_ref(text_object)
+#         t.move(origin=text_object.bbox[0], destination= (text_pos[0], text_pos[1]))
+
+#         p[0].references[i].parent.name = device_text
+
+#     p = p[0]
+#     p.name = text_letter
+#     p._internal_name = text_letter
+#     # p.flatten() # do not flatten.
+
+#     return p
+
+# def packer_rect(device_list, dimensions, spacing, text_pos=None, text_size = 50, text_layer = 1):
+#     """
+#     This function distributes devices from a list onto a rectangular grid. The aspect ratio (dimensions) and spacing must be specified.
+#     If specified, text can be added automatically in a A1, B2, C3, style. The text will start with A0 in the NW corner.
+
+#     Parameters
+#     ----------
+#     device_list : LIST
+#         LIST OF PHIDL DEVICE OBJECTS
+#     dimensions : TUPLE
+#         (X,Y) X BY Y GRID POINTS
+#     spacing : TUPLE
+#         (dX,dY) SPACING BETWEEN GRID POINTS
+#     text_pos : TUPLE, optional
+#         IF SPECIFIED THE GENERATED TEXT IS LOCATED AT (dX,dY) FROM SW CORNER. The default is None.
+#     text_size : INT, optional
+#         SIZE OF TEXT LABEL. The default is 50.
+#     text_layer : INT, optional
+#         LAYER TO ADD TEXT LABEL TO The default is 1.
+
+#     Returns
+#     -------
+#     D : DEVICE
+#         PHIDL device object. List is entered and a single device is returned with labels.
+#     text_list : LIST
+#         LIST of strings of device labels.
+
+#     """
+
+#     letters = list(string.ascii_uppercase)
+
+#     while len(device_list) < np.product(dimensions):
+#         device_list.append(None)
+
+#     new_shape = np.reshape(device_list,dimensions)
+#     text_list=[]
+#     D = Device('return')
+#     for i in range(dimensions[0]):
+#         for j in range(dimensions[1]):
+#             if not new_shape[i][j] == None:
+#                 moved_device = new_shape[i][j].move(origin=new_shape[i][j].bbox[0], destination=(i*spacing[0], -j*spacing[1]))
+#                 D.add_ref(moved_device)
+#                 if text_pos:
+#                     device_text = letters[i]+str(j)
+#                     text_list.append(device_text)
+#                     text_object = pg.text(text=device_text, size = text_size, justify='left', layer=text_layer)
+#                     text_object.move(destination= (i*spacing[0]+text_pos[0], -j*spacing[1]+text_pos[1]))
+#                     D.add_ref(text_object)
+
+#     return D, text_list
+
+# def packer_doc(D_pack_list):
+#     """
+#     This function creates a text document to be referenced during meansurement.
+#     Its primary purpose is to serve as a reference for device specifications on chip.
+#     For instance, "A2 is a 3um device."
+
+#     Currently. This function really only works with D_pack_list from packer().
+#     It looks at each reference and grabs the device parameters (which are hard coded).
+#     'line.append(str(D_pack_list[i].references[j].parent.width))'
+#     It would be great to have this as a dynamical property that can be expounded for every kind of device/parameter.
+
+#     'create_device_doc' predated this function and took every np.array parameter in the parameter-dict and wrote it to a .txt file.
+#     The main problem with this function is that the device name is not associated in the parameter-dict.
+
+#     Inputs
+#     ----------
+#     sample: STRING
+#         enter a sample name "SPX000". The file path will be generated on the NAS and the .txt file will be saved there.
+
+#     Parameters
+#     ----------
+#     D_pack_list : LIST
+#         List containing PHIDL Device objects.
+
+#     Returns
+#     -------
+#     None.
+
+#     """
+
+#     """ Safety net for writing to the correct location"""
+
+#     sample = input('enter a sample name: ')
+#     if sample == '':
+#         print('Doc not created')
+#         return
+#     else:
+#         path = os.path.join('S:\SC\Measurements',sample)
+#         os.makedirs(path, exist_ok=True)
+
+#         path = os.path.join('S:\SC\Measurements',sample, sample+'_device_doc.txt')
+
+#         file = open(path, "w")
+
+#         tab = ',\t'
+#         string_list=[]
+#         headers = ['ID', 'WIDTH', 'AREA', 'SQUARES']
+#         headers.append('\n----------------------------------\n')
+
+#         for i in range(len(D_pack_list)):
+#             for j in range(len(D_pack_list[i].references)):
+#                 line = []
+#                 line.append(str(D_pack_list[i].references[j].parent.name))
+#                 line.append(str(D_pack_list[i].references[j].parent.width))
+#                 line.append(str(D_pack_list[i].references[j].parent.area))
+#                 line.append(str(D_pack_list[i].references[j].parent.squares))
+
+#                 line.append('\n')
+#                 string_list.append(tab.join(line))
+#                 string_list.append('. . . . . . . . . . . . . . . . \n')
+#             string_list.append('\\-----------------------------------\\ \n')
+
+#         file.write(tab.join(headers))
+#         file.writelines(string_list)
+#         file.close()
+
+# def assign_ids(device_list, ids):
+#     """
+#     Attach device ID to device list.
+
+#     Parameters
+#     ----------
+#     device_list : LIST
+#         List of phidl device objects.
+#     ids : LIST
+#         list of identification strings.
+#         typically generated from packer_rect/text_labels.
+
+#     Returns
+#     -------
+#     None.
+
+#     """
+#     device_list = list(filter(None,device_list))
+#     for i in range(len(device_list)):
+#         device_list[i].name = ids[i]
```

### Comparing `qnngds-2.4.1/tests/all_dev_on_gds.py` & `qnngds-2.5.0/tests/all_dev_on_gds.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,99 +1,97 @@
-"""This module is designed to generate a GDS file named "all_dev.gds". It loops
-through the qnngds' modules, and add each function to the gds in the proper
-package's hierarchy. If the function returns a Device object, it is written.
-
-Run this test from its parent directory (qnngds/tests).
-
-This test is helpfull to check what is the hierarchy and the name in the
-Devices developped.
-
-For eg., a phidl.geometry.union() will return an entirely flattened
-Device named "union". Although very useful, union looses in some way the
-hierachy information and it is important to determine whether or not
-this information is to be kept. The same reflexion goes for
-phidl.geometry.boolean().
-"""
-
-from phidl import Device
-import os
-import importlib.util
-import inspect
-
-import qnngds
-
-
-def write_devices_from_module(module_name, src_path):
-
-    MODULE = Device(str(module_name))
-
-    # Import the module dynamically
-    module_path = os.path.join(src_path, module_name)
-    spec = importlib.util.spec_from_file_location(module_name, module_path)
-    module = importlib.util.module_from_spec(spec)
-    spec.loader.exec_module(module)
-
-    # Get all defined functions in the module
-    functions = inspect.getmembers(module, inspect.isfunction)
-
-    # Execute each function
-    for name, func in functions:
-        FUNCTION = Device(name)
-        try:
-            result = func()
-            if isinstance(result, Device):
-                FUNCTION << result
-                print(f"From '{module_name}', writing '{name}' on the gds.")
-            elif isinstance(result, tuple):
-                result = [item for item in result if isinstance(item, Device)]
-                for result in result:
-                    FUNCTION << result
-                    print(f"From '{module_name}', writing '{name}' on the gds.")
-        except TypeError:
-            pass
-
-        MODULE << FUNCTION
-
-    return MODULE
-
-
-def test_qnngds_devices(src_path):
-    GDS = Device()
-    try:
-        modules = [m for m in os.listdir(src_path) if not m.startswith("_")]
-
-        for module in sorted(modules):
-            if module.endswith(".py"):
-                GDS << write_devices_from_module(module, src_path)
-            else:
-                SUBMOD = Device(f"{module}")
-                module_path = os.path.join(src_path, module)
-                submodules = sorted(
-                    [
-                        m
-                        for m in os.listdir(module_path)
-                        if not m.startswith("_") and m.endswith(".py")
-                    ]
-                )
-                for submodule in submodules:
-                    SUBMOD << write_devices_from_module(
-                        submodule, os.path.join(src_path, module)
-                    )
-                GDS << SUBMOD
-
-    except FileNotFoundError as e:
-        print(e)
-        print(
-            "\nMake sure you are executing the test in the correct directory. "
-            "To fix this, you can run: \n"
-        )
-        current_file_path = os.path.realpath(__file__)
-        parent_folder = os.path.dirname(current_file_path)
-        print("     cd ", parent_folder)
-        print()
-
-    GDS.write_gds("all_dev.gds", max_cellname_length=32000)
-
-
-if __name__ == "__main__":
-    qnngds_path = os.path.join("..", "src", "qnngds")
-    test_qnngds_devices(qnngds_path)
+"""This module is designed to generate a GDS file named "all_dev.gds". It loops
+through the qnngds' modules, and add each function to the gds in the proper
+package's hierarchy. If the function returns a Device object, it is written.
+
+Run this test from its parent directory (qnngds/tests).
+
+This test is helpfull to check what is the hierarchy and the name in the
+Devices developped.
+
+For eg., a phidl.geometry.union() will return an entirely flattened
+Device named "union". Although very useful, union looses in some way the
+hierachy information and it is important to determine whether or not
+this information is to be kept. The same reflexion goes for
+phidl.geometry.boolean().
+"""
+
+from phidl import Device
+import os
+import importlib.util
+import inspect
+
+
+def write_devices_from_module(module_name, src_path):
+
+    MODULE = Device(str(module_name))
+
+    # Import the module dynamically
+    module_path = os.path.join(src_path, module_name)
+    spec = importlib.util.spec_from_file_location(module_name, module_path)
+    module = importlib.util.module_from_spec(spec)
+    spec.loader.exec_module(module)
+
+    # Get all defined functions in the module
+    functions = inspect.getmembers(module, inspect.isfunction)
+
+    # Execute each function
+    for name, func in functions:
+        FUNCTION = Device(name)
+        try:
+            result = func()
+            if isinstance(result, Device):
+                FUNCTION << result
+                print(f"From '{module_name}', writing '{name}' on the gds.")
+            elif isinstance(result, tuple):
+                result = [item for item in result if isinstance(item, Device)]
+                for result in result:
+                    FUNCTION << result
+                    print(f"From '{module_name}', writing '{name}' on the gds.")
+        except TypeError:
+            pass
+
+        MODULE << FUNCTION
+
+    return MODULE
+
+
+def test_qnngds_devices(src_path):
+    GDS = Device()
+    try:
+        modules = [m for m in os.listdir(src_path) if not m.startswith("_")]
+
+        for module in sorted(modules):
+            if module.endswith(".py"):
+                GDS << write_devices_from_module(module, src_path)
+            else:
+                SUBMOD = Device(f"{module}")
+                module_path = os.path.join(src_path, module)
+                submodules = sorted(
+                    [
+                        m
+                        for m in os.listdir(module_path)
+                        if not m.startswith("_") and m.endswith(".py")
+                    ]
+                )
+                for submodule in submodules:
+                    SUBMOD << write_devices_from_module(
+                        submodule, os.path.join(src_path, module)
+                    )
+                GDS << SUBMOD
+
+    except FileNotFoundError as e:
+        print(e)
+        print(
+            "\nMake sure you are executing the test in the correct directory. "
+            "To fix this, you can run: \n"
+        )
+        current_file_path = os.path.realpath(__file__)
+        parent_folder = os.path.dirname(current_file_path)
+        print("     cd ", parent_folder)
+        print()
+
+    GDS.write_gds("all_dev.gds", max_cellname_length=32000)
+
+
+if __name__ == "__main__":
+    qnngds_path = os.path.join("..", "src", "qnngds")
+    test_qnngds_devices(qnngds_path)
```

### Comparing `qnngds-2.4.1/PKG-INFO` & `qnngds-2.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qnngds
-Version: 2.4.1
+Version: 2.5.0
 Summary: The QNN library for creating gds files
 Keywords: phidl,nanowire_electronics,nanofabrication,gds
 Author-Email: "A. Jacquillat" <audrey01@mit.edu>, "A. Jacquillat" <audrey.jacquillat@gmail.com>, "R. Foster" <reedf@mit.edu>
 Maintainer-Email: "A. Jacquillat" <audrey01@mit.edu>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```


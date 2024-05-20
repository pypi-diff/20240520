# Comparing `tmp/sh1106_framework-0.0.7.tar.gz` & `tmp/sh1106_framework-0.0.8.tar.gz`

## Comparing `sh1106_framework-0.0.7.tar` & `sh1106_framework-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/setup.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/__init__.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/sh1106_font_generator.py
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/sh1106_framework.py
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/sh1106_image_generator.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/firmware/main.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/framework/constants.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/framework/states/state.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/framework/states/state_manager.py
--rw-r--r--   0        0        0    11500 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/graphics/drawing.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/graphics/fonts.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/graphics/images.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/tests/ping-pong/ping-pong.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/tests/ping-pong/ping.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/tests/ping-pong/pong.py
--rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/useful-assets/default-font.json
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/useful-assets/default-font.png
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/useful-assets/example-images.json
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/useful-assets/example-images.png
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/LICENSE
--rw-r--r--   0        0        0     8731 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/README.md
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     9542 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/setup.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/src/sh1106_framework/__init__.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/src/sh1106_framework/sh1106_font_generator.py
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/src/sh1106_framework/sh1106_framework.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/src/sh1106_framework/sh1106_image_generator.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/src/sh1106_framework/framework/constants.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/src/sh1106_framework/framework/states/state.py
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/src/sh1106_framework/framework/states/state_manager.py
+-rw-r--r--   0        0        0    11484 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/src/sh1106_framework/graphics/drawing.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/src/sh1106_framework/graphics/fonts.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/src/sh1106_framework/graphics/images.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/tests/ping-pong/ping-pong.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/tests/ping-pong/ping.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/tests/ping-pong/pong.py
+-rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/useful-assets/default-font.json
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/useful-assets/default-font.png
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/useful-assets/example-images.json
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/useful-assets/example-images.png
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/LICENSE
+-rw-r--r--   0        0        0     8731 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/README.md
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     9542 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/PKG-INFO
```

### Comparing `sh1106_framework-0.0.7/setup.py` & `sh1106_framework-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sh1106_framework',
-    version='0.0.7',
+    version='0.0.8',
     author='Dan Convey',
     description='A state manager, graphics, image, and custom font drawing package for the SH1106 OLED screen based on the luma.oled package. It works with Raspberry Pi and other Linux-based single-board computers.',
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `sh1106_framework-0.0.7/src/sh1106_framework/sh1106_font_generator.py` & `sh1106_framework-0.0.8/src/sh1106_framework/sh1106_font_generator.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.7/src/sh1106_framework/sh1106_framework.py` & `sh1106_framework-0.0.8/src/sh1106_framework/sh1106_framework.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from graphics.drawing import Drawing
-from graphics.fonts import Fonts
-from graphics.images import Images
-from framework.constants import Constants
-from framework.states.state_manager import StateManager, State
+from .graphics.drawing import Drawing
+from .graphics.fonts import Fonts
+from .graphics.images import Images
+from .framework.constants import Constants
+from .framework.states.state_manager import StateManager, State
 
 from abc import ABC
 import time
 
 # Seconds per frame
 _SPF = 1 / Constants.FPS
```

### Comparing `sh1106_framework-0.0.7/src/sh1106_framework/sh1106_image_generator.py` & `sh1106_framework-0.0.8/src/sh1106_framework/sh1106_image_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 import argparse
 import sys
-import os
 
 from PIL import Image
 
 
 def __get_pixel_data(image_path):
     # Open the image
     img = Image.open(image_path)
```

### Comparing `sh1106_framework-0.0.7/src/sh1106_framework/framework/states/state.py` & `sh1106_framework-0.0.8/src/sh1106_framework/framework/states/state.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.7/src/sh1106_framework/framework/states/state_manager.py` & `sh1106_framework-0.0.8/src/sh1106_framework/framework/states/state_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from graphics.drawing import Drawing
-from framework.states.state import State
+from ...graphics.drawing import Drawing
+from .state import State
 
 class StateManager:
     """
     The state manager is responsible for managing the state of the application.
     It handles the initialization, entering, updating, and rendering of the
     current state. These are done automatically by the SH1106Framework, however
     the user can manually set the state using the set_state and pop methods.
```

### Comparing `sh1106_framework-0.0.7/src/sh1106_framework/graphics/drawing.py` & `sh1106_framework-0.0.8/src/sh1106_framework/graphics/drawing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from luma.core.interface.serial import i2c
 from luma.oled.device import sh1106
 
 from PIL import Image
 import time
 
-from graphics.fonts import Fonts
-from graphics.images import Images
+from .fonts import Fonts
+from .images import Images
 
 class Drawing:
     """
     A drawing class for the SH1106 OLED screen. It handles drawing pixels, text, shapes, and images.
     """
     
     __lcdserial: i2c = None
```

### Comparing `sh1106_framework-0.0.7/src/sh1106_framework/graphics/images.py` & `sh1106_framework-0.0.8/src/sh1106_framework/graphics/images.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import os
 import json
 from pathlib import Path
 
-from graphics.drawing import Drawing
+from .drawing import Drawing
 
 class Images:
     __images = {}
     
     @staticmethod
     def _register_images(filepath: str) -> None:
         filename = Path(filepath).stem
```

### Comparing `sh1106_framework-0.0.7/tests/ping-pong/ping-pong.py` & `sh1106_framework-0.0.8/tests/ping-pong/ping-pong.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.7/tests/ping-pong/ping.py` & `sh1106_framework-0.0.8/tests/ping-pong/ping.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.7/tests/ping-pong/pong.py` & `sh1106_framework-0.0.8/tests/ping-pong/pong.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.7/useful-assets/default-font.json` & `sh1106_framework-0.0.8/useful-assets/default-font.json`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.7/useful-assets/default-font.png` & `sh1106_framework-0.0.8/useful-assets/default-font.png`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.7/useful-assets/example-images.png` & `sh1106_framework-0.0.8/useful-assets/example-images.png`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.7/LICENSE` & `sh1106_framework-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.7/README.md` & `sh1106_framework-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.7/pyproject.toml` & `sh1106_framework-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   "src/sh1106_framework/**/*.py",
   "tests/**/*.py",
   "useful-assets/*"
 ]
 
 [project]
 name = "sh1106_framework"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Dan Convey", email="author@example.com" },
 ]
 license = { text = "Apache License 2.0" }
 description = "A state manager, graphics, image, and custom font drawing package for the SH1106 OLED screen based on the luma.oled package. It works with Raspberry Pi and other Linux-based single-board computers."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `sh1106_framework-0.0.7/PKG-INFO` & `sh1106_framework-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sh1106_framework
-Version: 0.0.7
+Version: 0.0.8
 Summary: A state manager, graphics, image, and custom font drawing package for the SH1106 OLED screen based on the luma.oled package. It works with Raspberry Pi and other Linux-based single-board computers.
 Project-URL: Homepage, https://github.com/danspage/sh1106-framework
 Project-URL: Issues, https://github.com/danspage/sh1106-framework/issues
 Author-email: Dan Convey <author@example.com>
 License: Apache License 2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
```


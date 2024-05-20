# Comparing `tmp/sh1106_framework-0.0.6.tar.gz` & `tmp/sh1106_framework-0.0.7.tar.gz`

## Comparing `sh1106_framework-0.0.6.tar` & `sh1106_framework-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/setup.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/__init__.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/sh1106_font_generator.py
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/sh1106_framework.py
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/sh1106_image_generator.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/firmware/main.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/framework/constants.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/framework/states/state.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/framework/states/state_manager.py
--rw-r--r--   0        0        0    11500 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/graphics/drawing.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/graphics/fonts.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/graphics/images.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/tests/ping-pong/ping-pong.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/tests/ping-pong/ping.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/tests/ping-pong/pong.py
--rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/useful-assets/default-font.json
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/useful-assets/default-font.png
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/useful-assets/example-images.json
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/useful-assets/example-images.png
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/LICENSE
--rw-r--r--   0        0        0     7561 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/README.md
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     8372 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/setup.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/__init__.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/sh1106_font_generator.py
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/sh1106_framework.py
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/sh1106_image_generator.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/firmware/main.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/framework/constants.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/framework/states/state.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/framework/states/state_manager.py
+-rw-r--r--   0        0        0    11500 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/graphics/drawing.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/graphics/fonts.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/src/sh1106_framework/graphics/images.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/tests/ping-pong/ping-pong.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/tests/ping-pong/ping.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/tests/ping-pong/pong.py
+-rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/useful-assets/default-font.json
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/useful-assets/default-font.png
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/useful-assets/example-images.json
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/useful-assets/example-images.png
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/LICENSE
+-rw-r--r--   0        0        0     8731 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/README.md
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     9542 2020-02-02 00:00:00.000000 sh1106_framework-0.0.7/PKG-INFO
```

### Comparing `sh1106_framework-0.0.6/setup.py` & `sh1106_framework-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sh1106_framework',
-    version='0.0.6',
+    version='0.0.7',
     author='Dan Convey',
     description='A state manager, graphics, image, and custom font drawing package for the SH1106 OLED screen based on the luma.oled package. It works with Raspberry Pi and other Linux-based single-board computers.',
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `sh1106_framework-0.0.6/src/sh1106_framework/sh1106_font_generator.py` & `sh1106_framework-0.0.7/src/sh1106_framework/sh1106_font_generator.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.6/src/sh1106_framework/sh1106_framework.py` & `sh1106_framework-0.0.7/src/sh1106_framework/sh1106_framework.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.6/src/sh1106_framework/sh1106_image_generator.py` & `sh1106_framework-0.0.7/src/sh1106_framework/sh1106_image_generator.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.6/src/sh1106_framework/firmware/main.py` & `sh1106_framework-0.0.7/src/sh1106_framework/firmware/main.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.6/src/sh1106_framework/framework/states/state.py` & `sh1106_framework-0.0.7/src/sh1106_framework/framework/states/state.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.6/src/sh1106_framework/framework/states/state_manager.py` & `sh1106_framework-0.0.7/src/sh1106_framework/framework/states/state_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
         
         # Initializes the default route afterwards
         StateManager.__states[StateManager.__current_state].initialized = True
         StateManager.__states[StateManager.__current_state].init()
         
     @staticmethod
-    def set_state(route_name):
+    def set_route(route_name):
         """
         Sets the current state to the given route name.
         
         Parameters
         ----------
         route_name: str
             The name of the route to set the current state to.
@@ -47,15 +47,15 @@
         
     @staticmethod
     def pop():
         """
         Sets the current state to the previous state. Nothing happens if there is
         no previous state.
         """
-        StateManager.set_state(StateManager.__previous_state)
+        StateManager.set_route(StateManager.__previous_state)
     
     @staticmethod
     def _update(dt):
         StateManager.__states[StateManager.__current_state].update(dt)
     
     @staticmethod
     def _render():
```

### Comparing `sh1106_framework-0.0.6/src/sh1106_framework/graphics/drawing.py` & `sh1106_framework-0.0.7/src/sh1106_framework/graphics/drawing.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.6/src/sh1106_framework/graphics/images.py` & `sh1106_framework-0.0.7/src/sh1106_framework/graphics/images.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.6/tests/ping-pong/ping.py` & `sh1106_framework-0.0.7/tests/ping-pong/ping.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from src.sh1106_framework.framework.states.state import State
-from src.sh1106_framework.graphics.drawing import Drawing
+from sh1106_framework import Drawing, State
 
 import time
 
 class PingPage(State):
     def __init__(self, state_manager):
         self.state_manager = state_manager
     
@@ -14,12 +13,12 @@
         self.time_of_start = time.time()
 
     def handle_input(self, channel, message):
         pass
 
     def update(self, dt):
         if time.time() - self.time_of_start > 1:
-            self.state_manager.set_state("pong")
+            self.state_manager.set_route("pong")
 
     def render(self):
         Drawing.draw_image("weather-rain", 0, 0)
         Drawing.draw_text("Ping", 14, 0)
```

### Comparing `sh1106_framework-0.0.6/tests/ping-pong/pong.py` & `sh1106_framework-0.0.7/tests/ping-pong/pong.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-from src.sh1106_framework.framework.states.state import State
-from src.sh1106_framework.graphics.drawing import Drawing
+from sh1106_framework import Drawing, State
 
 import time
 
-class PingPage(State):
+class PongPage(State):
     def __init__(self, state_manager):
         self.state_manager = state_manager
     
     def init(self):
         pass
 
     def enter(self):
         self.time_of_start = time.time()
 
     def handle_input(self, channel, message):
         pass
 
     def update(self, dt):
         if time.time() - self.time_of_start > 1:
-            self.state_manager.set_state("ping")
+            self.state_manager.set_route("ping")
 
     def render(self):
         Drawing.draw_image("weather-storm", 0, 0)
         Drawing.draw_text("Pong", 14, 0)
```

### Comparing `sh1106_framework-0.0.6/useful-assets/default-font.json` & `sh1106_framework-0.0.7/useful-assets/default-font.json`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.6/useful-assets/default-font.png` & `sh1106_framework-0.0.7/useful-assets/default-font.png`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.6/useful-assets/example-images.png` & `sh1106_framework-0.0.7/useful-assets/example-images.png`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.6/LICENSE` & `sh1106_framework-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.6/README.md` & `sh1106_framework-0.0.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 A state manager, graphics, image, and custom font drawing package for the SH1106 OLED screen based on the luma.oled package. It works with Raspberry Pi and other Linux-based single-board computers.
 
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Features](#features)
 - [Installation](#installation)
+- [Tools](#tools)
+  - [Image utility](#image-utility)
+  - [Font utility](#font-utility)
+
 - [Usage](#usage)
   - [Basic Usage](#basic-usage)
   - [State Management](#state-management)
   - [Drawing Graphics](#drawing-graphics)
-  - [Custom Fonts](#custom-fonts)
-- [Examples](#examples)
-- [Contributing](#contributing)
+
 - [License](#license)
-- [Contact](#contact)
 
 ## Introduction
 
 This package provides a comprehensive solution for managing states, drawing graphics, images, and custom fonts on the SH1106 OLED screen. It leverages the capabilities of the luma.oled package to offer an easy-to-use interface for Raspberry Pi and other Linux-based single-board computers.
 
 ## Features
 
@@ -39,15 +40,15 @@
 
 ## Tools
 
 The package doesn't directly load image files for images and fonts, but instead uses custom JSON bitmap files.
 
 This package comes with two tools: an image utility and a font utility. These take user-supplied image files containing bitmaps, and convert them to json files which the framework can load. This process is split apart from the framework itself in order to reduce load time.
 
-#### Image utility:
+#### Image Utility:
 
 The image utility can be accessed with the `sh1106_image_generator` command. It takes in a reference image, which contains one or more bitmaps within itself, and a JSON reference file, containing information about the names of the images for the framework to reference, along with their coordinates and sizes in the reference image.
 
 The reference image can be of any size. Since the SH1106 display is monochromatic, each pixel only has a state of being on or off. In the reference image, an opaque white pixel represents a pixel being on, and any other color represents the pixel being off.
 
 An example image can be found [here](https://github.com/danspage/sh1106-framework/blob/main/useful-assets/example-images.png), and its corresponding JSON file can be found [here](https://github.com/danspage/sh1106-framework/blob/main/useful-assets/example-images.json).
 
@@ -60,48 +61,55 @@
 To generate an output JSON file for the images, use the following terminal command:
 ```bash
 sh1006_terminal_generator -i/--image <path to reference image> -j/--json <path to reference JSON> -o/--output <path to output file>
 ```
 
 Then you'll use the output JSON file for initializing images when the framework is loading.
 
-#### Font utility:
+#### Font Utility:
 
 The font utility works the exact same as the image utility, except with the `sh1106_font_generator` command instead. Instead of using names for each entry, use the character that you want to assign to the sub-image. The name of the font will be set manually via code upon initialization. The default font that you'll most likely want to include can be found here: [Image](https://github.com/danspage/sh1106-framework/blob/main/useful-assets/default-font.png), [JSON](https://github.com/danspage/sh1106-framework/blob/main/useful-assets/default-font.json)
 
 ## Usage
 
 ### Basic Usage
 
-Here is a simple example of how to initialize the display and draw a basic shape:
+Here is a simple ping-pong page that displays an image, draws some text, and switches between the two pages every second.
+
+<u>ping-pong.py</u>
 
 ```python
-# MAKE SURE TO INCLUDE IMPORT STATEMENTS
+from sh1106_framework import SH1106Framework, StateManager
+from ping import PingPage
+from pong import PongPage
 
 def __init():
     SH1106Framework.register_font("default", "default_font.json")
     SH1106Framework.register_images("icons.json")
     
     SH1106Framework.register_routes(
         default_route="splash",
         routes={
-            "splash": SplashPage(StateManager)
+            "ping": PingPage(StateManager),
+          	"pong": PongPage(StateManager)
         }
     )
     
     # Use the I2C port and address of the display
     SH1106Framework.begin(port=1, address=0x3C)
     pass
     
 if __name__ == "__main__":
     __init()
 ```
 
+<u>ping.py</u>
+
 ```python
-# MAKE SURE TO INCLUDE IMPORT STATEMENTS
+from sh1106_framework import Drawing, State
 
 import time
 
 class PingPage(State):
     def __init__(self, state_manager):
         self.state_manager = state_manager
     
@@ -112,113 +120,117 @@
         self.time_of_start = time.time()
 
     def handle_input(self, channel, message):
         pass
 
     def update(self, dt):
         if time.time() - self.time_of_start > 1:
-            self.state_manager.set_state("pong")
+            self.state_manager.set_route("pong")
 
     def render(self):
         Drawing.draw_image("weather-rain", 0, 0)
         Drawing.draw_text("Ping", 14, 0)
 ```
 
+<u>pong.py</u>
+
 ```python
-# MAKE SURE TO INCLUDE IMPORT STATEMENTS
+from sh1106_framework import Drawing, State
 
 import time
 
-class PingPage(State):
+class PongPage(State):
     def __init__(self, state_manager):
         self.state_manager = state_manager
     
     def init(self):
         pass
 
     def enter(self):
         self.time_of_start = time.time()
 
     def handle_input(self, channel, message):
         pass
 
     def update(self, dt):
         if time.time() - self.time_of_start > 1:
-            self.state_manager.set_state("ping")
+            self.state_manager.set_route("ping")
 
     def render(self):
         Drawing.draw_image("weather-storm", 0, 0)
         Drawing.draw_text("Pong", 14, 0)
 ```
 
 ### State Management
 
-Managing different application states can be done as follows:
+The state manager handles various states (which can be thought of as pages) that are referred to with strings (called routes) that they've been associated with. In the example above, "ping" has been assigned to a "PingPage" state and "pong" has been assigned to a "PongPage" state.
+
+Notice in the example how they're set up in the main file:
 
 ```python
-from sh1106_oled import StateManager
+SH1106Framework.register_routes(
+      default_route="splash",
+      routes={
+          "ping": PingPage(StateManager),
+          "pong": PongPage(StateManager)
+      }
+  )
+```
 
-# Initialize the state manager
-state_manager = StateManager()
 
-# Define states
-def home_screen():
-    # Draw home screen content
-    pass
 
-def settings_screen():
-    # Draw settings screen content
-    pass
+User-created states should follow this template, extending the State class:
 
-# Register states
-state_manager.add_state("home", home_screen)
-state_manager.add_state("settings", settings_screen)
+```python
+from sh1106_framework import State
 
-# Switch to a state
-state_manager.switch_state("home")
-```
+class MyCustomState(State):
+    def __init__(self, state_manager):
+     		# This line is required
+        self.state_manager = state_manager
+    
+    def init(self):
+        # Initialization code
 
-### Drawing Graphics
+    def enter(self):
+        # State entered code
 
-You can draw various graphics like lines, circles, and rectangles:
+    def update(self, dt):
+        # Update code, runs approximately 60 times per second
 
-```python
-# Draw a line
-display.line((0, 0, 128, 64), fill="white")
+    def render(self):
+        # Render code
+```
 
-# Draw a circle
-display.circle((64, 32), 20, outline="white")
+Within the states, you can use the methods `self.state_manager.set_route(route name)` and `self.state_manager.pop()` to set the current state or to go to the previous state.
 
-display.show()
-```
+### Drawing Graphics
 
-### Custom Fonts
+You can draw various graphics like lines, images, rectangles, and strings, as well as set individual pixels. This should be done within the render method of a state. Note that where color is mentioned, it should be either 0 or 1, with 0 representing an unlit pixel and 1 representing a lit pixel.
 
-To draw text with custom fonts:
+The screen will be automatically cleared before each render method is run.
 
 ```python
-from PIL import ImageFont
+from sh1106_framework import Drawing
 
-# Load a custom font
-font = ImageFont.truetype("path/to/font.ttf", 16)
+# Draw rectangle
+Drawing.draw_rect(x, y, width, height, color=1)
 
-# Draw text
-display.text((10, 10), "Hello, World!", font=font, fill="white")
-
-display.show()
-```
+# Draw outlined rectangle
+Drawing.draw_outlined_rect(x, y, width, height, color=1)
 
-## Examples
+# Draw line
+Drawing.draw_line(x0, y0, x1, y1, color=1)
 
-Check the [examples directory](examples/) for more detailed examples and use cases.
+# Set pixel
+Drawing.set_pixel(x, y, color)
 
-## Contributing
+# Draw text (using font names defined in the main file)
+Drawing.draw_text(text, x, y, color=1, font="default", scale=1, centered=False)
 
-Contributions are welcome! Please read the [contributing guidelines](CONTRIBUTING.md) first.
+# Draw image (using image names defined in the reference JSON files)
+Drawing.draw_image(image_name, x, y, color=1, scale=1, centered_horizontal=False, centered_vertical=False)
+```
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
-
-## Contact
-
-For any questions or feedback, please contact [Your Name](mailto:your.email@example.com).
+This project is licensed under the Apache License 2.0 - see the [LICENSE](https://github.com/danspage/sh1106-framework/blob/main/LICENSE) file for details.
```

### Comparing `sh1106_framework-0.0.6/pyproject.toml` & `sh1106_framework-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   "src/sh1106_framework/**/*.py",
   "tests/**/*.py",
   "useful-assets/*"
 ]
 
 [project]
 name = "sh1106_framework"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Dan Convey", email="author@example.com" },
 ]
 license = { text = "Apache License 2.0" }
 description = "A state manager, graphics, image, and custom font drawing package for the SH1106 OLED screen based on the luma.oled package. It works with Raspberry Pi and other Linux-based single-board computers."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `sh1106_framework-0.0.6/PKG-INFO` & `sh1106_framework-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sh1106_framework
-Version: 0.0.6
+Version: 0.0.7
 Summary: A state manager, graphics, image, and custom font drawing package for the SH1106 OLED screen based on the luma.oled package. It works with Raspberry Pi and other Linux-based single-board computers.
 Project-URL: Homepage, https://github.com/danspage/sh1106-framework
 Project-URL: Issues, https://github.com/danspage/sh1106-framework/issues
 Author-email: Dan Convey <author@example.com>
 License: Apache License 2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,23 +21,24 @@
 A state manager, graphics, image, and custom font drawing package for the SH1106 OLED screen based on the luma.oled package. It works with Raspberry Pi and other Linux-based single-board computers.
 
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Features](#features)
 - [Installation](#installation)
+- [Tools](#tools)
+  - [Image utility](#image-utility)
+  - [Font utility](#font-utility)
+
 - [Usage](#usage)
   - [Basic Usage](#basic-usage)
   - [State Management](#state-management)
   - [Drawing Graphics](#drawing-graphics)
-  - [Custom Fonts](#custom-fonts)
-- [Examples](#examples)
-- [Contributing](#contributing)
+
 - [License](#license)
-- [Contact](#contact)
 
 ## Introduction
 
 This package provides a comprehensive solution for managing states, drawing graphics, images, and custom fonts on the SH1106 OLED screen. It leverages the capabilities of the luma.oled package to offer an easy-to-use interface for Raspberry Pi and other Linux-based single-board computers.
 
 ## Features
 
@@ -56,15 +57,15 @@
 
 ## Tools
 
 The package doesn't directly load image files for images and fonts, but instead uses custom JSON bitmap files.
 
 This package comes with two tools: an image utility and a font utility. These take user-supplied image files containing bitmaps, and convert them to json files which the framework can load. This process is split apart from the framework itself in order to reduce load time.
 
-#### Image utility:
+#### Image Utility:
 
 The image utility can be accessed with the `sh1106_image_generator` command. It takes in a reference image, which contains one or more bitmaps within itself, and a JSON reference file, containing information about the names of the images for the framework to reference, along with their coordinates and sizes in the reference image.
 
 The reference image can be of any size. Since the SH1106 display is monochromatic, each pixel only has a state of being on or off. In the reference image, an opaque white pixel represents a pixel being on, and any other color represents the pixel being off.
 
 An example image can be found [here](https://github.com/danspage/sh1106-framework/blob/main/useful-assets/example-images.png), and its corresponding JSON file can be found [here](https://github.com/danspage/sh1106-framework/blob/main/useful-assets/example-images.json).
 
@@ -77,48 +78,55 @@
 To generate an output JSON file for the images, use the following terminal command:
 ```bash
 sh1006_terminal_generator -i/--image <path to reference image> -j/--json <path to reference JSON> -o/--output <path to output file>
 ```
 
 Then you'll use the output JSON file for initializing images when the framework is loading.
 
-#### Font utility:
+#### Font Utility:
 
 The font utility works the exact same as the image utility, except with the `sh1106_font_generator` command instead. Instead of using names for each entry, use the character that you want to assign to the sub-image. The name of the font will be set manually via code upon initialization. The default font that you'll most likely want to include can be found here: [Image](https://github.com/danspage/sh1106-framework/blob/main/useful-assets/default-font.png), [JSON](https://github.com/danspage/sh1106-framework/blob/main/useful-assets/default-font.json)
 
 ## Usage
 
 ### Basic Usage
 
-Here is a simple example of how to initialize the display and draw a basic shape:
+Here is a simple ping-pong page that displays an image, draws some text, and switches between the two pages every second.
+
+<u>ping-pong.py</u>
 
 ```python
-# MAKE SURE TO INCLUDE IMPORT STATEMENTS
+from sh1106_framework import SH1106Framework, StateManager
+from ping import PingPage
+from pong import PongPage
 
 def __init():
     SH1106Framework.register_font("default", "default_font.json")
     SH1106Framework.register_images("icons.json")
     
     SH1106Framework.register_routes(
         default_route="splash",
         routes={
-            "splash": SplashPage(StateManager)
+            "ping": PingPage(StateManager),
+          	"pong": PongPage(StateManager)
         }
     )
     
     # Use the I2C port and address of the display
     SH1106Framework.begin(port=1, address=0x3C)
     pass
     
 if __name__ == "__main__":
     __init()
 ```
 
+<u>ping.py</u>
+
 ```python
-# MAKE SURE TO INCLUDE IMPORT STATEMENTS
+from sh1106_framework import Drawing, State
 
 import time
 
 class PingPage(State):
     def __init__(self, state_manager):
         self.state_manager = state_manager
     
@@ -129,113 +137,117 @@
         self.time_of_start = time.time()
 
     def handle_input(self, channel, message):
         pass
 
     def update(self, dt):
         if time.time() - self.time_of_start > 1:
-            self.state_manager.set_state("pong")
+            self.state_manager.set_route("pong")
 
     def render(self):
         Drawing.draw_image("weather-rain", 0, 0)
         Drawing.draw_text("Ping", 14, 0)
 ```
 
+<u>pong.py</u>
+
 ```python
-# MAKE SURE TO INCLUDE IMPORT STATEMENTS
+from sh1106_framework import Drawing, State
 
 import time
 
-class PingPage(State):
+class PongPage(State):
     def __init__(self, state_manager):
         self.state_manager = state_manager
     
     def init(self):
         pass
 
     def enter(self):
         self.time_of_start = time.time()
 
     def handle_input(self, channel, message):
         pass
 
     def update(self, dt):
         if time.time() - self.time_of_start > 1:
-            self.state_manager.set_state("ping")
+            self.state_manager.set_route("ping")
 
     def render(self):
         Drawing.draw_image("weather-storm", 0, 0)
         Drawing.draw_text("Pong", 14, 0)
 ```
 
 ### State Management
 
-Managing different application states can be done as follows:
+The state manager handles various states (which can be thought of as pages) that are referred to with strings (called routes) that they've been associated with. In the example above, "ping" has been assigned to a "PingPage" state and "pong" has been assigned to a "PongPage" state.
+
+Notice in the example how they're set up in the main file:
 
 ```python
-from sh1106_oled import StateManager
+SH1106Framework.register_routes(
+      default_route="splash",
+      routes={
+          "ping": PingPage(StateManager),
+          "pong": PongPage(StateManager)
+      }
+  )
+```
 
-# Initialize the state manager
-state_manager = StateManager()
 
-# Define states
-def home_screen():
-    # Draw home screen content
-    pass
 
-def settings_screen():
-    # Draw settings screen content
-    pass
+User-created states should follow this template, extending the State class:
 
-# Register states
-state_manager.add_state("home", home_screen)
-state_manager.add_state("settings", settings_screen)
+```python
+from sh1106_framework import State
 
-# Switch to a state
-state_manager.switch_state("home")
-```
+class MyCustomState(State):
+    def __init__(self, state_manager):
+     		# This line is required
+        self.state_manager = state_manager
+    
+    def init(self):
+        # Initialization code
 
-### Drawing Graphics
+    def enter(self):
+        # State entered code
 
-You can draw various graphics like lines, circles, and rectangles:
+    def update(self, dt):
+        # Update code, runs approximately 60 times per second
 
-```python
-# Draw a line
-display.line((0, 0, 128, 64), fill="white")
+    def render(self):
+        # Render code
+```
 
-# Draw a circle
-display.circle((64, 32), 20, outline="white")
+Within the states, you can use the methods `self.state_manager.set_route(route name)` and `self.state_manager.pop()` to set the current state or to go to the previous state.
 
-display.show()
-```
+### Drawing Graphics
 
-### Custom Fonts
+You can draw various graphics like lines, images, rectangles, and strings, as well as set individual pixels. This should be done within the render method of a state. Note that where color is mentioned, it should be either 0 or 1, with 0 representing an unlit pixel and 1 representing a lit pixel.
 
-To draw text with custom fonts:
+The screen will be automatically cleared before each render method is run.
 
 ```python
-from PIL import ImageFont
+from sh1106_framework import Drawing
 
-# Load a custom font
-font = ImageFont.truetype("path/to/font.ttf", 16)
+# Draw rectangle
+Drawing.draw_rect(x, y, width, height, color=1)
 
-# Draw text
-display.text((10, 10), "Hello, World!", font=font, fill="white")
-
-display.show()
-```
+# Draw outlined rectangle
+Drawing.draw_outlined_rect(x, y, width, height, color=1)
 
-## Examples
+# Draw line
+Drawing.draw_line(x0, y0, x1, y1, color=1)
 
-Check the [examples directory](examples/) for more detailed examples and use cases.
+# Set pixel
+Drawing.set_pixel(x, y, color)
 
-## Contributing
+# Draw text (using font names defined in the main file)
+Drawing.draw_text(text, x, y, color=1, font="default", scale=1, centered=False)
 
-Contributions are welcome! Please read the [contributing guidelines](CONTRIBUTING.md) first.
+# Draw image (using image names defined in the reference JSON files)
+Drawing.draw_image(image_name, x, y, color=1, scale=1, centered_horizontal=False, centered_vertical=False)
+```
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
-
-## Contact
-
-For any questions or feedback, please contact [Your Name](mailto:your.email@example.com).
+This project is licensed under the Apache License 2.0 - see the [LICENSE](https://github.com/danspage/sh1106-framework/blob/main/LICENSE) file for details.
```


# Comparing `tmp/sh1106_framework-0.0.5.tar.gz` & `tmp/sh1106_framework-0.0.6.tar.gz`

## Comparing `sh1106_framework-0.0.5.tar` & `sh1106_framework-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/setup.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/src/sh1106_framework/__init__.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/src/sh1106_framework/sh1106_font_generator.py
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/src/sh1106_framework/sh1106_framework.py
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/src/sh1106_framework/sh1106_image_generator.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/src/sh1106_framework/firmware/main.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/src/sh1106_framework/framework/constants.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/src/sh1106_framework/framework/states/state.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/src/sh1106_framework/framework/states/state_manager.py
--rw-r--r--   0        0        0    11500 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/src/sh1106_framework/graphics/drawing.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/src/sh1106_framework/graphics/fonts.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/src/sh1106_framework/graphics/images.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/tests/ping-pong/ping-pong.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/tests/ping-pong/ping.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/tests/ping-pong/pong.py
--rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/useful-assets/default-font.json
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/useful-assets/default-font.png
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/useful-assets/example-images.json
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/useful-assets/example-images.png
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/LICENSE
--rw-r--r--   0        0        0     7561 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/README.md
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     8372 2020-02-02 00:00:00.000000 sh1106_framework-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/setup.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/__init__.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/sh1106_font_generator.py
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/sh1106_framework.py
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/sh1106_image_generator.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/firmware/main.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/framework/constants.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/framework/states/state.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/framework/states/state_manager.py
+-rw-r--r--   0        0        0    11500 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/graphics/drawing.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/graphics/fonts.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/src/sh1106_framework/graphics/images.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/tests/ping-pong/ping-pong.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/tests/ping-pong/ping.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/tests/ping-pong/pong.py
+-rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/useful-assets/default-font.json
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/useful-assets/default-font.png
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/useful-assets/example-images.json
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/useful-assets/example-images.png
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/LICENSE
+-rw-r--r--   0        0        0     7561 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/README.md
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     8372 2020-02-02 00:00:00.000000 sh1106_framework-0.0.6/PKG-INFO
```

### Comparing `sh1106_framework-0.0.5/setup.py` & `sh1106_framework-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sh1106_framework',
-    version='0.0.5',
+    version='0.0.6',
     author='Dan Convey',
     description='A state manager, graphics, image, and custom font drawing package for the SH1106 OLED screen based on the luma.oled package. It works with Raspberry Pi and other Linux-based single-board computers.',
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `sh1106_framework-0.0.5/src/sh1106_framework/sh1106_font_generator.py` & `sh1106_framework-0.0.6/src/sh1106_framework/sh1106_font_generator.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.5/src/sh1106_framework/sh1106_framework.py` & `sh1106_framework-0.0.6/src/sh1106_framework/sh1106_framework.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.5/src/sh1106_framework/sh1106_image_generator.py` & `sh1106_framework-0.0.6/src/sh1106_framework/sh1106_image_generator.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.5/src/sh1106_framework/firmware/main.py` & `sh1106_framework-0.0.6/src/sh1106_framework/firmware/main.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.5/src/sh1106_framework/framework/states/state.py` & `sh1106_framework-0.0.6/src/sh1106_framework/framework/states/state.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.5/src/sh1106_framework/framework/states/state_manager.py` & `sh1106_framework-0.0.6/src/sh1106_framework/framework/states/state_manager.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.5/src/sh1106_framework/graphics/drawing.py` & `sh1106_framework-0.0.6/src/sh1106_framework/graphics/drawing.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.5/src/sh1106_framework/graphics/images.py` & `sh1106_framework-0.0.6/src/sh1106_framework/graphics/images.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.5/tests/ping-pong/ping-pong.py` & `sh1106_framework-0.0.6/tests/ping-pong/ping-pong.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.5/tests/ping-pong/ping.py` & `sh1106_framework-0.0.6/tests/ping-pong/ping.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.5/tests/ping-pong/pong.py` & `sh1106_framework-0.0.6/tests/ping-pong/pong.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.5/useful-assets/default-font.json` & `sh1106_framework-0.0.6/useful-assets/default-font.json`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.5/useful-assets/default-font.png` & `sh1106_framework-0.0.6/useful-assets/default-font.png`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.5/useful-assets/example-images.png` & `sh1106_framework-0.0.6/useful-assets/example-images.png`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.5/LICENSE` & `sh1106_framework-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.5/README.md` & `sh1106_framework-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.5/pyproject.toml` & `sh1106_framework-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   "src/sh1106_framework/**/*.py",
   "tests/**/*.py",
   "useful-assets/*"
 ]
 
 [project]
 name = "sh1106_framework"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Dan Convey", email="author@example.com" },
 ]
 license = { text = "Apache License 2.0" }
 description = "A state manager, graphics, image, and custom font drawing package for the SH1106 OLED screen based on the luma.oled package. It works with Raspberry Pi and other Linux-based single-board computers."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `sh1106_framework-0.0.5/PKG-INFO` & `sh1106_framework-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sh1106_framework
-Version: 0.0.5
+Version: 0.0.6
 Summary: A state manager, graphics, image, and custom font drawing package for the SH1106 OLED screen based on the luma.oled package. It works with Raspberry Pi and other Linux-based single-board computers.
 Project-URL: Homepage, https://github.com/danspage/sh1106-framework
 Project-URL: Issues, https://github.com/danspage/sh1106-framework/issues
 Author-email: Dan Convey <author@example.com>
 License: Apache License 2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
```


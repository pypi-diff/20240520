# Comparing `tmp/svg2gcode-3.2.5.tar.gz` & `tmp/svg2gcode-3.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svg2gcode-3.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "svg2gcode-3.2.6.tar", last modified: Mon May 20 20:35:41 2024, max compression
```

## Comparing `svg2gcode-3.2.5.tar` & `svg2gcode-3.2.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    32422 2023-06-11 09:44:38.507409 svg2gcode-3.2.5/LICENSE
--rw-r--r--   0        0        0    13542 2024-02-07 15:56:59.876028 svg2gcode-3.2.5/README.md
--rw-r--r--   0        0        0      692 2024-02-07 15:42:18.579811 svg2gcode-3.2.5/pyproject.toml
--rw-r--r--   0        0        0       98 2024-02-07 15:57:28.916569 svg2gcode-3.2.5/svg2gcode/__init__.py
--rw-r--r--   0        0        0     9336 2024-02-07 15:43:28.961082 svg2gcode-3.2.5/svg2gcode/__main__.py
--rw-r--r--   0        0        0     1068 2023-12-02 21:51:39.266834 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/LICENSE
--rw-r--r--   0        0        0     9315 2024-01-08 19:17:21.077901 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/__init__.py
--rw-r--r--   0        0        0      145 2023-12-02 21:51:40.256852 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/compiler/__init__.py
--rw-r--r--   0        0        0    48541 2024-02-07 15:44:36.222302 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/compiler/_compiler.py
--rw-r--r--   0        0        0      249 2023-12-02 21:51:40.986866 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/compiler/interfaces/__init__.py
--rw-r--r--   0        0        0     5895 2023-12-02 21:51:41.056867 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/compiler/interfaces/_abstract_interface.py
--rw-r--r--   0        0        0     1180 2023-12-02 21:51:41.036867 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/compiler/interfaces/_fan_controlled_gcode.py
--rw-r--r--   0        0        0     9499 2023-12-02 21:51:41.016867 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/compiler/interfaces/_gcode.py
--rw-r--r--   0        0        0    15312 2024-01-08 19:18:10.798837 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/css_color.py
--rw-r--r--   0        0        0     5211 2024-01-08 19:18:54.599662 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/formulas.py
--rw-r--r--   0        0        0     1357 2023-12-02 21:51:39.786844 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/__init__.py
--rw-r--r--   0        0        0     3439 2023-12-02 21:51:39.766843 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_abstract_chain.py
--rw-r--r--   0        0        0     3117 2023-12-02 21:51:39.966847 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_abstract_curve.py
--rw-r--r--   0        0        0     3066 2023-12-02 21:51:39.876845 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_circular_arc.py
--rw-r--r--   0        0        0     1176 2023-12-02 21:51:39.816844 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_cubic_bazier.py
--rw-r--r--   0        0        0     2474 2024-01-08 19:29:33.863567 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_elliptical_arc.py
--rw-r--r--   0        0        0     4115 2024-01-08 19:31:40.116485 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_line.py
--rw-r--r--   0        0        0     5526 2024-01-08 19:32:19.677379 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_line_segment_chain.py
--rw-r--r--   0        0        0     3171 2023-12-02 21:51:39.946847 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_matrix.py
--rw-r--r--   0        0        0     1065 2023-12-02 21:51:39.746843 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_quadratic_bazier.py
--rw-r--r--   0        0        0     1095 2023-12-02 21:51:39.836845 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_raster_image.py
--rw-r--r--   0        0        0     2487 2023-12-02 21:51:39.926846 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_smooth_arc_chain.py
--rw-r--r--   0        0        0     1583 2023-12-02 21:51:39.906846 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_vector.py
--rw-r--r--   0        0        0      601 2023-12-02 21:51:39.506839 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/svg_parser/__init__.py
--rw-r--r--   0        0        0    11956 2023-12-02 21:51:39.496838 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/svg_parser/_parser_methods.py
--rw-r--r--   0        0        0    13678 2024-01-08 19:21:51.262986 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/svg_parser/_path.py
--rw-r--r--   0        0        0     5673 2023-12-02 21:51:39.446838 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/svg_parser/_transformation.py
--rw-r--r--   0        0        0     2440 2023-12-02 21:51:39.466838 svg2gcode-3.2.5/svg2gcode/svg_to_gcode/svg_parser/debug_methods.py
--rw-r--r--   0        0        0    14099 1970-01-01 00:00:00.000000 svg2gcode-3.2.5/PKG-INFO
+-rw-r--r--   0        0        0    32422 2023-06-11 09:44:38.000000 svg2gcode-3.2.6/LICENSE
+-rw-r--r--   0        0        0    14279 2024-05-20 20:33:44.175881 svg2gcode-3.2.6/README.md
+-rw-r--r--   0        0        0      692 2024-02-07 15:42:18.000000 svg2gcode-3.2.6/pyproject.toml
+-rw-r--r--   0        0        0       98 2024-05-20 20:34:36.035656 svg2gcode-3.2.6/svg2gcode/__init__.py
+-rw-r--r--   0        0        0     9346 2024-05-20 20:34:53.971578 svg2gcode-3.2.6/svg2gcode/__main__.py
+-rw-r--r--   0        0        0     1068 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/LICENSE
+-rw-r--r--   0        0        0     9315 2024-01-08 19:17:21.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/__init__.py
+-rw-r--r--   0        0        0      145 2023-12-02 21:51:40.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/compiler/__init__.py
+-rw-r--r--   0        0        0    48541 2024-02-07 15:44:36.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/compiler/_compiler.py
+-rw-r--r--   0        0        0      249 2023-12-02 21:51:40.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/compiler/interfaces/__init__.py
+-rw-r--r--   0        0        0     5895 2023-12-02 21:51:41.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/compiler/interfaces/_abstract_interface.py
+-rw-r--r--   0        0        0     1180 2023-12-02 21:51:41.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/compiler/interfaces/_fan_controlled_gcode.py
+-rw-r--r--   0        0        0     9499 2023-12-02 21:51:41.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/compiler/interfaces/_gcode.py
+-rw-r--r--   0        0        0    15312 2024-01-08 19:18:10.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/css_color.py
+-rw-r--r--   0        0        0     5211 2024-01-08 19:18:54.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/formulas.py
+-rw-r--r--   0        0        0     1357 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/__init__.py
+-rw-r--r--   0        0        0     3439 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_abstract_chain.py
+-rw-r--r--   0        0        0     3117 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_abstract_curve.py
+-rw-r--r--   0        0        0     3066 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_circular_arc.py
+-rw-r--r--   0        0        0     1176 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_cubic_bazier.py
+-rw-r--r--   0        0        0     2474 2024-01-08 19:29:33.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_elliptical_arc.py
+-rw-r--r--   0        0        0     4115 2024-01-08 19:31:40.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_line.py
+-rw-r--r--   0        0        0     5526 2024-01-08 19:32:19.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_line_segment_chain.py
+-rw-r--r--   0        0        0     3171 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_matrix.py
+-rw-r--r--   0        0        0     1065 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_quadratic_bazier.py
+-rw-r--r--   0        0        0     1095 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_raster_image.py
+-rw-r--r--   0        0        0     2487 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_smooth_arc_chain.py
+-rw-r--r--   0        0        0     1583 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_vector.py
+-rw-r--r--   0        0        0      601 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/svg_parser/__init__.py
+-rw-r--r--   0        0        0    11956 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/svg_parser/_parser_methods.py
+-rw-r--r--   0        0        0    13678 2024-01-08 19:21:51.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/svg_parser/_path.py
+-rw-r--r--   0        0        0     5673 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/svg_parser/_transformation.py
+-rw-r--r--   0        0        0     2440 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/svg_parser/debug_methods.py
+-rw-r--r--   0        0        0    14836 1970-01-01 00:00:00.000000 svg2gcode-3.2.6/PKG-INFO
```

### Comparing `svg2gcode-3.2.5/LICENSE` & `svg2gcode-3.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/README.md` & `svg2gcode-3.2.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -109,15 +109,15 @@
                         cutting depth in mm for one pass, only active for passes > 1
   --rapidmove <default:10>
                         generate G0 moves between shapes, for images: G0 moves when skipping more than 10mm (default), 0 is no G0 moves
   --noise <default:0>   reduces image noise by not emitting pixels with power lower or equal than this setting
   --overscan <default:0>
                         overscan image lines to avoid incorrect power levels for pixels at left and right borders, number in pixels, default off
   --showoverscan        show overscan pixels (note that this is visible and part of the gcode emitted!)
-  --constantburn        use constant burn mode M3 (a bit more dangerous!), instead of dynamic burn mode M4
+  --constantburn        set constant burn mode M3 (default set to dynamic burn mode M4); this enhances engraving quality
   --origin delta-x delta-y
                         translate origin by vector (delta-x,delta-y) in mm (default not set, option --selfcenter cannot be used at the same time)
   --scale factor-x factor-y
                         scale svg with (factor-x,factor-y) (default not set)
   --rotate <default:0>  number of degrees to rotate
   --splitfile           split gcode output of SVG path and image objects
   --pathcut             alway cut SVG path objects! (use laser power set with option --cuttingpower)
@@ -272,13 +272,17 @@
     > svg2gcode --splitfile ambachtmanlogo.svg logo.gc
     > ..
     > ls *.gc 
     > logo.gc             # all drawings
     > logo_images.gc      # all images
 ```   
 
+### Burn mode M3/M4:
+
+Default *svg2gcode* uses dynamic burn mode *M4*. This can be changed by setting option *--constantburn* which selects burn mode *M3*. Mode *M4* is not suitable for engravings because it automatically compensates (laser)power for speed. This conflicts with the specific gcode settings given by *image2gcode* (called by *svg2gcode*) for each pixel. In fact some experiments show that *M4* causes loss of quality and image deterioration when speed is increased. On white oak images had too much black and grey which did not go away for substantially higher speed. When switched back to constant burn (*M3*) mode, the same high speed gave excellent images having a sepia (licht yellow brown) color tone.
+
 ### Notes:
  - drawing objects - within the composer - must be converted to a```path```to be translated to a gcode sequence
  - also, image objects should **not** be converted to a ```path```
  - images must be linked or embedded using base64.
  - images can be in several formats (my tests included *.png* and  *.jpg* image files)
  - SVG source documents must be in unit 'mm' (and set to 1 'user unit' is 1 mm) which is the default for Inkscape (check document settings and look at the 'scaling' parameter)
```

### Comparing `svg2gcode-3.2.5/pyproject.toml` & `svg2gcode-3.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/__main__.py` & `svg2gcode-3.2.6/svg2gcode/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     parser.add_argument('--rapidmove', default=cfg["rapidmove_default"], metavar="<default:" + str(cfg["rapidmove_default"])+ ">",
         type=int, help='generate G0 moves between shapes, for images: G0 moves when skipping more than 10mm (default), 0 is no G0 moves' )
     parser.add_argument('--noise', default=cfg["noise_default"], metavar="<default:" +str(cfg["noise_default"])+ ">",
         type=int, help='reduces image noise by not emitting pixels with power lower or equal than this setting')
     parser.add_argument('--overscan', default=cfg["overscan_default"], metavar="<default:" +str(cfg["overscan_default"])+ ">",
         type=int, help="overscan image lines to avoid incorrect power levels for pixels at left and right borders, number in pixels, default off")
     parser.add_argument('--showoverscan', action='store_true', default=False, help='show overscan pixels (note that this is visible and part of the gcode emitted!)' )
-    parser.add_argument('--constantburn', action='store_true', default=False, help='use constant burn mode M3 (a bit more dangerous!), instead of dynamic burn mode M4')
+    parser.add_argument('--constantburn', action='store_true', default=False, help='set constant burn mode M3 (default is dynamic burn mode M4); this enhances engraving quality')
     parser.add_argument('--origin', default=None, nargs=2, metavar=('delta-x', 'delta-y'),
         type=float, help="translate origin by vector (delta-x,delta-y) in mm (default not set, option --selfcenter cannot be used at the same time)")
     parser.add_argument('--scale', default=None, nargs=2, metavar=('factor-x', 'factor-y'),
         type=float, help="scale svg with (factor-x,factor-y) (default not set)")
     parser.add_argument('--rotate', default=cfg["rotate_default"], metavar="<default:" +str(cfg["rotate_default"])+ ">",
         type=int, help="number of degrees to rotate")
     parser.add_argument('--splitfile', action='store_true', default=False, help='split gcode output of SVG path and image objects' )
```

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/LICENSE` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/LICENSE`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/__init__.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/__init__.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/compiler/_compiler.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/compiler/_compiler.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/compiler/interfaces/_abstract_interface.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/compiler/interfaces/_abstract_interface.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/compiler/interfaces/_fan_controlled_gcode.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/compiler/interfaces/_fan_controlled_gcode.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/compiler/interfaces/_gcode.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/compiler/interfaces/_gcode.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/css_color.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/css_color.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/formulas.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/formulas.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/__init__.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_abstract_chain.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_abstract_chain.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_abstract_curve.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_abstract_curve.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_circular_arc.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_circular_arc.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_cubic_bazier.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_cubic_bazier.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_elliptical_arc.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_elliptical_arc.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_line.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_line.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_line_segment_chain.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_line_segment_chain.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_matrix.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_matrix.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_quadratic_bazier.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_quadratic_bazier.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_raster_image.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_raster_image.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_smooth_arc_chain.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_smooth_arc_chain.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/geometry/_vector.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_vector.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/svg_parser/__init__.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/svg_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/svg_parser/_parser_methods.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/svg_parser/_parser_methods.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/svg_parser/_path.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/svg_parser/_path.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/svg_parser/_transformation.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/svg_parser/_transformation.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/svg2gcode/svg_to_gcode/svg_parser/debug_methods.py` & `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/svg_parser/debug_methods.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.5/PKG-INFO` & `svg2gcode-3.2.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svg2gcode
-Version: 3.2.5
+Version: 3.2.6
 Summary: svg2gcode: convert an SVG (Scalable Vector Graphic) image to gcode.
 Keywords: scalable vector graphics,svg,image,laser cutter,laser engraving
 Author-email: Johannes Noordanus <mailjohannes.mailnoordanus@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy >= 1.24.3
@@ -123,15 +123,15 @@
                         cutting depth in mm for one pass, only active for passes > 1
   --rapidmove <default:10>
                         generate G0 moves between shapes, for images: G0 moves when skipping more than 10mm (default), 0 is no G0 moves
   --noise <default:0>   reduces image noise by not emitting pixels with power lower or equal than this setting
   --overscan <default:0>
                         overscan image lines to avoid incorrect power levels for pixels at left and right borders, number in pixels, default off
   --showoverscan        show overscan pixels (note that this is visible and part of the gcode emitted!)
-  --constantburn        use constant burn mode M3 (a bit more dangerous!), instead of dynamic burn mode M4
+  --constantburn        set constant burn mode M3 (default set to dynamic burn mode M4); this enhances engraving quality
   --origin delta-x delta-y
                         translate origin by vector (delta-x,delta-y) in mm (default not set, option --selfcenter cannot be used at the same time)
   --scale factor-x factor-y
                         scale svg with (factor-x,factor-y) (default not set)
   --rotate <default:0>  number of degrees to rotate
   --splitfile           split gcode output of SVG path and image objects
   --pathcut             alway cut SVG path objects! (use laser power set with option --cuttingpower)
@@ -286,14 +286,18 @@
     > svg2gcode --splitfile ambachtmanlogo.svg logo.gc
     > ..
     > ls *.gc 
     > logo.gc             # all drawings
     > logo_images.gc      # all images
 ```   
 
+### Burn mode M3/M4:
+
+Default *svg2gcode* uses dynamic burn mode *M4*. This can be changed by setting option *--constantburn* which selects burn mode *M3*. Mode *M4* is not suitable for engravings because it automatically compensates (laser)power for speed. This conflicts with the specific gcode settings given by *image2gcode* (called by *svg2gcode*) for each pixel. In fact some experiments show that *M4* causes loss of quality and image deterioration when speed is increased. On white oak images had too much black and grey which did not go away for substantially higher speed. When switched back to constant burn (*M3*) mode, the same high speed gave excellent images having a sepia (licht yellow brown) color tone.
+
 ### Notes:
  - drawing objects - within the composer - must be converted to a```path```to be translated to a gcode sequence
  - also, image objects should **not** be converted to a ```path```
  - images must be linked or embedded using base64.
  - images can be in several formats (my tests included *.png* and  *.jpg* image files)
  - SVG source documents must be in unit 'mm' (and set to 1 'user unit' is 1 mm) which is the default for Inkscape (check document settings and look at the 'scaling' parameter)
```


# Comparing `tmp/svg2gcode-3.2.6.tar.gz` & `tmp/svg2gcode-3.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svg2gcode-3.2.6.tar", last modified: Mon May 20 20:35:41 2024, max compression
+gzip compressed data, was "svg2gcode-3.2.7.tar", last modified: Mon May 20 21:32:28 2024, max compression
```

## Comparing `svg2gcode-3.2.6.tar` & `svg2gcode-3.2.7.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0    32422 2023-06-11 09:44:38.000000 svg2gcode-3.2.6/LICENSE
--rw-r--r--   0        0        0    14279 2024-05-20 20:33:44.175881 svg2gcode-3.2.6/README.md
--rw-r--r--   0        0        0      692 2024-02-07 15:42:18.000000 svg2gcode-3.2.6/pyproject.toml
--rw-r--r--   0        0        0       98 2024-05-20 20:34:36.035656 svg2gcode-3.2.6/svg2gcode/__init__.py
--rw-r--r--   0        0        0     9346 2024-05-20 20:34:53.971578 svg2gcode-3.2.6/svg2gcode/__main__.py
--rw-r--r--   0        0        0     1068 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/LICENSE
--rw-r--r--   0        0        0     9315 2024-01-08 19:17:21.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/__init__.py
--rw-r--r--   0        0        0      145 2023-12-02 21:51:40.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/compiler/__init__.py
--rw-r--r--   0        0        0    48541 2024-02-07 15:44:36.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/compiler/_compiler.py
--rw-r--r--   0        0        0      249 2023-12-02 21:51:40.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/compiler/interfaces/__init__.py
--rw-r--r--   0        0        0     5895 2023-12-02 21:51:41.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/compiler/interfaces/_abstract_interface.py
--rw-r--r--   0        0        0     1180 2023-12-02 21:51:41.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/compiler/interfaces/_fan_controlled_gcode.py
--rw-r--r--   0        0        0     9499 2023-12-02 21:51:41.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/compiler/interfaces/_gcode.py
--rw-r--r--   0        0        0    15312 2024-01-08 19:18:10.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/css_color.py
--rw-r--r--   0        0        0     5211 2024-01-08 19:18:54.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/formulas.py
--rw-r--r--   0        0        0     1357 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/__init__.py
--rw-r--r--   0        0        0     3439 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_abstract_chain.py
--rw-r--r--   0        0        0     3117 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_abstract_curve.py
--rw-r--r--   0        0        0     3066 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_circular_arc.py
--rw-r--r--   0        0        0     1176 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_cubic_bazier.py
--rw-r--r--   0        0        0     2474 2024-01-08 19:29:33.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_elliptical_arc.py
--rw-r--r--   0        0        0     4115 2024-01-08 19:31:40.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_line.py
--rw-r--r--   0        0        0     5526 2024-01-08 19:32:19.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_line_segment_chain.py
--rw-r--r--   0        0        0     3171 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_matrix.py
--rw-r--r--   0        0        0     1065 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_quadratic_bazier.py
--rw-r--r--   0        0        0     1095 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_raster_image.py
--rw-r--r--   0        0        0     2487 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_smooth_arc_chain.py
--rw-r--r--   0        0        0     1583 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_vector.py
--rw-r--r--   0        0        0      601 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/svg_parser/__init__.py
--rw-r--r--   0        0        0    11956 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/svg_parser/_parser_methods.py
--rw-r--r--   0        0        0    13678 2024-01-08 19:21:51.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/svg_parser/_path.py
--rw-r--r--   0        0        0     5673 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/svg_parser/_transformation.py
--rw-r--r--   0        0        0     2440 2023-12-02 21:51:39.000000 svg2gcode-3.2.6/svg2gcode/svg_to_gcode/svg_parser/debug_methods.py
--rw-r--r--   0        0        0    14836 1970-01-01 00:00:00.000000 svg2gcode-3.2.6/PKG-INFO
+-rw-r--r--   0        0        0    32422 2023-06-11 09:44:38.000000 svg2gcode-3.2.7/LICENSE
+-rw-r--r--   0        0        0    14279 2024-05-20 20:33:44.175881 svg2gcode-3.2.7/README.md
+-rw-r--r--   0        0        0      692 2024-02-07 15:42:18.000000 svg2gcode-3.2.7/pyproject.toml
+-rw-r--r--   0        0        0       98 2024-05-20 21:31:31.597279 svg2gcode-3.2.7/svg2gcode/__init__.py
+-rw-r--r--   0        0        0     9346 2024-05-20 20:34:53.971578 svg2gcode-3.2.7/svg2gcode/__main__.py
+-rw-r--r--   0        0        0     1068 2023-12-02 21:51:39.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/LICENSE
+-rw-r--r--   0        0        0     9315 2024-01-08 19:17:21.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/__init__.py
+-rw-r--r--   0        0        0      145 2023-12-02 21:51:40.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/compiler/__init__.py
+-rw-r--r--   0        0        0    48541 2024-02-07 15:44:36.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/compiler/_compiler.py
+-rw-r--r--   0        0        0    48541 2024-05-20 21:29:32.853780 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/compiler/_compiler_1.py
+-rw-r--r--   0        0        0      249 2023-12-02 21:51:40.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/compiler/interfaces/__init__.py
+-rw-r--r--   0        0        0     5895 2023-12-02 21:51:41.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/compiler/interfaces/_abstract_interface.py
+-rw-r--r--   0        0        0     1180 2023-12-02 21:51:41.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/compiler/interfaces/_fan_controlled_gcode.py
+-rw-r--r--   0        0        0     9499 2023-12-02 21:51:41.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/compiler/interfaces/_gcode.py
+-rw-r--r--   0        0        0    15312 2024-01-08 19:18:10.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/css_color.py
+-rw-r--r--   0        0        0     5211 2024-01-08 19:18:54.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/formulas.py
+-rw-r--r--   0        0        0     1357 2023-12-02 21:51:39.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/__init__.py
+-rw-r--r--   0        0        0     3439 2023-12-02 21:51:39.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_abstract_chain.py
+-rw-r--r--   0        0        0     3117 2023-12-02 21:51:39.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_abstract_curve.py
+-rw-r--r--   0        0        0     3066 2023-12-02 21:51:39.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_circular_arc.py
+-rw-r--r--   0        0        0     1176 2023-12-02 21:51:39.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_cubic_bazier.py
+-rw-r--r--   0        0        0     2474 2024-01-08 19:29:33.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_elliptical_arc.py
+-rw-r--r--   0        0        0     4115 2024-01-08 19:31:40.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_line.py
+-rw-r--r--   0        0        0     5526 2024-01-08 19:32:19.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_line_segment_chain.py
+-rw-r--r--   0        0        0     3171 2023-12-02 21:51:39.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_matrix.py
+-rw-r--r--   0        0        0     1065 2023-12-02 21:51:39.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_quadratic_bazier.py
+-rw-r--r--   0        0        0     1095 2023-12-02 21:51:39.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_raster_image.py
+-rw-r--r--   0        0        0     2487 2023-12-02 21:51:39.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_smooth_arc_chain.py
+-rw-r--r--   0        0        0     1583 2023-12-02 21:51:39.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_vector.py
+-rw-r--r--   0        0        0      601 2023-12-02 21:51:39.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/svg_parser/__init__.py
+-rw-r--r--   0        0        0    11956 2023-12-02 21:51:39.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/svg_parser/_parser_methods.py
+-rw-r--r--   0        0        0    13678 2024-01-08 19:21:51.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/svg_parser/_path.py
+-rw-r--r--   0        0        0     5673 2023-12-02 21:51:39.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/svg_parser/_transformation.py
+-rw-r--r--   0        0        0     2440 2023-12-02 21:51:39.000000 svg2gcode-3.2.7/svg2gcode/svg_to_gcode/svg_parser/debug_methods.py
+-rw-r--r--   0        0        0    14836 1970-01-01 00:00:00.000000 svg2gcode-3.2.7/PKG-INFO
```

### Comparing `svg2gcode-3.2.6/LICENSE` & `svg2gcode-3.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/README.md` & `svg2gcode-3.2.7/README.md`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/pyproject.toml` & `svg2gcode-3.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/__main__.py` & `svg2gcode-3.2.7/svg2gcode/__main__.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/LICENSE` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/LICENSE`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/__init__.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/__init__.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/compiler/_compiler.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/compiler/_compiler.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/compiler/interfaces/_abstract_interface.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/compiler/interfaces/_abstract_interface.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/compiler/interfaces/_fan_controlled_gcode.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/compiler/interfaces/_fan_controlled_gcode.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/compiler/interfaces/_gcode.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/compiler/interfaces/_gcode.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/css_color.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/css_color.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/formulas.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/formulas.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/__init__.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_abstract_chain.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_abstract_chain.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_abstract_curve.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_abstract_curve.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_circular_arc.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_circular_arc.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_cubic_bazier.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_cubic_bazier.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_elliptical_arc.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_elliptical_arc.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_line.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_line.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_line_segment_chain.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_line_segment_chain.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_matrix.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_matrix.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_quadratic_bazier.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_quadratic_bazier.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_raster_image.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_raster_image.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_smooth_arc_chain.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_smooth_arc_chain.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/geometry/_vector.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/geometry/_vector.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/svg_parser/__init__.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/svg_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/svg_parser/_parser_methods.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/svg_parser/_parser_methods.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/svg_parser/_path.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/svg_parser/_path.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/svg_parser/_transformation.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/svg_parser/_transformation.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/svg2gcode/svg_to_gcode/svg_parser/debug_methods.py` & `svg2gcode-3.2.7/svg2gcode/svg_to_gcode/svg_parser/debug_methods.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-3.2.6/PKG-INFO` & `svg2gcode-3.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svg2gcode
-Version: 3.2.6
+Version: 3.2.7
 Summary: svg2gcode: convert an SVG (Scalable Vector Graphic) image to gcode.
 Keywords: scalable vector graphics,svg,image,laser cutter,laser engraving
 Author-email: Johannes Noordanus <mailjohannes.mailnoordanus@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy >= 1.24.3
```


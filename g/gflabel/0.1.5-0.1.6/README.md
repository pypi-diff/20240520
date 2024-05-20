# Comparing `tmp/gflabel-0.1.5.tar.gz` & `tmp/gflabel-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gflabel-0.1.5.tar", max compression
+gzip compressed data, was "gflabel-0.1.6.tar", max compression
```

## Comparing `gflabel-0.1.5.tar` & `gflabel-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,20 @@
--rw-r--r--   0        0        0     1456 2024-05-11 23:25:24.823859 gflabel-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0    18673 2024-05-11 23:25:24.823859 gflabel-0.1.5/README.md
--rw-r--r--   0        0        0      813 2024-05-11 23:25:24.831859 gflabel-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-11 23:25:24.831859 gflabel-0.1.5/src/gflabel/__init__.py
--rw-r--r--   0        0        0      220 2024-05-11 23:25:24.831859 gflabel-0.1.5/src/gflabel/bases/__init__.py
--rw-r--r--   0        0        0     1369 2024-05-11 23:25:24.831859 gflabel-0.1.5/src/gflabel/bases/plain.py
--rw-r--r--   0        0        0     4148 2024-05-11 23:25:24.831859 gflabel-0.1.5/src/gflabel/bases/pred.py
--rw-r--r--   0        0        0     3726 2024-05-11 23:25:24.831859 gflabel-0.1.5/src/gflabel/bases/webb.py
--rw-r--r--   0        0        0   110480 2024-05-11 23:25:24.831859 gflabel-0.1.5/src/gflabel/chris-pikul-symbols.zip
--rwxr-xr-x   0        0        0    13526 2024-05-11 23:25:24.831859 gflabel-0.1.5/src/gflabel/cli.py
--rw-r--r--   0        0        0    40521 2024-05-11 23:25:24.831859 gflabel-0.1.5/src/gflabel/fragments.py
--rw-r--r--   0        0        0    12565 2024-05-11 23:25:24.831859 gflabel-0.1.5/src/gflabel/label.py
--rw-r--r--   0        0        0     2238 2024-05-11 23:25:24.831859 gflabel-0.1.5/src/gflabel/options.py
--rw-r--r--   0        0        0     1739 2024-05-11 23:25:24.831859 gflabel-0.1.5/src/gflabel/util.py
--rw-r--r--   0        0        0    19220 1970-01-01 00:00:00.000000 gflabel-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-05-20 16:30:40.913903 gflabel-0.1.6/LICENSE.txt
+-rw-r--r--   0        0        0    21067 2024-05-20 16:30:40.913903 gflabel-0.1.6/README.md
+-rw-r--r--   0        0        0      813 2024-05-20 16:30:40.921903 gflabel-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/__init__.py
+-rw-r--r--   0        0        0      220 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/bases/__init__.py
+-rw-r--r--   0        0        0     1369 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/bases/plain.py
+-rw-r--r--   0        0        0     4148 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/bases/pred.py
+-rw-r--r--   0        0        0     3726 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/bases/webb.py
+-rwxr-xr-x   0        0        0    13860 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/cli.py
+-rw-r--r--   0        0        0    41424 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/fragments.py
+-rw-r--r--   0        0        0    12565 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/label.py
+-rw-r--r--   0        0        0     3619 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/options.py
+-rw-r--r--   0        0        0     4390 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/resources/LICENSE_OpenSans
+-rw-r--r--   0        0        0     1068 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/resources/LICENSE_symbols
+-rw-r--r--   0        0        0   130860 2024-05-20 16:30:40.925903 gflabel-0.1.6/src/gflabel/resources/OpenSans-Bold.ttf
+-rw-r--r--   0        0        0   136604 2024-05-20 16:30:40.925903 gflabel-0.1.6/src/gflabel/resources/OpenSans-Italic.ttf
+-rw-r--r--   0        0        0   130832 2024-05-20 16:30:40.925903 gflabel-0.1.6/src/gflabel/resources/OpenSans-Regular.ttf
+-rw-r--r--   0        0        0   110480 2024-05-20 16:30:40.925903 gflabel-0.1.6/src/gflabel/resources/chris-pikul-symbols.zip
+-rw-r--r--   0        0        0     1739 2024-05-20 16:30:40.925903 gflabel-0.1.6/src/gflabel/util.py
+-rw-r--r--   0        0        0    21614 1970-01-01 00:00:00.000000 gflabel-0.1.6/PKG-INFO
```

### Comparing `gflabel-0.1.5/LICENSE.txt` & `gflabel-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.5/README.md` & `gflabel-0.1.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # GFLabel
 
-Generates labels for labelled [gridfinity][gridfinity] bins (primarily
+Generates 3d printable labels for labelled [gridfinity][gridfinity] bins (primarily
 [pred][pred] and [Cullen J Webb][webb] labels), and similar
 generate-smallish-printable-label uses. Leverages [build123d][build123d].
 
 [gridfinity]: https://gridfinity.xyz/
 [pred]: https://www.printables.com/model/592545-gridfinity-bin-with-printable-label-by-pred-parame
 [webb]: https://makerworld.com/en/models/446624
 [build123d]: https://github.com/gumyr/build123d
@@ -223,40 +223,59 @@
 
 | Style    | Description | Image      |
 | -------- | ----------- | --------- |
 | Embossed | This is the default. The labels contents are extruded upwards out of the base, as raised features. You can print this multicoloured by changing material at a specific layer height. | ![](images/style_embossed.png)
 | Debossed | Instead of being raised, the label contents are cut into the base. You can also print this multicoloured by changing material at specific layer height.  | ![](images/style_debossed.png)
 | Embedded | The label contents are flush with the surface of the label. This can be printed with a multimaterial system, as it will require material changes within a single layer. You can print this label face-down. To print this, you will need to "Split to Parts" (Bambu/OrcaSlicer) in your slicer and manually change the selected material for the bases.  | ![](images/style_embedded.png)
 
+### Text Style, and Fonts
+
+Text is rendered as text on the label, including variable width whitespaces so e.g. a halfspace
+will render a halfspace width, which is good for minor separation if you don't want a gap of
+specific width.
+
+GFLabel comes with [Open Sans][opensans], and will use this (in regular, bold or italic) if you
+don't otherwise specify any font preference.
+
+Options for controlling font rendering are:
+
+| Setting       | Description |
+| ------------- | ------------|
+| `--font NAME` | Specified font directly, by name. This will have to be a font that is generally installed and available on your system. If you don't specify this (or -path), then a packaged version of Open Sans will be used. |
+| `--font-path /path/to/font` | Specify font by directly specifying the location of the font file on disk. Takes precedence over `--font`, so if you specify both, this will be used.
+| `--font-style STYLE` | Where `STYLE` can be `bolt`, `italic`, or `regular` (the default). If you haven't specified a font file then the underlying font system will make a best-effort attempt to find your selected font in one of these weights.
+| `--font-size NUMBER` | Specifies a fixed height (in mm) for the font on the label. Text will always be rendered at this size, even if it causes the text to not fit. Using this can help text-size consistency over many labels, as otherwise the shorter text labels may end up at a larger scale (because they can fill the vertical without over-running it's available space).
+| `--font-size-maximum NUMBER` | Specifies a _maximum_ font size. Text won't be allowed to go larger than this, but text can be shrunk to fit if it would otherwise overrun it's label area. This can help text-size disparity over many labels in cases where some of them are much longer, and you can tolerate them being shrunken. This is used to generate the electrical symbol examples.
 
 ### Symbols/Fragments
 
 Along with text, you can add symbols and features to a label by specifying
 "fragments". These are directives enclosed in `{`curly braces`}`.
 
 A list of all the fragments currently recognised:
 
 | Names             | Description                                                       |
 |-------------------|-------------------------------------------------------------------|
 | ...               | Blank area that always expands to fill available space.<br><br>If specified multiple times, the areas will be balanced between<br>entries. This can be used to justify/align text. |
+| 1, 4.2, ...       | A gap of specific width, in mm.                                   |
 | &lt;, &gt;        | Only used at the start of a single label or column. Specifies that all lines in the area should be left or right aligned. Invalid when specified elsewhere. |
-| &lt;number&gt;    | A gap of specific width, in mm.                                   |
 | bolt              | Variable length bolt, in the style of Printables pred-box labels.<br><br>If the requested bolt is longer than the available space, then the<br>bolt will be as large as possible with a broken thread. |
 | box               | Arbitrary width, height centered box. If height is not specified, will expand to row height. |
 | head              | Screw head with specifiable head-shape.                           |
 | hexhead           | Hexagonal screw head. Will accept drives, but not compulsory.     |
 | hexnut, nut       | Hexagonal outer profile nut with circular cutout.                 |
 | lockwasher        | Circular washer with a locking cutout.                            |
-| measure           | Fills as much area as possible with a dimension line, and shows the length. Useful for debugging.|
+| magnet            | Horseshoe shaped magnet symbol.                                   |
+| measure           | Fills as much area as possible with a dimension line, and shows the length. Useful for debugging. |
 | sym, symbol       | Render an electronic symbol.                                      |
 | threaded_insert   | Representation of a threaded insert.                              |
 | variable_resistor | Electrical symbol of a variable resistor.                         |
 | washer            | Circular washer with a circular hole.                             |
 | webbolt           | Alternate bolt representation incorporating screw drive, with fixed length. |
-| `\|` (pipe)         | Denotes a column edge, where the label should be split. You can specify relative proportions for the columns, as well as specifying the column alignment. |
+| `\|` (pipe)       | Denotes a column edge, where the label should be split. You can specify relative proportions for the columns, as well as specifying the column alignment. |
 
 A basic set of examples showing the usage of some of these:
 
 ![](images/examples.svg)
 
 ### Bolt/Screw Drives
 
@@ -338,15 +357,15 @@
 ![](images/column_basic_proportion_align.svg)
 
 
 ### Electronic Symbols
 
 Electronic symbols can be generated using the `{symbol(...)}` fragment.
 GFLabel is using the [Chris Pikul Electronic Symbols ][pikul] library kindly
-released under MIT Licence.
+released under MIT License.
 
 [pikul]: https://github.com/chris-pikul/electronic-symbols
 
 There are currently three main approaches to selecting the symbol that you
 want:
 
 - Exact [ID][ID], or exact [Filename][files], as defined the original source.
@@ -385,8 +404,18 @@
 [ID]: https://github.com/chris-pikul/electronic-symbols/blob/main/manifest.json
 [files]: https://github.com/chris-pikul/electronic-symbols/tree/main/SVG
 
 Here is a table of all symbols, rendered by GFLabel, with their name as per the
 source symbol library. Note that for some of the symbols, they are rendered
 incorrectly. This is an unresolved bug in GFLabel.
 
-![](images/symbols.svg)
+![](images/symbols.svg)
+
+# Bundled Dependencies
+
+GFLabel uses (and bundles) a couple of dependencies in subdirectories:
+- The [Chris Pikul Electronic Symbols ][pikul] library, MIT License © 2022 Chris Pikul.
+- The [Open Sans][opensans] font family, OFL-1.1 License © 2020 The Open Sans Project Authors.
+
+
+[opensans]: https://github.com/googlefonts/opensans
+[pikul]: https://github.com/chris-pikul/electronic-symbols
```

### Comparing `gflabel-0.1.5/pyproject.toml` & `gflabel-0.1.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gflabel"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Nicholas Devenish <ndevenish@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -24,15 +24,15 @@
 [tool.ruff.lint.isort]
 required-imports = ["from __future__ import annotations"]
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpversion]
-current_version = "0.1.5"
+current_version = "0.1.6"
 tag = true
 tag_name = "v{new_version}"
 commit = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
```

### Comparing `gflabel-0.1.5/src/gflabel/bases/plain.py` & `gflabel-0.1.6/src/gflabel/bases/plain.py`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.5/src/gflabel/bases/pred.py` & `gflabel-0.1.6/src/gflabel/bases/pred.py`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.5/src/gflabel/bases/webb.py` & `gflabel-0.1.6/src/gflabel/bases/webb.py`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.5/src/gflabel/chris-pikul-symbols.zip` & `gflabel-0.1.6/src/gflabel/resources/chris-pikul-symbols.zip`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.5/src/gflabel/cli.py` & `gflabel-0.1.6/src/gflabel/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/usr/bin/env python3
 # ruff: noqa: F403
 
 from __future__ import annotations
 
 import argparse
 import logging
+import os
 import sys
 from argparse import ArgumentParser
+from pathlib import Path
 from typing import Any, Sequence
 
 import build123d as bd
 import rich
 import rich.table
 
 # from build123d import *
@@ -141,39 +143,44 @@
         help="How many areas to divide a single label into. If more labels that this are requested, multiple labels will be generated. Default: %(default)s.",
         type=int,
         default=1,
     )
 
     parser.add_argument(
         "--font",
-        help="The font to use for rendering. [Default: %(default)s]",
+        help="The name of the system font to use for rendering. If unspecified, a bundled version of Open Sans will be used. Set GFLABEL_FONT in your environment to change the default.",
         type=str,
-        default="Futura",
+        default=os.getenv("GFLABEL_FONT"),
     )
 
     font_size = parser.add_mutually_exclusive_group()
     font_size.add_argument(
         "--font-size-maximum",
         help="Specify a maximum font size (in mm) to use for rendering. The text may end up smaller than this if it needs to fit in the area.",
         type=float,
     )
     font_size.add_argument(
         "--font-size",
         help="The font size (in mm) to use for rendering. If unset, then the font will use as much vertical space as needed (that also fits within the horizontal area).",
         type=float,
     )
-
     parser.add_argument(
         "--font-style",
         help="The font style use for rendering. [Default: %(default)s]",
         choices=[x.name.lower() for x in FontStyle],
         default="regular",
         type=str,
     )
     parser.add_argument(
+        "--font-path",
+        help="Path to font file, if not using a system-level font.",
+        type=Path,
+        # default=None,
+    )
+    parser.add_argument(
         "--margin",
         help="The margin area (in mm) to leave around the label contents. Default is per-base.",
         type=float,
     )
     parser.add_argument(
         "-o",
         "--output",
```

### Comparing `gflabel-0.1.5/src/gflabel/fragments.py` & `gflabel-0.1.6/src/gflabel/fragments.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     Locations,
     Mode,
     Plane,
     PolarLocations,
     Polyline,
     Rectangle,
     RegularPolygon,
+    Rot,
     Sketch,
     SlotCenterToCenter,
     Text,
     Triangle,
     Vector,
     add,
     fillet,
@@ -226,20 +227,17 @@
 
 class TextFragment(Fragment):
     def __init__(self, text: str):
         self.text = text
 
     def render(self, height: float, maxsize: float, options: RenderOptions) -> Sketch:
         with BuildSketch() as sketch:
-            Text(
-                self.text,
-                font_size=options.font.get_allowed_height(height),
-                font=options.font.font,
-                font_style=options.font.font_style,
-            )
+            with options.font.font_options() as f:
+                print(f"Using {f}")
+                Text(self.text, font_size=options.font.get_allowed_height(height), **f)
         return sketch.sketch
 
 
 @functools.lru_cache
 def _whitespace_width(spacechar: str, height: float, options: RenderOptions) -> float:
     """Calculate the width of a space at a specific text height"""
     w2 = (
@@ -892,15 +890,15 @@
                     else None
                 ),
                 examples=getattr(fragment, "examples", None) or [],
             )
         )
     descriptions.append(
         FragmentDescriptionRow(
-            names=["<number>"],
+            names=["1", "4.2", "..."],
             description="A gap of specific width, in mm.",
             examples=["]{12.5}["],
         )
     )
     return sorted(descriptions, key=lambda x: x.names[0])
 
 
@@ -1072,15 +1070,15 @@
 class _electrical_symbol_fragment(Fragment):
     """Render an electronic symbol."""
 
     def __init__(self, *selectors: str):
         self.symbol = _match_electronic_symbol_with_selectors(selectors)
 
         with importlib.resources.files("gflabel").joinpath(
-            "chris-pikul-symbols.zip"
+            "resources/chris-pikul-symbols.zip"
         ).open("rb") as f:
             zip = zipfile.ZipFile(f)
             svg_data = io.StringIO(
                 zip.read("SVG/" + self.symbol["filename"] + ".svg").decode()
             )
             self.shapes = import_svg(svg_data, flip_y=False)
 
@@ -1154,14 +1152,35 @@
 
     def __init__(self, *args):
         raise InvalidFragmentSpecification(
             "Got Alignment fragment ({<} or {>}) not at the start of a label; for selective alignment please pad with {...}, or specify alignment in column division."
         )
 
 
+@fragment("magnet", examples=["{magnet}"])
+def _fragment_magnet(height: float, _maxsize: float) -> Sketch:
+    """Horseshoe shaped magnet symbol."""
+    scale = height * 2 / 3
+    thickness = 0.2
+    arm_len = 1.8
+    with BuildSketch() as sketch:
+        Circle(scale / 2)
+        Circle(scale / 2 * (1 - thickness * 2), mode=Mode.SUBTRACT)
+        Rectangle(
+            scale * arm_len, scale, align=(Align.MIN, Align.CENTER), mode=Mode.SUBTRACT
+        )
+        with Locations(
+            (0, scale / 2 - scale * thickness / 2),
+            (0, -(scale / 2 - scale * thickness / 2)),
+        ):
+            Rectangle(scale / 2, scale * thickness, align=(Align.MIN, Align.CENTER))
+
+    return Rot(0, 0, 45) * sketch.sketch
+
+
 if __name__ == "__main__":
     # Generate a markdown table of fragment definitions
     frags = fragment_description_table()
     maxname = max(len(", ".join(frag.names)) for frag in frags)
 
     # os.geten
     desc_len = 82 - maxname
@@ -1169,12 +1188,19 @@
     print("|" + "-" * (maxname + 2) + "|" + "-" * (desc_len + 2) + "|")
 
     for frag in frags:
 
         def _clean(s):
             if s is None:
                 return ""
-            return s.replace("<", "&lt;").replace(">", "&gt;").replace("\n", "<br>")
+            return (
+                s.replace("<", "&lt;")
+                .replace(">", "&gt;")
+                .replace("\n", "<br>")
+                .replace("|", "\\|")
+            )
 
+        if frag.names == ["|"]:
+            frag = frag._replace(names=["`|` (pipe)"])
         desc = _clean(frag.description)
         names = _clean(", ".join(frag.names))
         print(f"| {names:{maxname}} | {desc:{desc_len}} |")
```

### Comparing `gflabel-0.1.5/src/gflabel/label.py` & `gflabel-0.1.6/src/gflabel/label.py`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.5/src/gflabel/options.py` & `gflabel-0.1.6/src/gflabel/options.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 from __future__ import annotations
 
 import argparse
+import contextlib
+import importlib
+import importlib.resources
+import logging
 from enum import Enum, auto
-from typing import NamedTuple
+from typing import Iterator, NamedTuple
 
-from build123d import FontStyle
+from build123d import FontStyle, Path
+
+logger = logging.getLogger(__name__)
 
 
 class LabelStyle(Enum):
     EMBOSSED = auto()
     DEBOSSED = auto()
     EMBEDDED = auto()
 
@@ -19,16 +25,18 @@
                 return kind
 
     def __str__(self):
         return self.name.lower()
 
 
 class FontOptions(NamedTuple):
-    font: str = "Futura"
-    font_style: FontStyle = FontStyle.BOLD
+    font: str | None = None
+    font_style: FontStyle = FontStyle.REGULAR
+    font_path: Path | None = None
+
     # The font height, in mm. If this is unspecified, then the font will
     # be scaled to maximum area height, and then scaled down accordingly.
     # Setting this can explicitly cause overflow, as the text will be
     # unable to scale down if required.
     font_height_mm: float | None = None
     # Whether this is specifying exact font height
     font_height_exact: bool = True
@@ -36,14 +44,44 @@
     def get_allowed_height(self, requested_height: float) -> float:
         """Calculate the font height, accounting for option specifications"""
         if self.font_height_exact:
             return self.font_height_mm or requested_height
         else:
             return min(self.font_height_mm or requested_height, requested_height)
 
+    @contextlib.contextmanager
+    def font_options(self) -> Iterator:
+        """
+        Handle loading of any font files, generating the kwargs to pass to build123d.Text
+        """
+
+        kwargs = {"font_style": self.font_style}
+        if self.font_path:
+            kwargs["font_path"] = str(self.font_path)
+        # Need to work out if path is enough or if we also need name
+        if self.font:
+            kwargs["font"] = self.font
+
+        with contextlib.ExitStack() as stack:
+            # If we have no font, and no font path, then use the built-in ones
+            if not self.font and not self.font_path:
+                logger.debug("Falling back to internal font OpenSans")
+                # This is a bit noisy but the way you are supposed to do it
+                fontfile = stack.enter_context(
+                    importlib.resources.as_file(
+                        importlib.resources.files("gflabel").joinpath(
+                            f"resources/OpenSans-{self.font_style.name.title()}"
+                        )
+                    )
+                )
+
+                kwargs["font_path"] = str(fontfile)
+
+            yield kwargs
+
 
 class RenderOptions(NamedTuple):
     line_spacing_mm: float = 0.1
     margin_mm: float = 0.4
     font: FontOptions = FontOptions()
     # Overheight fragments cause the entire line to be scaled down in
     # height so that they can fit. Is this allowed, or will they scale
@@ -59,11 +97,12 @@
         return cls(
             margin_mm=args.margin,
             font=FontOptions(
                 font=args.font,
                 font_style=font_style,
                 font_height_mm=args.font_size or args.font_size_maximum,
                 font_height_exact=not args.font_size_maximum,
+                font_path=args.font_path,
             ),
             allow_overheight=not args.no_overheight,
             column_gap=args.column_gap,
         )
```

### Comparing `gflabel-0.1.5/src/gflabel/util.py` & `gflabel-0.1.6/src/gflabel/util.py`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.5/PKG-INFO` & `gflabel-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gflabel
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 License: BSD-3-Clause
 Author: Nicholas Devenish
 Author-email: ndevenish@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: build123d (>=0.5.0,<0.6.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Description-Content-Type: text/markdown
 
 # GFLabel
 
-Generates labels for labelled [gridfinity][gridfinity] bins (primarily
+Generates 3d printable labels for labelled [gridfinity][gridfinity] bins (primarily
 [pred][pred] and [Cullen J Webb][webb] labels), and similar
 generate-smallish-printable-label uses. Leverages [build123d][build123d].
 
 [gridfinity]: https://gridfinity.xyz/
 [pred]: https://www.printables.com/model/592545-gridfinity-bin-with-printable-label-by-pred-parame
 [webb]: https://makerworld.com/en/models/446624
 [build123d]: https://github.com/gumyr/build123d
@@ -240,40 +240,59 @@
 
 | Style    | Description | Image      |
 | -------- | ----------- | --------- |
 | Embossed | This is the default. The labels contents are extruded upwards out of the base, as raised features. You can print this multicoloured by changing material at a specific layer height. | ![](images/style_embossed.png)
 | Debossed | Instead of being raised, the label contents are cut into the base. You can also print this multicoloured by changing material at specific layer height.  | ![](images/style_debossed.png)
 | Embedded | The label contents are flush with the surface of the label. This can be printed with a multimaterial system, as it will require material changes within a single layer. You can print this label face-down. To print this, you will need to "Split to Parts" (Bambu/OrcaSlicer) in your slicer and manually change the selected material for the bases.  | ![](images/style_embedded.png)
 
+### Text Style, and Fonts
+
+Text is rendered as text on the label, including variable width whitespaces so e.g. a halfspace
+will render a halfspace width, which is good for minor separation if you don't want a gap of
+specific width.
+
+GFLabel comes with [Open Sans][opensans], and will use this (in regular, bold or italic) if you
+don't otherwise specify any font preference.
+
+Options for controlling font rendering are:
+
+| Setting       | Description |
+| ------------- | ------------|
+| `--font NAME` | Specified font directly, by name. This will have to be a font that is generally installed and available on your system. If you don't specify this (or -path), then a packaged version of Open Sans will be used. |
+| `--font-path /path/to/font` | Specify font by directly specifying the location of the font file on disk. Takes precedence over `--font`, so if you specify both, this will be used.
+| `--font-style STYLE` | Where `STYLE` can be `bolt`, `italic`, or `regular` (the default). If you haven't specified a font file then the underlying font system will make a best-effort attempt to find your selected font in one of these weights.
+| `--font-size NUMBER` | Specifies a fixed height (in mm) for the font on the label. Text will always be rendered at this size, even if it causes the text to not fit. Using this can help text-size consistency over many labels, as otherwise the shorter text labels may end up at a larger scale (because they can fill the vertical without over-running it's available space).
+| `--font-size-maximum NUMBER` | Specifies a _maximum_ font size. Text won't be allowed to go larger than this, but text can be shrunk to fit if it would otherwise overrun it's label area. This can help text-size disparity over many labels in cases where some of them are much longer, and you can tolerate them being shrunken. This is used to generate the electrical symbol examples.
 
 ### Symbols/Fragments
 
 Along with text, you can add symbols and features to a label by specifying
 "fragments". These are directives enclosed in `{`curly braces`}`.
 
 A list of all the fragments currently recognised:
 
 | Names             | Description                                                       |
 |-------------------|-------------------------------------------------------------------|
 | ...               | Blank area that always expands to fill available space.<br><br>If specified multiple times, the areas will be balanced between<br>entries. This can be used to justify/align text. |
+| 1, 4.2, ...       | A gap of specific width, in mm.                                   |
 | &lt;, &gt;        | Only used at the start of a single label or column. Specifies that all lines in the area should be left or right aligned. Invalid when specified elsewhere. |
-| &lt;number&gt;    | A gap of specific width, in mm.                                   |
 | bolt              | Variable length bolt, in the style of Printables pred-box labels.<br><br>If the requested bolt is longer than the available space, then the<br>bolt will be as large as possible with a broken thread. |
 | box               | Arbitrary width, height centered box. If height is not specified, will expand to row height. |
 | head              | Screw head with specifiable head-shape.                           |
 | hexhead           | Hexagonal screw head. Will accept drives, but not compulsory.     |
 | hexnut, nut       | Hexagonal outer profile nut with circular cutout.                 |
 | lockwasher        | Circular washer with a locking cutout.                            |
-| measure           | Fills as much area as possible with a dimension line, and shows the length. Useful for debugging.|
+| magnet            | Horseshoe shaped magnet symbol.                                   |
+| measure           | Fills as much area as possible with a dimension line, and shows the length. Useful for debugging. |
 | sym, symbol       | Render an electronic symbol.                                      |
 | threaded_insert   | Representation of a threaded insert.                              |
 | variable_resistor | Electrical symbol of a variable resistor.                         |
 | washer            | Circular washer with a circular hole.                             |
 | webbolt           | Alternate bolt representation incorporating screw drive, with fixed length. |
-| `\|` (pipe)         | Denotes a column edge, where the label should be split. You can specify relative proportions for the columns, as well as specifying the column alignment. |
+| `\|` (pipe)       | Denotes a column edge, where the label should be split. You can specify relative proportions for the columns, as well as specifying the column alignment. |
 
 A basic set of examples showing the usage of some of these:
 
 ![](images/examples.svg)
 
 ### Bolt/Screw Drives
 
@@ -355,15 +374,15 @@
 ![](images/column_basic_proportion_align.svg)
 
 
 ### Electronic Symbols
 
 Electronic symbols can be generated using the `{symbol(...)}` fragment.
 GFLabel is using the [Chris Pikul Electronic Symbols ][pikul] library kindly
-released under MIT Licence.
+released under MIT License.
 
 [pikul]: https://github.com/chris-pikul/electronic-symbols
 
 There are currently three main approaches to selecting the symbol that you
 want:
 
 - Exact [ID][ID], or exact [Filename][files], as defined the original source.
@@ -403,7 +422,18 @@
 [files]: https://github.com/chris-pikul/electronic-symbols/tree/main/SVG
 
 Here is a table of all symbols, rendered by GFLabel, with their name as per the
 source symbol library. Note that for some of the symbols, they are rendered
 incorrectly. This is an unresolved bug in GFLabel.
 
 ![](images/symbols.svg)
+
+# Bundled Dependencies
+
+GFLabel uses (and bundles) a couple of dependencies in subdirectories:
+- The [Chris Pikul Electronic Symbols ][pikul] library, MIT License © 2022 Chris Pikul.
+- The [Open Sans][opensans] font family, OFL-1.1 License © 2020 The Open Sans Project Authors.
+
+
+[opensans]: https://github.com/googlefonts/opensans
+[pikul]: https://github.com/chris-pikul/electronic-symbols
+
```


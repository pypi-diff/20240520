# Comparing `tmp/vr180_convert-0.3.0.tar.gz` & `tmp/vr180_convert-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vr180_convert-0.3.0.tar", max compression
+gzip compressed data, was "vr180_convert-0.3.1.tar", max compression
```

## Comparing `vr180_convert-0.3.0.tar` & `vr180_convert-0.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1061 2024-05-19 06:19:09.880628 vr180_convert-0.3.0/LICENSE
--rw-r--r--   0        0        0    10741 2024-05-19 06:19:09.880628 vr180_convert-0.3.0/README.md
--rw-r--r--   0        0        0     3837 2024-05-19 06:19:11.120636 vr180_convert-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      707 2024-05-19 06:19:11.120636 vr180_convert-0.3.0/src/vr180_convert/__init__.py
--rw-r--r--   0        0        0      113 2024-05-19 06:19:09.896628 vr180_convert-0.3.0/src/vr180_convert/__main__.py
--rw-r--r--   0        0        0    12817 2024-05-19 06:19:09.896628 vr180_convert-0.3.0/src/vr180_convert/cli.py
--rw-r--r--   0        0        0        0 2024-05-19 06:19:09.896628 vr180_convert-0.3.0/src/vr180_convert/py.typed
--rw-r--r--   0        0        0    12090 2024-05-19 06:19:09.896628 vr180_convert-0.3.0/src/vr180_convert/remapper.py
--rw-r--r--   0        0        0     1889 2024-05-19 06:19:09.896628 vr180_convert-0.3.0/src/vr180_convert/testing.py
--rw-r--r--   0        0        0    20213 2024-05-19 06:19:09.896628 vr180_convert-0.3.0/src/vr180_convert/transformer.py
--rw-r--r--   0        0        0    12140 1970-01-01 00:00:00.000000 vr180_convert-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-19 06:35:15.636507 vr180_convert-0.3.1/LICENSE
+-rw-r--r--   0        0        0    10741 2024-05-19 06:35:15.636507 vr180_convert-0.3.1/README.md
+-rw-r--r--   0        0        0     3837 2024-05-19 06:35:16.696504 vr180_convert-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      707 2024-05-19 06:35:16.696504 vr180_convert-0.3.1/src/vr180_convert/__init__.py
+-rw-r--r--   0        0        0      113 2024-05-19 06:35:15.652507 vr180_convert-0.3.1/src/vr180_convert/__main__.py
+-rw-r--r--   0        0        0    12204 2024-05-19 06:35:15.652507 vr180_convert-0.3.1/src/vr180_convert/cli.py
+-rw-r--r--   0        0        0        0 2024-05-19 06:35:15.652507 vr180_convert-0.3.1/src/vr180_convert/py.typed
+-rw-r--r--   0        0        0    12090 2024-05-19 06:35:15.652507 vr180_convert-0.3.1/src/vr180_convert/remapper.py
+-rw-r--r--   0        0        0     1889 2024-05-19 06:35:15.652507 vr180_convert-0.3.1/src/vr180_convert/testing.py
+-rw-r--r--   0        0        0    20213 2024-05-19 06:35:15.652507 vr180_convert-0.3.1/src/vr180_convert/transformer.py
+-rw-r--r--   0        0        0    12140 1970-01-01 00:00:00.000000 vr180_convert-0.3.1/PKG-INFO
```

### Comparing `vr180_convert-0.3.0/LICENSE` & `vr180_convert-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.3.0/README.md` & `vr180_convert-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.3.0/pyproject.toml` & `vr180_convert-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vr180-convert"
-version = "0.3.0"
+version = "0.3.1"
 description = "Simple VR180 image converter"
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/vr180-convert"
 documentation = "https://vr180-convert.readthedocs.io"
 classifiers = [
```

### Comparing `vr180_convert-0.3.0/src/vr180_convert/__init__.py` & `vr180_convert-0.3.1/src/vr180_convert/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 from .remapper import apply, apply_lr, get_map
 from .transformer import (
     DenormalizeTransformer,
     EquirectangularEncoder,
     Euclidean3DRotator,
     Euclidean3DTransformer,
     FisheyeDecoder,
```

### Comparing `vr180_convert-0.3.0/src/vr180_convert/cli.py` & `vr180_convert-0.3.1/src/vr180_convert/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,22 +164,14 @@
         left_path_candidates = [
             p
             for p in left_path_candidates
             if (p != right_path) and (p.suffix == right_path.suffix)
         ]
         if len(left_path_candidates) == 0:
             raise ValueError("No time-matched left image found")
-        if (
-            len(left_path_candidates) > 1
-            and left_path_candidates[0].stat().st_mtime
-            == left_path_candidates[1].stat().st_mtime
-        ):
-            raise ValueError(
-                f"Multiple time-matched left images found: {left_path_candidates}"
-            )
         left_path = left_path_candidates[0]
     elif not left_path.is_dir() and right_path.is_dir():
         # find closest time-matched left image
         # sort with time
         left_time = left_path.stat().st_mtime
         right_path_candidates = sorted(
             right_path.rglob("*"),
@@ -191,22 +183,14 @@
         right_path_candidates = [
             p
             for p in right_path_candidates
             if (p != left_path) and (p.suffix == left_path.suffix)
         ]
         if len(right_path_candidates) == 0:
             raise ValueError("No time-matched right image found")
-        if (
-            len(right_path_candidates) > 1
-            and right_path_candidates[0].stat().st_mtime
-            == right_path_candidates[1].stat().st_mtime
-        ):
-            raise ValueError(
-                f"Multiple time-matched right images found: {right_path_candidates}"
-            )
         right_path = right_path_candidates[0]
     elif left_path.is_dir() and right_path.is_dir():
         raise ValueError("Both left and right paths must not be directories")
 
     LOG.info(
         f"L: {left_path}"
         f"@{datetime.fromtimestamp(left_path.stat().st_mtime, timezone.utc)}, "
```

### Comparing `vr180_convert-0.3.0/src/vr180_convert/remapper.py` & `vr180_convert-0.3.1/src/vr180_convert/remapper.py`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.3.0/src/vr180_convert/testing.py` & `vr180_convert-0.3.1/src/vr180_convert/testing.py`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.3.0/src/vr180_convert/transformer.py` & `vr180_convert-0.3.1/src/vr180_convert/transformer.py`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.3.0/PKG-INFO` & `vr180_convert-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vr180-convert
-Version: 0.3.0
+Version: 0.3.1
 Summary: Simple VR180 image converter
 Home-page: https://github.com/34j/vr180-convert
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vr180-convert Version: 0.3.0 Summary: Simple VR180
+Metadata-Version: 2.1 Name: vr180-convert Version: 0.3.1 Summary: Simple VR180
 image converter Home-page: https://github.com/34j/vr180-convert License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```


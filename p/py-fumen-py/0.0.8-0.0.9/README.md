# Comparing `tmp/py_fumen_py-0.0.8.tar.gz` & `tmp/py_fumen_py-0.0.9.tar.gz`

## Comparing `py_fumen_py-0.0.8.tar` & `py_fumen_py-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 py_fumen_py-0.0.8/src/py_fumen_py/__init__.py
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 py_fumen_py-0.0.8/src/py_fumen_py/action.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 py_fumen_py-0.0.8/src/py_fumen_py/comment.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 py_fumen_py-0.0.8/src/py_fumen_py/constant.py
--rw-r--r--   0        0        0    11124 2020-02-02 00:00:00.000000 py_fumen_py-0.0.8/src/py_fumen_py/field.py
--rw-r--r--   0        0        0     8437 2020-02-02 00:00:00.000000 py_fumen_py-0.0.8/src/py_fumen_py/fumen_buffer.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 py_fumen_py-0.0.8/src/py_fumen_py/fumen_codec.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 py_fumen_py-0.0.8/src/py_fumen_py/js_escape.py
--rw-r--r--   0        0        0     6718 2020-02-02 00:00:00.000000 py_fumen_py-0.0.8/src/py_fumen_py/operation.py
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 py_fumen_py-0.0.8/src/py_fumen_py/page.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 py_fumen_py-0.0.8/src/py_fumen_py/quiz.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 py_fumen_py-0.0.8/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 py_fumen_py-0.0.8/LICENSE
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 py_fumen_py-0.0.8/README.md
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 py_fumen_py-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 py_fumen_py-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 py_fumen_py-0.0.9/src/py_fumen_py/__init__.py
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 py_fumen_py-0.0.9/src/py_fumen_py/action.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 py_fumen_py-0.0.9/src/py_fumen_py/comment.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 py_fumen_py-0.0.9/src/py_fumen_py/constant.py
+-rw-r--r--   0        0        0    11124 2020-02-02 00:00:00.000000 py_fumen_py-0.0.9/src/py_fumen_py/field.py
+-rw-r--r--   0        0        0     8437 2020-02-02 00:00:00.000000 py_fumen_py-0.0.9/src/py_fumen_py/fumen_buffer.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 py_fumen_py-0.0.9/src/py_fumen_py/fumen_codec.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 py_fumen_py-0.0.9/src/py_fumen_py/js_escape.py
+-rw-r--r--   0        0        0     6718 2020-02-02 00:00:00.000000 py_fumen_py-0.0.9/src/py_fumen_py/operation.py
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 py_fumen_py-0.0.9/src/py_fumen_py/page.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 py_fumen_py-0.0.9/src/py_fumen_py/quiz.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 py_fumen_py-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 py_fumen_py-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 py_fumen_py-0.0.9/README.md
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 py_fumen_py-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 py_fumen_py-0.0.9/PKG-INFO
```

### Comparing `py_fumen_py-0.0.8/src/py_fumen_py/action.py` & `py_fumen_py-0.0.9/src/py_fumen_py/action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 from dataclasses import dataclass
 
-from .constant import FieldConstants
+from .constant import FieldConstants as Consts
 from .operation import Mino, Rotation, Operation
 
 @dataclass
 class Action():
     """A dataclass for storing encoded Fumen page flags and field changes.
     Keyword arguments:
     operation: the operation applied to the field.
```

### Comparing `py_fumen_py-0.0.8/src/py_fumen_py/comment.py` & `py_fumen_py-0.0.9/src/py_fumen_py/comment.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.8/src/py_fumen_py/constant.py` & `py_fumen_py-0.0.9/src/py_fumen_py/constant.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.8/src/py_fumen_py/field.py` & `py_fumen_py-0.0.9/src/py_fumen_py/field.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.8/src/py_fumen_py/fumen_buffer.py` & `py_fumen_py-0.0.9/src/py_fumen_py/fumen_buffer.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.8/src/py_fumen_py/fumen_codec.py` & `py_fumen_py-0.0.9/src/py_fumen_py/fumen_codec.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     prev_comment = ''
     prev_lock = False
     prev_mino = Mino._
 
     for page in pages:
         page.flags = Flags() if page.flags is None else page.flags
         page.operation = (
-            Operation(Mino._, Rotation.REVERSE, 0, Consts.HEIGHT-1)
+            Operation(Mino._, Rotation.REVERSE, 0, FieldConstants.HEIGHT-1)
             if page.operation is None else page.operation
         )
         quiz = Quiz(prev_comment)
         if prev_lock:
             quiz.step(prev_mino)
         prev_comment = str(quiz)
```

### Comparing `py_fumen_py-0.0.8/src/py_fumen_py/js_escape.py` & `py_fumen_py-0.0.9/src/py_fumen_py/js_escape.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.8/src/py_fumen_py/operation.py` & `py_fumen_py-0.0.9/src/py_fumen_py/operation.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.8/src/py_fumen_py/page.py` & `py_fumen_py-0.0.9/src/py_fumen_py/page.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.8/src/py_fumen_py/quiz.py` & `py_fumen_py-0.0.9/src/py_fumen_py/quiz.py`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.8/.gitignore` & `py_fumen_py-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.8/LICENSE` & `py_fumen_py-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.8/README.md` & `py_fumen_py-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `py_fumen_py-0.0.8/pyproject.toml` & `py_fumen_py-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "py_fumen_py"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
 	{ name="Octupus Tea" },
 ]
 description = "Python implementation of the JavaScript package 'tetris-fumen'"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `py_fumen_py-0.0.8/PKG-INFO` & `py_fumen_py-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_fumen_py
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python implementation of the JavaScript package 'tetris-fumen'
 Project-URL: Source, https://github.com/OctupusTea/py-fumen-py
 Author: Octupus Tea
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/profiles_pycorelib-0.12.0-py3-none-any.whl.zip` & `tmp/profiles_pycorelib-0.13.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,12 @@
-Zip file size: 9410 bytes, number of entries: 8
--rw-r--r--  2.0 unx      306 b- defN 24-Apr-17 11:22 profiles-pycorelib/__init__.py
--rw-r--r--  2.0 unx    16817 b- defN 24-Apr-22 06:37 profiles-pycorelib/attribution_model.py
--rw-r--r--  2.0 unx     5532 b- defN 24-Apr-22 12:10 profiles-pycorelib/common_col_union.py
--rw-r--r--  2.0 unx     6336 b- defN 24-Apr-17 11:22 profiles-pycorelib/sample_model.py
--rw-r--r--  2.0 unx      378 b- defN 24-Apr-25 11:19 profiles_pycorelib-0.12.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 11:19 profiles_pycorelib-0.12.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-Apr-25 11:19 profiles_pycorelib-0.12.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      714 b- defN 24-Apr-25 11:19 profiles_pycorelib-0.12.0.dist-info/RECORD
-8 files, 30194 bytes uncompressed, 8146 bytes compressed:  73.0%
+Zip file size: 11628 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      383 b- defN 24-May-15 11:24 profiles-pycorelib/__init__.py
+-rw-r--r--  2.0 unx    16817 b- defN 24-May-15 11:24 profiles-pycorelib/attribution_model.py
+-rw-r--r--  2.0 unx     5532 b- defN 24-May-15 11:24 profiles-pycorelib/common_col_union.py
+-rw-r--r--  2.0 unx      370 b- defN 24-May-15 11:24 profiles-pycorelib/errors.py
+-rw-r--r--  2.0 unx     6359 b- defN 24-May-15 11:24 profiles-pycorelib/pyplot.py
+-rw-r--r--  2.0 unx     6336 b- defN 24-May-15 11:24 profiles-pycorelib/sample_model.py
+-rw-r--r--  2.0 unx      472 b- defN 24-May-15 11:24 profiles_pycorelib-0.13.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-15 11:24 profiles_pycorelib-0.13.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-May-15 11:24 profiles_pycorelib-0.13.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      883 b- defN 24-May-15 11:24 profiles_pycorelib-0.13.0.dist-info/RECORD
+10 files, 37263 bytes uncompressed, 10100 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -3,23 +3,29 @@
 
 Filename: profiles-pycorelib/attribution_model.py
 Comment: 
 
 Filename: profiles-pycorelib/common_col_union.py
 Comment: 
 
+Filename: profiles-pycorelib/errors.py
+Comment: 
+
+Filename: profiles-pycorelib/pyplot.py
+Comment: 
+
 Filename: profiles-pycorelib/sample_model.py
 Comment: 
 
-Filename: profiles_pycorelib-0.12.0.dist-info/METADATA
+Filename: profiles_pycorelib-0.13.0.dist-info/METADATA
 Comment: 
 
-Filename: profiles_pycorelib-0.12.0.dist-info/WHEEL
+Filename: profiles_pycorelib-0.13.0.dist-info/WHEEL
 Comment: 
 
-Filename: profiles_pycorelib-0.12.0.dist-info/top_level.txt
+Filename: profiles_pycorelib-0.13.0.dist-info/top_level.txt
 Comment: 
 
-Filename: profiles_pycorelib-0.12.0.dist-info/RECORD
+Filename: profiles_pycorelib-0.13.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## profiles-pycorelib/__init__.py

```diff
@@ -1,7 +1,9 @@
 from profiles_rudderstack.project import WhtProject
 from .common_col_union import CommonColumnUnionModel
+from .pyplot import PyPlotModel
 from .attribution_model import AttributionModel
 
 def register_extensions(project: WhtProject):
     project.register_model_type(CommonColumnUnionModel)
     project.register_model_type(AttributionModel)
+    project.register_model_type(PyPlotModel)
```

## Comparing `profiles_pycorelib-0.12.0.dist-info/RECORD` & `profiles_pycorelib-0.13.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-profiles-pycorelib/__init__.py,sha256=1HZi4n3xY_p_rPrV7NiUZNuxex0X3eUELf18HEmiubQ,306
+profiles-pycorelib/__init__.py,sha256=jARYnJSKI6YVyySS5zo8jneh0bxvurK95uQEFtREQCQ,383
 profiles-pycorelib/attribution_model.py,sha256=6ZieetgZNLOEwxb5K94NgugtdSoZZBPrSxYX1mxw6RE,16817
 profiles-pycorelib/common_col_union.py,sha256=GgnMhpQlxSrmm2QZ0NDkmgNbf1untBHZ1lRxLW584lo,5532
+profiles-pycorelib/errors.py,sha256=djEVK7Ta0zDD_Q2Bn2lJ-Xc2PZ9kDRH3ud0V94FRIYo,370
+profiles-pycorelib/pyplot.py,sha256=a6-SFrsJOY-xSxRqc0XSvhyWgWieL1QlI4X26z8vyn4,6359
 profiles-pycorelib/sample_model.py,sha256=eGt2I0BUq5S7pumvHqmlKLxOPXSYONI6P6jcDq2fOQE,6336
-profiles_pycorelib-0.12.0.dist-info/METADATA,sha256=PoClB_wsdgUo4yhzz7O-7hTw1RxPGhK4rfkiAHMfQJE,378
-profiles_pycorelib-0.12.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-profiles_pycorelib-0.12.0.dist-info/top_level.txt,sha256=InRwLnEjGzuE_N_OQAswVHHRbc8_WHJz9OOaJiaZMl0,19
-profiles_pycorelib-0.12.0.dist-info/RECORD,,
+profiles_pycorelib-0.13.0.dist-info/METADATA,sha256=jZ7LKtCX32mYgjS-9GKzAg5UO4mZqIIxs3ePCrBXA5w,472
+profiles_pycorelib-0.13.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+profiles_pycorelib-0.13.0.dist-info/top_level.txt,sha256=InRwLnEjGzuE_N_OQAswVHHRbc8_WHJz9OOaJiaZMl0,19
+profiles_pycorelib-0.13.0.dist-info/RECORD,,
```


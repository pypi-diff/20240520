# Comparing `tmp/property_utils-0.2.3.tar.gz` & `tmp/property_utils-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "property_utils-0.2.3.tar", last modified: Tue Apr 23 06:52:42 2024, max compression
+gzip compressed data, was "property_utils-0.2.4.tar", last modified: Mon May 20 14:40:24 2024, max compression
```

## Comparing `property_utils-0.2.3.tar` & `property_utils-0.2.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-23 06:52:42.799153 property_utils-0.2.3/
--rw-r--r--   0 max       (1000) max       (1000)     1076 2024-03-28 17:51:01.000000 property_utils-0.2.3/LICENSE
--rw-r--r--   0 max       (1000) max       (1000)     4249 2024-04-23 06:52:42.799153 property_utils-0.2.3/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     2907 2024-04-09 14:48:45.000000 property_utils-0.2.3/README.md
--rw-r--r--   0 max       (1000) max       (1000)     1594 2024-04-23 06:52:17.000000 property_utils-0.2.3/pyproject.toml
--rw-r--r--   0 max       (1000) max       (1000)       38 2024-04-23 06:52:42.799153 property_utils-0.2.3/setup.cfg
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-23 06:52:42.789153 property_utils-0.2.3/src/
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-23 06:52:42.792486 property_utils-0.2.3/src/property_utils/
--rw-r--r--   0 max       (1000) max       (1000)        0 2024-03-28 17:51:01.000000 property_utils-0.2.3/src/property_utils/__init__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-23 06:52:42.792486 property_utils-0.2.3/src/property_utils/constants/
--rw-r--r--   0 max       (1000) max       (1000)       49 2024-04-08 13:07:09.000000 property_utils-0.2.3/src/property_utils/constants/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      898 2024-04-08 13:07:09.000000 property_utils-0.2.3/src/property_utils/constants/constants.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-23 06:52:42.795819 property_utils-0.2.3/src/property_utils/exceptions/
--rw-r--r--   0 max       (1000) max       (1000)      142 2024-04-08 13:07:09.000000 property_utils-0.2.3/src/property_utils/exceptions/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      524 2024-03-28 17:51:01.000000 property_utils-0.2.3/src/property_utils/exceptions/base.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-23 06:52:42.795819 property_utils-0.2.3/src/property_utils/exceptions/properties/
--rw-r--r--   0 max       (1000) max       (1000)      185 2024-04-08 13:07:09.000000 property_utils-0.2.3/src/property_utils/exceptions/properties/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      641 2024-03-28 17:51:01.000000 property_utils-0.2.3/src/property_utils/exceptions/properties/property.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-23 06:52:42.795819 property_utils-0.2.3/src/property_utils/exceptions/units/
--rw-r--r--   0 max       (1000) max       (1000)      364 2024-04-08 13:07:09.000000 property_utils-0.2.3/src/property_utils/exceptions/units/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      866 2024-04-06 06:13:47.000000 property_utils-0.2.3/src/property_utils/exceptions/units/converter_types.py
--rw-r--r--   0 max       (1000) max       (1000)      479 2024-03-28 17:51:01.000000 property_utils-0.2.3/src/property_utils/exceptions/units/descriptors.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-23 06:52:42.795819 property_utils-0.2.3/src/property_utils/properties/
--rw-r--r--   0 max       (1000) max       (1000)      134 2024-04-08 13:07:09.000000 property_utils-0.2.3/src/property_utils/properties/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)    28066 2024-04-09 14:48:45.000000 property_utils-0.2.3/src/property_utils/properties/property.py
--rw-r--r--   0 max       (1000) max       (1000)     2683 2024-04-23 06:52:05.000000 property_utils-0.2.3/src/property_utils/properties/validated_property.py
--rw-r--r--   0 max       (1000) max       (1000)        0 2024-04-22 06:47:39.000000 property_utils-0.2.3/src/property_utils/py.typed
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-23 06:52:42.799153 property_utils-0.2.3/src/property_utils/units/
--rw-r--r--   0 max       (1000) max       (1000)       43 2024-04-08 13:07:09.000000 property_utils-0.2.3/src/property_utils/units/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     2939 2024-04-08 15:23:31.000000 property_utils-0.2.3/src/property_utils/units/aliases.py
--rw-r--r--   0 max       (1000) max       (1000)    33193 2024-04-08 14:48:05.000000 property_utils-0.2.3/src/property_utils/units/converter_types.py
--rw-r--r--   0 max       (1000) max       (1000)    12051 2024-04-08 14:48:05.000000 property_utils-0.2.3/src/property_utils/units/converters.py
--rw-r--r--   0 max       (1000) max       (1000)    67715 2024-04-08 14:48:05.000000 property_utils-0.2.3/src/property_utils/units/descriptors.py
--rw-r--r--   0 max       (1000) max       (1000)     4383 2024-04-08 15:28:32.000000 property_utils-0.2.3/src/property_utils/units/units.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-04-23 06:52:42.799153 property_utils-0.2.3/src/property_utils.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)     4249 2024-04-23 06:52:42.000000 property_utils-0.2.3/src/property_utils.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     1089 2024-04-23 06:52:42.000000 property_utils-0.2.3/src/property_utils.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2024-04-23 06:52:42.000000 property_utils-0.2.3/src/property_utils.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)       51 2024-04-23 06:52:42.000000 property_utils-0.2.3/src/property_utils.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)       15 2024-04-23 06:52:42.000000 property_utils-0.2.3/src/property_utils.egg-info/top_level.txt
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-20 14:40:24.514639 property_utils-0.2.4/
+-rw-r--r--   0 max       (1000) max       (1000)     1076 2024-03-28 17:51:01.000000 property_utils-0.2.4/LICENSE
+-rw-r--r--   0 max       (1000) max       (1000)     4249 2024-05-20 14:40:24.514639 property_utils-0.2.4/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     2907 2024-04-09 14:48:45.000000 property_utils-0.2.4/README.md
+-rw-r--r--   0 max       (1000) max       (1000)     1594 2024-05-20 14:38:56.000000 property_utils-0.2.4/pyproject.toml
+-rw-r--r--   0 max       (1000) max       (1000)       38 2024-05-20 14:40:24.514639 property_utils-0.2.4/setup.cfg
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-20 14:40:24.507972 property_utils-0.2.4/src/
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-20 14:40:24.507972 property_utils-0.2.4/src/property_utils/
+-rw-r--r--   0 max       (1000) max       (1000)        0 2024-03-28 17:51:01.000000 property_utils-0.2.4/src/property_utils/__init__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-20 14:40:24.511305 property_utils-0.2.4/src/property_utils/constants/
+-rw-r--r--   0 max       (1000) max       (1000)       49 2024-04-08 13:07:09.000000 property_utils-0.2.4/src/property_utils/constants/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      898 2024-04-08 13:07:09.000000 property_utils-0.2.4/src/property_utils/constants/constants.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-20 14:40:24.511305 property_utils-0.2.4/src/property_utils/exceptions/
+-rw-r--r--   0 max       (1000) max       (1000)      142 2024-04-08 13:07:09.000000 property_utils-0.2.4/src/property_utils/exceptions/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      524 2024-03-28 17:51:01.000000 property_utils-0.2.4/src/property_utils/exceptions/base.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-20 14:40:24.511305 property_utils-0.2.4/src/property_utils/exceptions/properties/
+-rw-r--r--   0 max       (1000) max       (1000)      185 2024-04-08 13:07:09.000000 property_utils-0.2.4/src/property_utils/exceptions/properties/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      641 2024-03-28 17:51:01.000000 property_utils-0.2.4/src/property_utils/exceptions/properties/property.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-20 14:40:24.511305 property_utils-0.2.4/src/property_utils/exceptions/units/
+-rw-r--r--   0 max       (1000) max       (1000)      364 2024-04-08 13:07:09.000000 property_utils-0.2.4/src/property_utils/exceptions/units/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      866 2024-04-06 06:13:47.000000 property_utils-0.2.4/src/property_utils/exceptions/units/converter_types.py
+-rw-r--r--   0 max       (1000) max       (1000)      479 2024-03-28 17:51:01.000000 property_utils-0.2.4/src/property_utils/exceptions/units/descriptors.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-20 14:40:24.511305 property_utils-0.2.4/src/property_utils/properties/
+-rw-r--r--   0 max       (1000) max       (1000)      134 2024-04-08 13:07:09.000000 property_utils-0.2.4/src/property_utils/properties/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)    28203 2024-05-20 12:17:00.000000 property_utils-0.2.4/src/property_utils/properties/property.py
+-rw-r--r--   0 max       (1000) max       (1000)     2683 2024-04-23 06:52:05.000000 property_utils-0.2.4/src/property_utils/properties/validated_property.py
+-rw-r--r--   0 max       (1000) max       (1000)        0 2024-04-22 06:47:39.000000 property_utils-0.2.4/src/property_utils/py.typed
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-20 14:40:24.514639 property_utils-0.2.4/src/property_utils/units/
+-rw-r--r--   0 max       (1000) max       (1000)       43 2024-04-08 13:07:09.000000 property_utils-0.2.4/src/property_utils/units/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     2939 2024-04-08 15:23:31.000000 property_utils-0.2.4/src/property_utils/units/aliases.py
+-rw-r--r--   0 max       (1000) max       (1000)    33193 2024-04-08 14:48:05.000000 property_utils-0.2.4/src/property_utils/units/converter_types.py
+-rw-r--r--   0 max       (1000) max       (1000)    12051 2024-04-08 14:48:05.000000 property_utils-0.2.4/src/property_utils/units/converters.py
+-rw-r--r--   0 max       (1000) max       (1000)    67715 2024-04-08 14:48:05.000000 property_utils-0.2.4/src/property_utils/units/descriptors.py
+-rw-r--r--   0 max       (1000) max       (1000)     4383 2024-04-08 15:28:32.000000 property_utils-0.2.4/src/property_utils/units/units.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-20 14:40:24.514639 property_utils-0.2.4/src/property_utils.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)     4249 2024-05-20 14:40:24.000000 property_utils-0.2.4/src/property_utils.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     1089 2024-05-20 14:40:24.000000 property_utils-0.2.4/src/property_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2024-05-20 14:40:24.000000 property_utils-0.2.4/src/property_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)       51 2024-05-20 14:40:24.000000 property_utils-0.2.4/src/property_utils.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)       15 2024-05-20 14:40:24.000000 property_utils-0.2.4/src/property_utils.egg-info/top_level.txt
```

### Comparing `property_utils-0.2.3/LICENSE` & `property_utils-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.3/PKG-INFO` & `property_utils-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: property-utils
-Version: 0.2.3
+Version: 0.2.4
 Summary: Utilities for programming that involves physical properties
 Author-email: Maximos Nikiforakis <nikiforos@live.co.uk>
 License: MIT
 Project-URL: Homepage, https://github.com/Maxcode123/property-utils
 Project-URL: Issues, https://github.com/Maxcode123/property-utils/issues
 Keywords: physical properties,properties
 Classifier: Programming Language :: Python
```

### Comparing `property_utils-0.2.3/README.md` & `property_utils-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.3/pyproject.toml` & `property_utils-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "property-utils"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
     { name="Maximos Nikiforakis", email="nikiforos@live.co.uk" },
 ]
 description = "Utilities for programming that involves physical properties"
 keywords = ["physical properties", "properties"]
 readme = "README.md"
 license = {text = "MIT"}
```

### Comparing `property_utils-0.2.3/src/property_utils/constants/constants.py` & `property_utils-0.2.4/src/property_utils/constants/constants.py`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.3/src/property_utils/exceptions/base.py` & `property_utils-0.2.4/src/property_utils/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.3/src/property_utils/exceptions/properties/property.py` & `property_utils-0.2.4/src/property_utils/exceptions/properties/property.py`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.3/src/property_utils/exceptions/units/converter_types.py` & `property_utils-0.2.4/src/property_utils/exceptions/units/converter_types.py`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.3/src/property_utils/properties/property.py` & `property_utils-0.2.4/src/property_utils/properties/property.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 This module defines the Property class and property arithmetics.
 """
 
 from dataclasses import dataclass, replace
-from typing import Type, Optional
+from typing import Type, Optional, ClassVar
 from math import isclose
 
 try:
     from typing import Self  # Python > 3.10 pylint: disable=ungrouped-imports
 except ImportError:
     from typing_extensions import Self  # Python <= 3.10
 
@@ -59,25 +59,31 @@
     A Property can have any 'value' or 'unit'; validations are not applied to it.
     For example, a Property with length units and negative value is valid.
     """
 
     value: float
     unit: UnitDescriptor
     unit_converter: Optional[Type[UnitConverter]] = None
+    default_units: ClassVar[Optional[UnitDescriptor]] = None
 
-    def __init__(self, value: float, unit: UnitDescriptor) -> None:
+    def __init__(self, value: float, unit: Optional[UnitDescriptor] = None) -> None:
         if not isinstance(value, (float, int)):
             raise PropertyValidationError(
                 f"cannot create Property; invalid 'value': {value}; expected numeric. "
             )
+
+        if unit is None and self.default_units is not None:
+            unit = self.default_units
+
         if not isinstance(unit, (MeasurementUnit, Dimension, CompositeDimension)):
             raise PropertyValidationError(
                 f"cannot create Property; invalid 'unit': {unit}. Expected an instance"
                 " of one of: MeasurementUnit, Dimension, CompositeDimension. "
             )
+
         self.value = value
         self.unit = unit
 
     def eq(self, other: "Property", *, rel_tol=1e-9, abs_tol=0) -> bool:
         """
         Perform equality comparison between this and some other Property. This method
         of testing equality is preferable to the equality operator '==' because float
@@ -203,15 +209,15 @@
             >>> 2*T
             <Property: 600 K>
             >>> A = Property(10, LengthUnit.METER**2)
             >>> T * A
             <Property: 3000 (m^2) * K>
         """
         if isinstance(other, (float, int)):
-            return Property(self.value * other, self.unit)
+            return self.__class__(self.value * other, self.unit)
         if isinstance(other, Property):
             _other = self._unit_preconversion(other)
             return Property(
                 self.value * _other.value, (self.unit * _other.unit).simplified()
             )
         raise PropertyBinaryOperationError(
             f"cannot multiply {self} with {other}; "
@@ -306,18 +312,18 @@
         Examples:
             >>> from property_utils.units.units import LengthUnit
             >>> x1 = Property(15, LengthUnit.METER)
             >>> x2 = Property(5, LengthUnit.METER)
             >>> x1 + x2
             <Property: 20 m>
         """
-        if not isinstance(other, self.__class__):
+        if not isinstance(other, Property):
             raise PropertyBinaryOperationError(
-                f"cannot add {other} to ({self}); {other} is not a {self.__class__}; "
-                "only same properties can be added to each other. "
+                f"cannot add {other} to ({self}); {other} is not a Property; "
+                "only properties can be added to properties. "
             )
         if not self.unit.isinstance_equivalent(other.unit.to_generic()):
             raise PropertyBinaryOperationError(
                 f"cannot add ({other}) to ({self}); "
                 f"({other}) must have ({self.unit.to_generic()}) units. "
             )
         try:
@@ -354,19 +360,18 @@
         Examples:
             >>> from property_utils.units.units import TimeUnit
             >>> t1 = Property(2, TimeUnit.MINUTE)
             >>> t2 = Property(60, TimeUnit.SECOND)
             >>> t1 - t2
             <Property: 1.0 min>
         """
-        if not isinstance(other, self.__class__):
+        if not isinstance(other, Property):
             raise PropertyBinaryOperationError(
                 f"cannot subtract {other} from ({self}); {other} is not a "
-                f"{self.__class__}; only same properties can be subtracted from each "
-                "other. "
+                "Property; only properties can be subtracted from properties. "
             )
         if not self.unit.isinstance_equivalent(other.unit.to_generic()):
             raise PropertyBinaryOperationError(
                 f"cannot subtract ({other}) from ({self}); "
                 f"({other}) must have ({self.unit.to_generic()}) units. "
             )
         try:
@@ -379,26 +384,26 @@
             ) from None
         except UnitConversionError as exc:
             raise PropertyBinaryOperationError(
                 f"cannot subtract ({other}) from ({self});", exc
             ) from None
         return self.__class__(self.value - prop.value, self.unit)
 
-    def __rsub__(self, other) -> Self:
+    def __rsub__(self, other) -> "Property":
         """
         Defines right subtraction between properties.
 
         Examples:
             >>> from property_utils.units.units import TimeUnit
             >>> t1 = Property(2, TimeUnit.MINUTE)
             >>> t2 = Property(60, TimeUnit.SECOND)
             >>> t1 - t2
             <Property: 1.0 min>
         """
-        if not isinstance(other, self.__class__):
+        if not isinstance(other, Property):
             raise PropertyBinaryOperationError(
                 f"cannot subtract {self} from ({other}); {other} is not a "
                 f"{self.__class__}; only same properties can be subtracted from each "
                 "other. "
             )
         if not self.unit.isinstance_equivalent(other.unit.to_generic()):
             raise PropertyBinaryOperationError(
```

### Comparing `property_utils-0.2.3/src/property_utils/properties/validated_property.py` & `property_utils-0.2.4/src/property_utils/properties/validated_property.py`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.3/src/property_utils/units/aliases.py` & `property_utils-0.2.4/src/property_utils/units/aliases.py`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.3/src/property_utils/units/converter_types.py` & `property_utils-0.2.4/src/property_utils/units/converter_types.py`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.3/src/property_utils/units/converters.py` & `property_utils-0.2.4/src/property_utils/units/converters.py`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.3/src/property_utils/units/descriptors.py` & `property_utils-0.2.4/src/property_utils/units/descriptors.py`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.3/src/property_utils/units/units.py` & `property_utils-0.2.4/src/property_utils/units/units.py`

 * *Files identical despite different names*

### Comparing `property_utils-0.2.3/src/property_utils.egg-info/PKG-INFO` & `property_utils-0.2.4/src/property_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: property-utils
-Version: 0.2.3
+Version: 0.2.4
 Summary: Utilities for programming that involves physical properties
 Author-email: Maximos Nikiforakis <nikiforos@live.co.uk>
 License: MIT
 Project-URL: Homepage, https://github.com/Maxcode123/property-utils
 Project-URL: Issues, https://github.com/Maxcode123/property-utils/issues
 Keywords: physical properties,properties
 Classifier: Programming Language :: Python
```

### Comparing `property_utils-0.2.3/src/property_utils.egg-info/SOURCES.txt` & `property_utils-0.2.4/src/property_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*


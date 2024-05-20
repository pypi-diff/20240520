# Comparing `tmp/lucupy-0.1.9.tar.gz` & `tmp/lucupy-0.1.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lucupy-0.1.9.tar", max compression
+gzip compressed data, was "lucupy-0.1.90.tar", max compression
```

## Comparing `lucupy-0.1.9.tar` & `lucupy-0.1.90.tar`

### file list

```diff
@@ -1,39 +1,46 @@
--rw-r--r--   0        0        0     1528 2022-10-17 17:24:45.820558 lucupy-0.1.9/LICENSE
--rw-r--r--   0        0        0     1006 2022-10-17 17:24:45.820882 lucupy-0.1.9/README.rst
--rw-r--r--   0        0        0     1026 2022-10-17 17:24:45.821333 lucupy-0.1.9/lucupy/__init__.py
--rw-r--r--   0        0        0      734 2022-10-17 17:24:45.821567 lucupy-0.1.9/lucupy/decorators/__init__.py
--rw-r--r--   0        0        0     7408 2022-10-17 17:24:45.821843 lucupy-0.1.9/lucupy/helpers/__init__.py
--rw-r--r--   0        0        0      636 2022-10-17 17:24:45.822222 lucupy-0.1.9/lucupy/minimodel/__init__.py
--rw-r--r--   0        0        0     1309 2022-10-17 17:24:45.822493 lucupy-0.1.9/lucupy/minimodel/atom.py
--rw-r--r--   0        0        0     8328 2022-10-17 17:24:45.822840 lucupy-0.1.9/lucupy/minimodel/constraints.py
--rw-r--r--   0        0        0     9204 2022-11-09 03:07:10.325056 lucupy-0.1.9/lucupy/minimodel/group.py
--rw-r--r--   0        0        0     2766 2022-10-17 17:24:45.823700 lucupy-0.1.9/lucupy/minimodel/magnitude.py
--rw-r--r--   0        0        0    10051 2022-11-09 03:07:10.325546 lucupy-0.1.9/lucupy/minimodel/observation.py
--rw-r--r--   0        0        0      974 2022-10-17 17:24:45.824269 lucupy-0.1.9/lucupy/minimodel/observationmode.py
--rw-r--r--   0        0        0     4715 2022-11-09 03:07:10.326105 lucupy-0.1.9/lucupy/minimodel/program.py
--rw-r--r--   0        0        0      780 2022-10-17 17:24:45.824744 lucupy-0.1.9/lucupy/minimodel/qastate.py
--rw-r--r--   0        0        0     1055 2022-10-17 17:24:45.825010 lucupy-0.1.9/lucupy/minimodel/resource.py
--rw-r--r--   0        0        0      914 2022-10-17 17:24:45.825413 lucupy-0.1.9/lucupy/minimodel/semester.py
--rw-r--r--   0        0        0     1562 2022-10-17 17:24:45.825817 lucupy-0.1.9/lucupy/minimodel/site.py
--rw-r--r--   0        0        0     2878 2022-10-17 17:24:45.826095 lucupy-0.1.9/lucupy/minimodel/target.py
--rw-r--r--   0        0        0     2135 2022-10-17 17:24:45.826341 lucupy-0.1.9/lucupy/minimodel/timeallocation.py
--rw-r--r--   0        0        0     1364 2022-10-17 17:24:45.826580 lucupy-0.1.9/lucupy/minimodel/timingwindow.py
--rw-r--r--   0        0        0      844 2022-10-17 17:24:45.826826 lucupy-0.1.9/lucupy/minimodel/too.py
--rw-r--r--   0        0        0      424 2022-11-07 18:10:11.047500 lucupy-0.1.9/lucupy/observatory/__init__.py
--rw-r--r--   0        0        0     3262 2022-10-20 01:15:57.052740 lucupy-0.1.9/lucupy/observatory/abstract/__init__.py
--rw-r--r--   0        0        0      245 2022-10-06 01:52:10.238720 lucupy-0.1.9/lucupy/observatory/gemini/__init__.py
--rw-r--r--   0        0        0     1119 2022-11-09 03:07:10.326550 lucupy-0.1.9/lucupy/observatory/gemini/geminiobservation.py
--rw-r--r--   0        0        0     3599 2022-10-31 08:20:40.160082 lucupy-0.1.9/lucupy/observatory/gemini/geminiproperties.py
--rw-r--r--   0        0        0      606 2022-10-17 17:17:40.108151 lucupy-0.1.9/lucupy/sky/__init__.py
--rw-r--r--   0        0        0     4426 2022-10-17 17:24:45.829186 lucupy-0.1.9/lucupy/sky/altitude.py
--rw-r--r--   0        0        0     9312 2022-10-17 17:24:45.830370 lucupy-0.1.9/lucupy/sky/brightness.py
--rw-r--r--   0        0        0     2039 2022-10-17 17:24:45.830966 lucupy-0.1.9/lucupy/sky/constants.py
--rw-r--r--   0        0        0     3136 2022-10-17 17:24:45.831527 lucupy-0.1.9/lucupy/sky/events.py
--rw-r--r--   0        0        0    21553 2022-10-17 17:24:45.832550 lucupy-0.1.9/lucupy/sky/moon.py
--rw-r--r--   0        0        0     8763 2022-10-17 17:24:45.833321 lucupy-0.1.9/lucupy/sky/sun.py
--rw-r--r--   0        0        0    14876 2022-10-17 17:24:45.833972 lucupy-0.1.9/lucupy/sky/utils.py
--rw-r--r--   0        0        0     4248 2022-10-17 17:24:45.834519 lucupy-0.1.9/lucupy/timeutils/__init__.py
--rw-r--r--   0        0        0      558 2022-11-09 03:07:10.338478 lucupy-0.1.9/lucupy/types/__init__.py
--rw-r--r--   0        0        0     1998 2022-11-09 03:07:10.327506 lucupy-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1975 1970-01-01 00:00:00.000000 lucupy-0.1.9/setup.py
--rw-r--r--   0        0        0     1916 1970-01-01 00:00:00.000000 lucupy-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1528 2024-05-20 20:53:43.487496 lucupy-0.1.90/LICENSE
+-rw-r--r--   0        0        0     1006 2024-05-20 20:53:43.487496 lucupy-0.1.90/README.rst
+-rw-r--r--   0        0        0     1026 2024-05-20 20:53:43.487496 lucupy-0.1.90/lucupy/__init__.py
+-rw-r--r--   0        0        0     1425 2024-05-20 20:53:43.487496 lucupy-0.1.90/lucupy/decorators/__init__.py
+-rw-r--r--   0        0        0    14345 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/helpers/__init__.py
+-rw-r--r--   0        0        0      566 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/meta/__init__.py
+-rw-r--r--   0        0        0     1013 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/minimodel/__init__.py
+-rw-r--r--   0        0        0     1943 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/minimodel/atom.py
+-rw-r--r--   0        0        0    10302 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/minimodel/constraints.py
+-rw-r--r--   0        0        0    15891 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/minimodel/group.py
+-rw-r--r--   0        0        0     1405 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/minimodel/ids.py
+-rw-r--r--   0        0        0     3042 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/minimodel/magnitude.py
+-rw-r--r--   0        0        0     1016 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/minimodel/obs_filter.py
+-rw-r--r--   0        0        0    13191 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/minimodel/observation.py
+-rw-r--r--   0        0        0      934 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/minimodel/observationmode.py
+-rw-r--r--   0        0        0     7001 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/minimodel/program.py
+-rw-r--r--   0        0        0      769 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/minimodel/qastate.py
+-rw-r--r--   0        0        0     2175 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/minimodel/resource.py
+-rw-r--r--   0        0        0      544 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/minimodel/resource_type.py
+-rw-r--r--   0        0        0     3683 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/minimodel/semester.py
+-rw-r--r--   0        0        0     3111 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/minimodel/site.py
+-rw-r--r--   0        0        0     3036 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/minimodel/target.py
+-rw-r--r--   0        0        0     2237 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/minimodel/timeallocation.py
+-rw-r--r--   0        0        0     1466 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/minimodel/timingwindow.py
+-rw-r--r--   0        0        0      906 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/minimodel/too.py
+-rw-r--r--   0        0        0      367 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/minimodel/wavelength.py
+-rw-r--r--   0        0        0      424 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/observatory/__init__.py
+-rw-r--r--   0        0        0     3185 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/observatory/abstract/__init__.py
+-rw-r--r--   0        0        0      245 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/observatory/gemini/__init__.py
+-rw-r--r--   0        0        0     1225 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/observatory/gemini/geminiobservation.py
+-rw-r--r--   0        0        0     4951 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/observatory/gemini/geminiproperties.py
+-rw-r--r--   0        0        0     4168 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/plot/__init__.py
+-rw-r--r--   0        0        0      212 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/resource_manager/__init__.py
+-rw-r--r--   0        0        0     1924 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/resource_manager/resource_manager.py
+-rw-r--r--   0        0        0      606 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/sky/__init__.py
+-rw-r--r--   0        0        0     4564 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/sky/altitude.py
+-rw-r--r--   0        0        0     9428 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/sky/brightness.py
+-rw-r--r--   0        0        0     2488 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/sky/constants.py
+-rw-r--r--   0        0        0     3175 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/sky/events.py
+-rw-r--r--   0        0        0    21630 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/sky/moon.py
+-rw-r--r--   0        0        0     8820 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/sky/sun.py
+-rw-r--r--   0        0        0    15144 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/sky/utils.py
+-rw-r--r--   0        0        0     5545 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/timeutils/__init__.py
+-rw-r--r--   0        0        0     1334 2024-05-20 20:53:43.491496 lucupy-0.1.90/lucupy/types/__init__.py
+-rw-r--r--   0        0        0     2016 2024-05-20 20:53:43.495496 lucupy-0.1.90/pyproject.toml
+-rw-r--r--   0        0        0     2020 1970-01-01 00:00:00.000000 lucupy-0.1.90/PKG-INFO
```

### Comparing `lucupy-0.1.9/LICENSE` & `lucupy-0.1.90/LICENSE`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.9/README.rst` & `lucupy-0.1.90/README.rst`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.9/lucupy/__init__.py` & `lucupy-0.1.90/lucupy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2016-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
+# Copyright (c) 2016-2024 Association of Universities for Research in Astronomy, Inc. (AURA)
 # For license information see LICENSE or https://opensource.org/licenses/BSD-3-Clause
 """ # Lucupy
 
 This package contains data structures and functions to support all the microservices that make up the Schedule app
 for the Gemini Program Plataform (and other auxiliary services such as Env and Resource)
 
 ##Content
```

### Comparing `lucupy-0.1.9/lucupy/minimodel/constraints.py` & `lucupy-0.1.90/lucupy/minimodel/constraints.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,43 @@
-# Copyright (c) 2016-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
+# Copyright (c) 2016-2024 Association of Universities for Research in Astronomy, Inc. (AURA)
 # For license information see LICENSE or https://opensource.org/licenses/BSD-3-Clause
 
-from dataclasses import dataclass
-from datetime import datetime
+from __future__ import annotations
+
+from dataclasses import dataclass, field
 from enum import Enum, IntEnum, auto
-from typing import ClassVar, List, Optional, Sequence, Union
+from typing import ClassVar, List, Optional, Sequence, final
 
 import numpy as np
 import numpy.typing as npt
 from astropy.coordinates import Angle
 from astropy.units import Quantity
+from astropy import units as u
 
 from lucupy.helpers import flatten
 from lucupy.types import ScalarOrNDArray
 
+from ..decorators import immutable
 from .timingwindow import TimingWindow
 
+__all__ = [
+    'CloudCover',
+    'Conditions',
+    'Constraints',
+    'ElevationType',
+    'ImageQuality',
+    'SkyBackground',
+    'Strehl',
+    'Variant',
+    'VariantSnapshot',
+    'WaterVapor',
+]
+
 
+@final
 class SkyBackground(float, Enum):
     """
     Bins for observation sky background requirements or current conditions.
 
     Members:
         - SB20 = 0.2
         - SB50 = 0.5
@@ -30,14 +47,15 @@
     """
     SB20 = 0.2
     SB50 = 0.5
     SB80 = 0.8
     SBANY = 1.0
 
 
+@final
 class CloudCover(float, Enum):
     """
     Bins for observation cloud cover requirements or current conditions.
 
     Members:
         - CC50 = 0.5
         - CC70 = 0.7
@@ -46,14 +64,15 @@
     """
     CC50 = 0.5
     CC70 = 0.7
     CC80 = 0.8
     CCANY = 1.0
 
 
+@final
 class ImageQuality(float, Enum):
     """
     Bins for observation image quality requirements or current conditions.
 
     Members:
         - IQ20 = 0.2
         - IQ70 = 0.7
@@ -63,14 +82,15 @@
     """
     IQ20 = 0.2
     IQ70 = 0.7
     IQ85 = 0.85
     IQANY = 1.0
 
 
+@final
 class WaterVapor(float, Enum):
     """
     Bins for observation water vapor requirements or current conditions.
 
     Members:
         - WV20 = 0.2
         - WV50 = 0.5
@@ -80,14 +100,15 @@
     """
     WV20 = 0.2
     WV50 = 0.5
     WV80 = 0.8
     WVANY = 1.0
 
 
+@final
 class Strehl(float, Enum):
     """
     The Strehl ratio is a measure of the quality of optical image formation.
     Used variously in situations where optical resolution is compromised due to lens aberrations or due to imaging
     through the turbulent atmosphere, the Strehl ratio has a value between 0 and 1, with a hypothetical, perfectly
     unaberrated optical system having a Strehl ratio of 1. (Source: Wikipedia.)
 
@@ -104,29 +125,32 @@
     S02 = 0.2
     S04 = 0.4
     S06 = 0.6
     S08 = 0.8
     S10 = 1.0
 
 
+@final
 class ElevationType(IntEnum):
     """
     The type of elevation constraints in the observing conditions.
 
     Members:
        - NONE
        - HOUR_ANGLE
        - AIRMASS
     """
     NONE = auto()
     HOUR_ANGLE = auto()
     AIRMASS = auto()
 
 
-@dataclass(order=True, frozen=True)
+@final
+@immutable
+@dataclass(frozen=True)
 class Conditions:
     """
     A set of conditions.
 
     Note that we make this dataclass eq and ordered so that we can compare one
     set of conditions with another to see if one satisfies the other.
 
@@ -143,15 +167,15 @@
     cc: ScalarOrNDArray[CloudCover]
     iq: ScalarOrNDArray[ImageQuality]
     sb: ScalarOrNDArray[SkyBackground]
     wv: ScalarOrNDArray[WaterVapor]
 
     # Least restrictive conditions.
     @classmethod
-    def least_restrictive(cls) -> 'Conditions':
+    def least_restrictive(cls) -> Conditions:
         """
         Return the least possible restrictive conditions.
         """
         return cls(cc=CloudCover.CCANY,
                    iq=ImageQuality.IQANY,
                    sb=SkyBackground.SBANY,
                    wv=WaterVapor.WVANY)
@@ -167,15 +191,15 @@
         are_arrays = isinstance(self.cc, np.ndarray)
         if are_arrays:
             uniform_lengths = len({self.cc.size, self.iq.size, self.sb.size, self.wv.size}) == 1
             if not uniform_lengths:
                 raise ValueError(f'Conditions have a variable number of array sizes: {self}')
 
     @staticmethod
-    def most_restrictive_conditions(conditions: Sequence['Conditions']) -> 'Conditions':
+    def most_restrictive_conditions(conditions: Sequence[Conditions]) -> Conditions:
         """
         Given an iterable of conditions, find the most restrictive amongst the set.
         If no conditions are given, return the most flexible conditions possible.
         """
         if len(conditions) == 0:
             return Conditions.least_restrictive()
         min_cc = min(flatten(c.cc for c in conditions), default=CloudCover.CCANY)
@@ -188,15 +212,17 @@
         """
         For array values, return the length of the arrays.
         For scalar values, return a length of 1.
         """
         return len(self.cc) if isinstance(self.cc, np.ndarray) else 1
 
 
-@dataclass
+@final
+@immutable
+@dataclass(frozen=True)
 class Constraints:
     """The constraints required for an observation to be performed.
 
     Default airmass values to use for elevation constraints if:
         1. The Constraints are not present in the Observation at all; or
         2. The elevation_type is set to NONE.
 
@@ -209,49 +235,42 @@
         strehl (Strehl:optional): None
 
         DEFAULT_AIRMASS_ELEVATION_MIN (ClassVar[float]): 1.0
         DEFAULT_AIRMASS_ELEVATION_MAX (ClassVar[float]): 2.3
 
     """
     conditions: Conditions
-    # constrast: Constrast
     elevation_type: ElevationType
     elevation_min: float
     elevation_max: float
     timing_windows: List[TimingWindow]
     # clearance_windows: Optional[List[ClearanceWindow]] = None
     strehl: Optional[Strehl] = None
 
     # Default airmass values to use for elevation constraints if:
     # 1. The Constraints are not present in the Observation at all; or
     # 2. The elevation_type is set to NONE.
-    DEFAULT_AIRMASS_ELEVATION_MIN: ClassVar[float] = 1.0
-    DEFAULT_AIRMASS_ELEVATION_MAX: ClassVar[float] = 2.3
+    DEFAULT_AIRMASS_ELEVATION_MIN: ClassVar[float] = field(init=False, default=1.0, repr=False, compare=False)
+    DEFAULT_AIRMASS_ELEVATION_MAX: ClassVar[float] = field(init=False, default=2.05, repr=False, compare=False)
 
 
-@dataclass(order=True, eq=True, frozen=True)
+@final
+@immutable
+@dataclass(frozen=True)
 class Variant:
-    """A weather variant.
-    wind_speed should be in m / s.
-
+    """
+    A weather variant.
     Attributes:
-
-        start_time (datetime): Time of the variant.
         iq (Union[npt.NDArray[ImageQuality], ImageQuality]): Image quality.
         cc (Union[npt.NDArray[CloudCover], CloudCover]): Cloud Cover.
-        wind_dir (Angle): Wind direction.
-        wind_spd (Quantity): Wind speed.
-
+        wind_dir (Angle): Wind direction (degrees).
+        wind_spd (Quantity): Wind speed (m/s).
     """
-    # TODO: No idea what time blocks are. Note this could be a list or a single value.
-    # TODO: Because of this, we cannot hash Variants, which is problematic.
-
-    start_time: datetime
-    iq: Union[npt.NDArray[ImageQuality], ImageQuality]
-    cc: Union[npt.NDArray[CloudCover], CloudCover]
+    iq: npt.NDArray[ImageQuality] | ImageQuality
+    cc: npt.NDArray[CloudCover] | CloudCover
     wind_dir: Angle
     wind_spd: Quantity
 
     def __post_init__(self):
         """
         Ensure that if any arrays are specified, all values are specified arrays of the same size.
         """
@@ -264,7 +283,54 @@
                          np.asarray(self.wind_spd).size}
         if are_arrays:
             uniform_lengths = len({len(self.cc), len(self.iq)}.union(array_lengths)) == 1
         else:
             uniform_lengths = len(array_lengths) == 1
         if not uniform_lengths:
             raise ValueError(f'Variant has a variable number of array sizes: {self}')
+
+
+@final
+@immutable
+@dataclass(frozen=True)
+class VariantSnapshot:
+    """
+    A snapshot of a variant: this is used to keep track of weather changes or the current state of
+    the weather at a site.
+
+    wind_dir should be in degrees.
+    wind_speed should be in m / s.
+
+    Attributes:
+        iq (ImageQuality): Image quality.
+        cc (CloudCover): Cloud cover.
+        wind_dir (Angle): Wind direction (in degrees). Should be scalar.
+        wind_spd (Quantity): Wind speed (in m/s). Should be scalar.
+    """
+    iq: ImageQuality
+    cc: CloudCover
+    wind_dir: Angle
+    wind_spd: Quantity
+
+    def __post_init__(self):
+        if self.wind_dir.size != 1:
+            raise ValueError(f'Wind direction should be scalar, but has size {self.wind_dir.size}.')
+        if self.wind_spd.unit != u.m / u.s:
+            raise ValueError(f'Wind speed should be in m / s, but {self.wind_spd.unit} specified.')
+        if self.wind_spd.size != 1:
+            raise ValueError(f'Wind speed should be scalar, but has size {self.wind_spd.size}.')
+
+    def make_variant(self, num_timeslots: int) -> Variant:
+        """
+        Create a Variant object with the specified number of timeslots.
+        """
+        if num_timeslots <= 0:
+            raise ValueError(f'Request to make a Variant for illegal number of timeslots: {num_timeslots}.')
+
+        cc_array = np.array([self.cc] * num_timeslots)
+        iq_array = np.array([self.iq] * num_timeslots)
+        wind_dir_array = Angle(np.full(num_timeslots, self.wind_dir.value), unit=self.wind_dir.unit)
+        wind_spd_array = np.full(num_timeslots, self.wind_spd.value) * self.wind_spd.unit
+        return Variant(iq=iq_array,
+                       cc=cc_array,
+                       wind_dir=wind_dir_array,
+                       wind_spd=wind_spd_array)
```

### Comparing `lucupy-0.1.9/lucupy/minimodel/magnitude.py` & `lucupy-0.1.90/lucupy/minimodel/magnitude.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,65 @@
-# Copyright (c) 2016-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
+# Copyright (c) 2016-2024 Association of Universities for Research in Astronomy, Inc. (AURA)
 # For license information see LICENSE or https://opensource.org/licenses/BSD-3-Clause
 
 from dataclasses import dataclass
 from enum import Enum, auto
-from typing import Optional
+from typing import FrozenSet, Optional, TypeAlias, final
 
+from ..decorators import immutable
 
+__all__ = [
+    'MagnitudeBand',
+    'MagnitudeBands',
+    'Magnitude',
+    'Magnitudes',
+    'MagnitudeSystem',
+]
+
+
+@final
 class MagnitudeSystem(Enum):
     """
     List of magnitude systems associated with magnitude bands.
 
     Members:
        - VEGA
        - AB
        - JY
     """
     VEGA = auto()
     AB = auto()
     JY = auto()
 
 
+@final
+@immutable
 @dataclass(frozen=True)
 class MagnitudeBand:
     """They are fully enumerated in MagnitudeBands, so they should be looked up by name there.
     THIS CLASS SHOULD NOT BE INSTANTIATED.
 
     Values for center and width are specified in microns.
 
     Attributes:
         name (str):
         center (float):
         width (float):
-        system (MagnitudeSystem): Default to MagnitudeSystem.VEGA .
+        system (MagnitudeSystem): Default to MagnitudeSystem.VEGA
         description (str, optional): Default to None.
 
     """
     name: str
     center: float
     width: float
     system: MagnitudeSystem = MagnitudeSystem.VEGA
     description: Optional[str] = None
 
 
+@final
 class MagnitudeBands(Enum):
     """
     It is unconventional to use lowercase characters in an enum, but to differentiate
     them from the uppercase magnitude bands, we must.
 
     Look up the MagnitudeBand from this Enum as follows:
     MagnitudeBands[name]
@@ -69,19 +83,24 @@
     L = MagnitudeBand('L', 3.760, 0.700)
     M = MagnitudeBand('M', 4.770, 0.240)
     N = MagnitudeBand('N', 10.470, 5.230)
     Q = MagnitudeBand('Q', 20.130, 1.650)
     AP = MagnitudeBand('AP', 0.550, 0.085, description='apparent')
 
 
+@final
+@immutable
 @dataclass(frozen=True)
 class Magnitude:
     """A magnitude value in a particular band.
 
     Attributes:
         band (MagnitudeBands):
         value (float):
         error (float): Default to None.
     """
     band: MagnitudeBands
     value: float
     error: Optional[float] = None
+
+
+Magnitudes: TypeAlias = FrozenSet[Magnitude]
```

### Comparing `lucupy-0.1.9/lucupy/minimodel/observation.py` & `lucupy-0.1.90/lucupy/minimodel/observation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,87 +1,108 @@
-# Copyright (c) 2016-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
+# Copyright (c) 2016-2024 Association of Universities for Research in Astronomy, Inc. (AURA)
 # For license information see LICENSE or https://opensource.org/licenses/BSD-3-Clause
 
+from __future__ import annotations
+
 from dataclasses import dataclass
 from datetime import timedelta
 from enum import IntEnum, auto
-from typing import FrozenSet, List, Mapping, NoReturn, Optional
+from typing import List, Mapping, Optional, final
+
+import numpy as np
+import numpy.typing as npt
 
-from lucupy.observatory.abstract import ObservatoryProperties
+from lucupy.types import ZeroTime
 
 from .atom import Atom
 from .constraints import Constraints
+from .ids import ObservationID, ProgramID, UniqueGroupID
+from .observationmode import ObservationMode
 from .qastate import QAState
-from .resource import Resource
+from .resource import Resource, Resources
 from .site import Site
 from .target import Target, TargetType
 from .too import TooType
-from ..types import ZeroTime
+from .wavelength import Wavelengths
 
-ObservationID = str
+__all__ = [
+    'Observation',
+    'ObservationClass',
+    'ObservationMode',
+    'ObservationStatus',
+    'Priority',
+    'SetupTimeType',
+]
 
 
+@final
 class ObservationStatus(IntEnum):
     """
     The status of an observation as indicated in the Observing Tool / ODB.
 
     Members:
         - NEW
         - INCLUDED
         - PROPOSED
         - APPROVED
         - FOR_REVIEW: Not in original mini-model description, but returned by OCS.
+        - IN_REVIEW
         - ON_HOLD
         - READY
         - ONGOING
         - OBSERVED
         - INACTIVE
         - PHASE2
     """
     NEW = auto()
     INCLUDED = auto()
     PROPOSED = auto()
     APPROVED = auto()
     FOR_REVIEW = auto()
-    # TODO: Not in original mini-model description, but returned by OCS.
+    IN_REVIEW = auto()
     ON_HOLD = auto()
     READY = auto()
     ONGOING = auto()
     OBSERVED = auto()
     INACTIVE = auto()
     PHASE2 = auto()
 
 
+@final
 class Priority(IntEnum):
     """An observation's priority.
-    Note that these are ordered specifically so that we can compare them.
+    Note that these are ordered specifically so that we can compare them, and assigned
+    specific int values so that we can sum over them to get a Program's mean priority over
+    its Observations and get a value in the interval [LOW.value, HIGH.value].
 
     Members:
         - LOW
         - MEDIUM
         - HIGH
     """
-    LOW = auto()
-    MEDIUM = auto()
-    HIGH = auto()
+    LOW = 0
+    MEDIUM = 1
+    HIGH = 2
 
 
+@final
 class SetupTimeType(IntEnum):
     """The setup time type for an observation.
 
     Members:
         - NONE
         - REACQUISITION
         - FULL
     """
     NONE = auto()
     REACQUISITION = auto()
     FULL = auto()
 
 
+@final
 class ObservationClass(IntEnum):
     """The class of an observation.
 
     Note that the order of these is specific and deliberate: they are listed in
     preference order for observation classes, and hence, should not be rearranged.
     These correspond to the values in the OCS when made uppercase.
 
@@ -96,14 +117,15 @@
     """
     SCIENCE = auto()
     PROGCAL = auto()
     PARTNERCAL = auto()
     ACQ = auto()
     ACQCAL = auto()
     DAYCAL = auto()
+    NONE = auto()
 
 
 @dataclass
 class Observation:
     """Representation of an observation.
     Non-obvious fields are documented below.
     Attributes:
@@ -119,16 +141,18 @@
             indicates if a reacquisition, a full setup or just nothing has to be done.
         acq_overhead (timedelta): Time overhead for acquisition.
         obs_class (ObservationClass): Type of Observation.
         targets (List[Target]): should contain a complete list of all targets associated with the observation,
             with the base being in the first position
         guiding (Mapping[Resource, Target]): is a map between guide probe resources and their targets.
         sequence (List[Atom]): Sequence of Atoms that describe the observation.
+        belongs_to (ProgramID): ID for the program the observation belongs to.
         constraints (Constraints, optional): Some observations do not have constraints, e.g. GN-208A-FT-103-6.
         too_type (TooType, optional): Default to None.
+        preimaging: (bool, optional): Pre-imaging observation?
 
     """
     id: ObservationID
     internal_id: str
     order: int
     title: str
     site: Site
@@ -147,26 +171,49 @@
     # TODO:    special processing.
     # TODO: Should this be Optional?
     obs_class: ObservationClass
 
     targets: List[Target]
     guiding: Mapping[Resource, Target]
     sequence: List[Atom]
+    belongs_to: ProgramID
 
     # Some observations do not have constraints, e.g. GN-208A-FT-103-6.
-    constraints: Optional[Constraints]
+    # to mypy complaince we should have an EmptyConstraints
+    constraints: Constraints
 
     too_type: Optional[TooType] = None
+    preimaging: bool = False
+
+    @property
+    def to_unique_group_id(self) -> UniqueGroupID:
+        """
+        A method to return the UniqueGroupID that contains this observation.
+        """
+        return self.id.to_unique_group_id
+
+    @property
+    def unique_id(self) -> ObservationID:
+        """
+        Unique ID for the Observation to amalgamate all the IDs from Group down to Observation.
+        This way, for any group, group.children will return an ID, giving a mixed list of UniqueGroupID and
+        ObservationID, which will be used to select the top level groups.
+        """
+        return self.id
 
     def base_target(self) -> Optional[Target]:
         """
         Returns:
             Get the base target for this Observation if it has one, and None otherwise.
         """
-        return next(filter(lambda t: t.type == TargetType.BASE, self.targets), None)
+        def filter_by_type(t: Optional[Target]):
+            if t is not None:
+                return t.type == TargetType.BASE
+
+        return next(filter(lambda t: filter_by_type(t), self.targets), None)
 
     def exec_time(self) -> timedelta:
         """
         Returns:
             Total execution time for the program, which is the sum across atoms and the acquisition overhead.
         """
         return sum((atom.exec_time for atom in self.sequence), ZeroTime) + self.acq_overhead
@@ -174,114 +221,156 @@
     def total_used(self) -> timedelta:
         """
         Returns:
             Total program time used: includes program time and partner time.
         """
         return self.program_used() + self.partner_used()
 
-    def required_resources(self) -> FrozenSet[Resource]:
+    def required_resources(self) -> Resources:
         """
         Returns:
             The required resources for an observation based on the sequence's needs.
         """
         # TODO: For now, we do not return guiding keys amongst the resources.
         # return frozenset(self.guiding.keys() | {r for a in self.sequence for r in a.resources})
-        return frozenset((r for a in self.sequence for r in a.resources))
+        return frozenset({self.site.resource} | {r for a in self.sequence for r in a.resources})
 
     def instrument(self) -> Optional[Resource]:
         """
         Returns:
             A resource that is an instrument, if one exists. There should be only one.
         """
-        return next(filter(lambda r: ObservatoryProperties.is_instrument(r),
+        def check_instrument(r: Optional[Resource]):
+            if r is not None:
+                # To avoid a circular import.
+                from lucupy.observatory.abstract import ObservatoryProperties
+                return ObservatoryProperties.is_instrument(r)
+
+        return next(filter(lambda r: check_instrument(r),
                            self.required_resources()), None)
 
-    def wavelengths(self) -> FrozenSet[float]:
-        """
-        Returns:
-            The set of wavelengths included in the sequence.
-        """
-        return frozenset((w for c in self.sequence for w in c.wavelengths))
+    def is_nir(self) -> bool:
+        """Define if the observation is a NIR observation or not."""
+        inst_req = self.instrument()
+        # To avoid a circular import.
+        from lucupy.observatory.abstract import ObservatoryProperties
+        return any(inst_req == nir_ins for nir_ins in ObservatoryProperties.nir_instruments())
 
-    def constraints(self) -> FrozenSet[Constraints]:
+    def wavelengths(self) -> Wavelengths:
         """
         Returns:
-            A set of the constraints required by the observation.
-            In the case of an observation, this is just the (optional) constraints.
+            The set of wavelengths included in the sequence.
         """
-        return frozenset([self.constraints] if self.constraints is not None else [])
+        return frozenset(w for c in self.sequence for w in c.wavelengths)
 
     def program_used(self) -> timedelta:
         """We roll this information up from the atoms as it will be calculated
             during the Optimizer algorithm. Note that it is also available directly
             from the OCS, which is used to populate the time allocation.
         Returns:
             (timedelta): With the time program used.
         """
-        return sum((atom.prog_time for atom in self.sequence), start=ZeroTime)
+        return sum((atom.program_used for atom in self.sequence), start=ZeroTime)
 
     def partner_used(self) -> timedelta:
         """We roll this information up from the atoms as it will be calculated
         during the Optimizer algorithm. Note that it is also available directly
         from the OCS, which is used to populate the time allocation.
 
         Returns:
-            (timedelta): With the time program used.
+            (timedelta): With the time partner used.
+        """
+        return sum((atom.partner_used for atom in self.sequence), start=ZeroTime)
+
+    def prog_time(self) -> timedelta:
+        """We roll this information up from the atoms.
+
+        Returns:
+            (timedelta): With the total planned program time.
         """
-        return sum((atom.part_time for atom in self.sequence), start=ZeroTime)
+        acq_time = ZeroTime
+        if self.obs_class in [ObservationClass.SCIENCE, ObservationClass.PROGCAL]:
+            acq_time = self.acq_overhead
+
+        return sum((atom.prog_time for atom in self.sequence), start=acq_time)
+
+    def part_time(self) -> timedelta:
+        """We roll this information up from the atoms.
+
+        Returns:
+            (timedelta): With the total planned partner time.
+        """
+        acq_time = ZeroTime
+        if self.obs_class in [ObservationClass.PARTNERCAL]:
+            acq_time = self.acq_overhead
+
+        return sum((atom.part_time for atom in self.sequence), start=acq_time)
+
+    def cumulative_exec_times(self) -> npt.NDArray[timedelta]:
+        """Cumulative series of execution times for the unobserved atoms
+        in a sequence, excluding acquisition time."""
+        cum_seq = [atom.exec_time if not atom.observed else ZeroTime for atom in self.sequence]
+        return np.cumsum(cum_seq)
+
+    def not_charged(self) -> timedelta:
+        """not_charged time rolled up from atoms"""
+        return sum((atom.not_charged for atom in self.sequence), start=ZeroTime)
 
     @staticmethod
     def _select_obsclass(classes: List[ObservationClass]) -> Optional[ObservationClass]:
         """Given a list of non-empty ObservationClasses, determine which occurs with
-        highest precedence in the ObservationClasses enum, i.e. has the lowest index.
+        the highest precedence in the ObservationClasses enum, i.e. has the lowest index.
 
         This will be used when examining the sequence for atoms.
 
         Returns:
             (ObservationClass): Lowest-index ObservationClasses or None if the list is empty.
         """
         # TODO: Move this to the ODB program extractor as the logic is used there.
         # TODO: Remove from Bryan's atomizer.
         return min(classes, default=None)
 
     @staticmethod
     def _select_qastate(qastates: List[QAState]) -> Optional[QAState]:
         """
-        Given a list of non-empty QAStates, determine which occurs with
+        Given a list of non-empty QAStates, determine which occurs with the
         highest precedence in the QAStates enum, i.e. has the lowest index.
 
         Returns:
             (QAState): Lowest-index QAStates or None if the list is empty.
         """
         # TODO: Move this to the ODB program extractor as the logic is used there.
         # TODO: Remove from Bryan's atomizer.
 
         return min(qastates, default=None)
 
-    def show(self, depth: int = 1) -> NoReturn:
+    def obs_mode(self) -> ObservationMode:
+        return self.sequence[0].obs_mode
+
+    def show(self, depth: int = 1) -> None:
         """Print content of the Observation.
 
         Args:
             depth (int, optional): depth of the separator. Defaults to 1.
         """
         def sep(indent: int) -> str:
-            return '----- ' * indent
+            return '-----' * indent
 
-        print(f'{sep(depth)} Observation: {self.id}')
+        print(f'{sep(depth)} Observation: {self.id.id} {self.status.name}')
         for atom in self.sequence:
             print(f'{sep(depth + 1)} {atom}')
 
     def __len__(self):
         """
         This is to treat observations the same as groups and is a bit of a hack.
         Observations are to be placed in AND Groups of size 1 for scheduling purposes.
         """
         return 1
 
-    def __eq__(self, other: 'Observation') -> bool:
+    def __eq__(self, other: Observation) -> bool:  # type: ignore[override]
         """
         We override the equality checker created by @dataclass to temporarily skip sequence
         comparison in test cases until the atom creation process is finish.
         """
 
         return (dict((k, v) for k, v in self.__dict__.items() if k != 'sequence') ==
                 dict((k, v) for k, v in other.__dict__.items() if k != 'sequence'))
```

### Comparing `lucupy-0.1.9/lucupy/minimodel/program.py` & `lucupy-0.1.90/lucupy/minimodel/program.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,63 @@
-# Copyright (c) 2016-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
+# Copyright (c) 2016-2024 Association of Universities for Research in Astronomy, Inc. (AURA)
 # For license information see LICENSE or https://opensource.org/licenses/BSD-3-Clause
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from datetime import datetime, timedelta
 from enum import Enum, IntEnum, auto
-from typing import ClassVar, FrozenSet, List, Optional
+from typing import ClassVar, FrozenSet, List, Optional, final
 
-from .group import AndGroup, Group, GroupID
-from .observation import Observation
+import numpy as np
+
+from lucupy.decorators import immutable
+from lucupy.types import ZeroTime
+from lucupy.minimodel.obs_filter import obs_is_not_inactive, obs_is_science_or_progcal
+
+from .group import ROOT_GROUP_ID, AndGroup, Group
+from .ids import ObservationID, ProgramID, UniqueGroupID
+from .observation import Observation, Priority
 from .semester import Semester
 from .timeallocation import TimeAllocation
 from .too import TooType
-from ..types import ZeroTime
 
-ProgramID = str
+__all__ = [
+    'Band',
+    'Program',
+    'ProgramMode',
+    'ProgramType',
+    'ProgramTypes',
+]
 
 
+@final
 class Band(IntEnum):
     """
     Program band.
     """
     BAND1 = 1
     BAND2 = 2
     BAND3 = 3
     BAND4 = 4
 
 
+@final
 class ProgramMode(IntEnum):
     """
     Main operational mode, which is one of:
     * Queue
     * Classical
     * Priority Visitor (hybrid mode between queue and classical)
     """
     QUEUE = auto()
     CLASSICAL = auto()
     PV = auto()
 
 
+@final
+@immutable
 @dataclass(frozen=True)
 class ProgramType:
     """
     Represents the information encompassing the type of program.
     * abbreviation: the code used by the program type (e.g. Q, C, FT, LP)
     * name: user readable representation of the program type
     * is_science: indicates if this program type is a science program
@@ -51,14 +67,15 @@
     and should be accessed from there.
     """
     abbreviation: str
     name: str
     is_science: bool = True
 
 
+@final
 class ProgramTypes(Enum):
     """
     A complete list of the ProgramType instances used by Gemini.
     As mentioned in ProgramType, ProgramType should never be instantiated
     outside of this enum: instead, ProgramType instances should be retrieved
     from here.
     """
@@ -69,15 +86,16 @@
     ENG = ProgramType('ENG', 'Engineering', False)
     FT = ProgramType('FT', 'Fast Turnaround')
     LP = ProgramType('LP', 'Large Program')
     Q = ProgramType('Q', 'Queue')
     SV = ProgramType('SV', 'System Verification')
 
 
-@dataclass(unsafe_hash=True)
+@final
+@dataclass
 class Program:
     """
     Representation of a program.
 
     The FUZZY_BOUNDARY is a constant that allows for a fuzzy boundary for a program's
     start and end times.
     """
@@ -87,20 +105,28 @@
     semester: Optional[Semester]
     band: Band
     thesis: bool
     mode: ProgramMode
     type: Optional[ProgramTypes]
     start: datetime
     end: datetime
-    allocated_time: FrozenSet[TimeAllocation]
+    allocated_time: FrozenSet[TimeAllocation] = field(hash=False, compare=False)
+
+    # Root group is immutable and should not be used in hashing or comparisons.
     root_group: AndGroup
+
     too_type: Optional[TooType] = None
 
     FUZZY_BOUNDARY: ClassVar[timedelta] = timedelta(days=14)
 
+    def __post_init__(self):
+        if self.root_group.id != ROOT_GROUP_ID:
+            raise ValueError(f"Program {self.id.id} should have root group should named {ROOT_GROUP_ID.id}, received: "
+                             f'"{self.root_group.id}".')
+
     def program_awarded(self) -> timedelta:
         return sum((t.program_awarded for t in self.allocated_time), ZeroTime)
 
     def program_awarded_used(self) -> timedelta:
         return sum((t.program_used for t in self.allocated_time), ZeroTime)
 
     def partner_awarded(self) -> timedelta:
@@ -120,32 +146,68 @@
 
     def partner_used(self) -> timedelta:
         return self.root_group.partner_used()
 
     def total_used(self) -> timedelta:
         return self.root_group.total_used()
 
+    def not_charged(self) -> timedelta:
+        return self.root_group.not_charged()
+
     def observations(self) -> List[Observation]:
         return self.root_group.observations()
 
-    def get_group_ids(self) -> FrozenSet[GroupID]:
-        return self.root_group.subgroup_ids()
-
-    def get_group(self, group_id: GroupID) -> Optional[Group]:
+    def get_group(self, group_id: UniqueGroupID) -> Optional[Group]:
+        """
+        Given a UniqueGroupID, find the subgroup with the ID if it exists.
+        Returns None if no such group can be found.
+        """
         def aux(group: Group) -> Optional[Group]:
-            if group.id == group_id:
+            if group.unique_id == group_id:
                 return group
-            elif group.is_scheduling_group():
+            elif not isinstance(group.children, Observation):
                 for subgroup in group.children:
                     retval = aux(subgroup)
                     if retval is not None:
                         return retval
             return None
 
         return aux(self.root_group)
 
+    def get_observation(self, observation_id: ObservationID) -> Optional[Observation]:
+        """
+        Given an ObservationID, find the Observation with the ID if it exists.
+        Returns None if no such Observation can be found.
+        """
+        def aux(group: Group) -> Optional[Observation]:
+            match group.children:
+                case Observation():
+                    if group.children.id == observation_id:
+                        return group.children
+                    else:
+                        return None
+                case _:
+                    for subgroup in group.children:
+                        check_subgroup = aux(subgroup)
+                        if check_subgroup is not None:
+                            return check_subgroup
+                    return None
+        return aux(self.root_group)
+
+    def mean_priority(self) -> float:
+        """
+        Return the mean user priority from the active SCIENCE and PROGCAL observations.
+        This will be a value in the interval [Priority.LOW.value, Priority.HIGH.value] indicating
+        the mean over Observations.
+
+        :return: float
+        """
+        priorities = [obs.priority.value for obs in self.observations()
+                      if obs_is_science_or_progcal(obs) and obs_is_not_inactive(obs)]
+        return np.mean(priorities) if len(priorities) else Priority.LOW.value
+
     def show(self):
         """Print content of the Program.
         """
-        print(f'Program: {self.id}')
+        print(f'Program: {self.id.id}')
         # Print the group and atom information.
         self.root_group.show(1)
```

### Comparing `lucupy-0.1.9/lucupy/minimodel/site.py` & `lucupy-0.1.90/lucupy/minimodel/site.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,83 @@
-# Copyright (c) 2016-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
+# Copyright (c) 2016-2024 Association of Universities for Research in Astronomy, Inc. (AURA)
 # For license information see LICENSE or https://opensource.org/licenses/BSD-3-Clause
 
 """This will have to be customized by a given observatory if used independently
     of Gemini.
 """
 
 from enum import Enum
-from typing import Optional
+from typing import Final, FrozenSet, Optional, final
+from zoneinfo import ZoneInfo, ZoneInfoNotFoundError
 
-import astropy.coordinates
-import pytz
+from astropy.coordinates import EarthLocation, UnknownSiteException
 
+from lucupy.decorators import immutable
+from lucupy.minimodel.resource import ResourceType
+from lucupy.resource_manager.resource_manager import ResourceManager
 
+__all__ = [
+    'Site',
+    'ALL_SITES',
+]
+
+
+@final
+@immutable
 class Site(Enum):
     """The sites belonging to the observatory using the Scheduler.
 
     Attributes:
         GN: Gemini North (568@399)
         GS: Gemini South (I11@399)
 
     """
     GN = ('Gemini North', '568@399')
     GS = ('Gemini South', 'I11@399')
 
-    def __init__(self, site_name: str, coordinate_center: str, astropy_lookup: Optional[str] = None):
+    def __init__(self, site_name: str,
+                 coordinate_center: str,
+                 *,
+                 location: Optional[EarthLocation] = None,
+                 timezone: Optional[ZoneInfo] = None):
+        """
+        Perform the necessary initialization for a Site object, which is also a Resource.
+        Args:
+            site_name: the name of the site
+            coordinate_center: the coordinate center of the site (probably not needed)
+            location: the EarthLocation of the site, which, if not provided, will be looked up by the site_name
+            timezone: the ZoneInfo timezone at the location which, if not provided, will be looked up by location
+
+        Note: if outdated information is found during lookups (e.g. time zone information is not what one would expect),
+        this may be because AstroPy downloads and caches this data. Clearing the cache to force a re-download may help:
+
+        import astropy.utils.data
+        astropy.utils.data.clear_download_cache()
+        """
         self.site_name = site_name
         self.coordinate_center = coordinate_center
 
-        if astropy_lookup is None:
-            astropy_lookup = site_name.lower().replace(' ', '_')
+        if location is not None:
+            self.location = location
+        else:
+            try:
+                self.location = EarthLocation.of_site(site_name)
+            except UnknownSiteException as ex:
+                msg = f'AstroPy cannot resolve site lookup for location: "{site_name}".'
+                raise ValueError(ex, msg)
+
+        if timezone is not None:
+            self.timezone = timezone
+        else:
+            timezone_name = self.location.info.meta['timezone']
+            try:
+                self.timezone = ZoneInfo(timezone_name)
+            except ZoneInfoNotFoundError as e:
+                msg = f'zoneinfo cannot resolve time zone lookup: {timezone_name}.'
+                raise ValueError(e, msg)
 
-        try:
-            self.location = astropy.coordinates.EarthLocation.of_site(astropy_lookup)
-        except astropy.coordinates.UnknownSiteException as e:
-            msg = f'Unknown site lookup: {astropy_lookup}.'
-            raise ValueError(e, msg)
-
-        timezone_info = self.location.info.meta['timezone']
-        try:
-            self.timezone = pytz.timezone(timezone_info)
-        except pytz.UnknownTimeZoneError as e:
-            msg = f'Unknown time zone lookup: {timezone_info}.'
-            raise ValueError(e, msg)
+        self.resource = ResourceManager().lookup_resource(rid=site_name,
+                                                          rtype=ResourceType.SITE)
 
 
-ALL_SITES = frozenset(s for s in Site)  # A variable to work with all the sites in scheduler components.
+# A variable to work with all the sites in scheduler components as a frozenset.
+ALL_SITES: Final[FrozenSet[Site]] = frozenset(s for s in Site)
```

### Comparing `lucupy-0.1.9/lucupy/minimodel/timeallocation.py` & `lucupy-0.1.90/lucupy/minimodel/timeallocation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,22 @@
-# Copyright (c) 2016-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
+# Copyright (c) 2016-2024 Association of Universities for Research in Astronomy, Inc. (AURA)
 # For license information see LICENSE or https://opensource.org/licenses/BSD-3-Clause
 
 from dataclasses import dataclass
 from datetime import timedelta
 from enum import Enum
+from typing import final
 
+__all__ = [
+    'TimeAccountingCode',
+    'TimeAllocation',
+]
 
+
+@final
 class TimeAccountingCode(str, Enum):
     """
     The time accounting codes for the possible partner submissions or internal program
     types used at Gemini, also known as categories.
 
     This will have to be customized for a given observatory if used independently
     of Gemini.
@@ -31,14 +38,15 @@
     SV = 'System Verification'
     UH = 'University of Hawaii'
     UK = 'United Kingdom'
     US = 'United States'
     XCHK = 'Keck Exchange'
 
 
+@final
 @dataclass
 class TimeAllocation:
     """
     Time allocation information for a given category for a program.
     Programs may be sponsored by multiple categories with different amounts
     of time awarded. This class maintains information about the time awarded
     and the time that has been used, divided between program time and partner
```

### Comparing `lucupy-0.1.9/lucupy/minimodel/timingwindow.py` & `lucupy-0.1.90/lucupy/minimodel/timingwindow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 # Copyright (c) 2016-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
 # For license information see LICENSE or https://opensource.org/licenses/BSD-3-Clause
 
 from dataclasses import dataclass
 from datetime import datetime, timedelta
-from typing import ClassVar, Optional
+from typing import ClassVar, Optional, final
 
+from ..decorators import immutable
 
+__all__ = [
+    'TimingWindow',
+]
+
+
+@final
+@immutable
 @dataclass(frozen=True)
 class TimingWindow:
     """Representation of timing windows in the mini-model.
 
     Attributes:
         start (datetime): When a timing window begins.
         duration (timedelta): For infinite duration, set duration to timedelta.max.
@@ -19,15 +27,15 @@
     start: datetime
     duration: timedelta
     repeat: int
     period: Optional[timedelta]
 
     # For infinite duration, use the length of an LP.
     INFINITE_DURATION_FLAG: ClassVar[int] = -1
-    INFINITE_DURATION: ClassVar[int] = timedelta(days=3 * 365, hours=24)
+    INFINITE_DURATION: ClassVar[timedelta] = timedelta(days=3 * 365, hours=24)
     FOREVER_REPEATING: ClassVar[int] = -1
     NON_REPEATING: ClassVar[int] = 0
     NO_PERIOD: ClassVar[Optional[timedelta]] = None
 
     # A number to be used by the Scheduler to represent infinite repeats from the
     # perspective of the OCS: if FOREVER_REPEATING is selected, then it is converted
     # into this for calculation purposes.
```

### Comparing `lucupy-0.1.9/lucupy/minimodel/too.py` & `lucupy-0.1.90/lucupy/minimodel/too.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,19 @@
-# Copyright (c) 2016-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
+# Copyright (c) 2016-2024 Association of Universities for Research in Astronomy, Inc. (AURA)
 # For license information see LICENSE or https://opensource.org/licenses/BSD-3-Clause
 
 from enum import IntEnum, auto
+from typing import final
 
+__all__ = [
+    'TooType',
+]
 
+
+@final
 class TooType(IntEnum):
     """
     The target-of-opportunity type for a program and for an observation.
     These are ordered specifically so that we can compare them.
 
     The INTERRUPT is considered the highest level of TooType, followed by RAPID, and then STANDARD.
```

### Comparing `lucupy-0.1.9/lucupy/observatory/abstract/__init__.py` & `lucupy-0.1.90/lucupy/observatory/abstract/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,97 @@
-# Copyright (c) 2016-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
+# Copyright (c) 2016-2023 Association of Universities for Research in Astronomy, Inc. (AURA)
 # For license information see LICENSE or https://opensource.org/licenses/BSD-3-Clause
 
+from __future__ import annotations
+
 from abc import ABC
-from datetime import timedelta
-from typing import FrozenSet, NoReturn, Optional
+from typing import Optional, cast
 
 from astropy.time import Time
 
+from lucupy.minimodel.observationmode import ObservationModes
+from lucupy.minimodel.resource import Resource, Resources
+from lucupy.minimodel.wavelength import Wavelengths
+
+__all__ = [
+    'ObservatoryProperties',
+]
+
 
 class ObservatoryProperties(ABC):
     """Observatory-specific methods.
 
        These are not tied to other components or
        structures, and allow computations to be implemented in one place.
 
     """
-    _properties: Optional['ObservatoryProperties'] = None
+    _properties: Optional[ObservatoryProperties] = None
 
     @staticmethod
-    def set_properties(cls) -> NoReturn:
+    def set_properties(cls) -> None:
         """Set properties for an specific Observatory
 
         Raises:
             ValueError: Illegal properties value.
 
         """
         if not issubclass(cls, ObservatoryProperties):
             raise ValueError('Illegal properties value.')
         ObservatoryProperties._properties = cls()
 
     @staticmethod
-    def _check_properties() -> NoReturn:
-        """ Check if any properties are set
+    def _check() -> ObservatoryProperties:
+        """ Check if the properties have been set.
 
         Raises:
             ValueError: Properties have not been set.
-
         """
         if ObservatoryProperties._properties is None:
-            raise ValueError('Properties have not been set.')
+            raise ValueError('Observatory properties have not been set.')
+        return cast(ObservatoryProperties, ObservatoryProperties._properties)
 
     @staticmethod
-    def determine_standard_time(resources: FrozenSet,
-                                wavelengths: FrozenSet[float],
-                                modes: FrozenSet,
+    def determine_standard_time(resources: Resources,
+                                wavelengths: Wavelengths,
+                                modes: ObservationModes,
                                 cal_length: int) -> Time:
         """Determine standard time for a specific Observatory
 
         Args:
-            resources (FrozenSet): Set of Resources(instruments, mask, etc).
-            wavelengths (FrozenSet[float]): An array of Wavelengths to be observed.
-            modes (FrozenSet): The different modes of observation.
+            resources (Resources): Set of Resources(instruments, mask, etc).
+            wavelengths (Wavelengths): An array of Wavelengths to be observed.
+            modes (ObservationModes): The different modes of observation.
             cal_length (int): The length (in seconds) of a calibration.
 
         Returns:
             Time: Value(s) of standard time
         """
-
-        ObservatoryProperties._check_properties()
-        return ObservatoryProperties._properties.determine_standard_time(
+        return ObservatoryProperties._check().determine_standard_time(
             resources,
             wavelengths,
             modes,
             cal_length
         )
 
     @staticmethod
-    def is_instrument(resource) -> bool:
-        """Determine if the given resource is an instrument or not.
+    def nir_instruments() -> Resources:
+        return ObservatoryProperties._check().nir_instruments()
 
-        Args:
-            resource (Resource): An instrument.
+    @staticmethod
+    def instruments() -> Resources:
+        return ObservatoryProperties._check().instruments()
 
-        Returns:
-            bool: True is the resource is an instrument of the Observatory, otherwise False.
-        """
-        ObservatoryProperties._check_properties()
-        return ObservatoryProperties._properties.is_instrument(resource)
+    @staticmethod
+    def is_nir_instrument(resource: Resource) -> bool:
+        return ObservatoryProperties._check().is_nir_instrument(resource)
 
     @staticmethod
-    def acquisition_time(resource, observation_mode) -> Optional[timedelta]:
-        """Given a resource, check if it is an instrument, and if so, lookup the
-           acquisition time for the specified mode.
+    def is_instrument(resource: Resource) -> bool:
+        """Determine if the given resource is an instrument or not.
 
         Args:
-            resource (Resource): A resource that should be an Instrument.
-            observation_mode (ObservationMode): The observation mode to be used.
+            resource (Resource): An instrument.
 
         Returns:
-            Optional[timedelta]: The acquisition time for the instrument in that specific mode.
+            bool: True is the resource is an instrument of the Observatory, otherwise False.
         """
-        ObservatoryProperties._check_properties()
-        return ObservatoryProperties._properties.acquisition_time(resource, observation_mode)
+        return ObservatoryProperties._check().is_instrument(resource)
```

### Comparing `lucupy-0.1.9/lucupy/observatory/gemini/geminiobservation.py` & `lucupy-0.1.90/lucupy/observatory/gemini/geminiobservation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-# Copyright (c) 2016-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
+# Copyright (c) 2016-2024 Association of Universities for Research in Astronomy, Inc. (AURA)
 # For license information see LICENSE or https://opensource.org/licenses/BSD-3-Clause
 
 from datetime import timedelta
-from typing import Final
+from typing import Final, final
 
+from lucupy.observatory.gemini.geminiproperties import GeminiProperties
 from lucupy.minimodel import Observation
+from lucupy.types import ZeroTime
+
+__all__ = [
+    'GeminiObservation',
+    'with_igrins_cal',
+]
 
-from .geminiproperties import GeminiProperties
-from ...types import ZeroTime
 
 _IGRINS_CAL_TIME: Final[timedelta] = timedelta(minutes=10)
 
 
 def with_igrins_cal(func):
     def add_calibration(self):
         if (GeminiProperties.Instruments.IGRINS in self.required_resources()
                 and self.total_used - self.program_time() > ZeroTime):
             return func(self) + _IGRINS_CAL_TIME
         return func(self)
 
     return add_calibration
 
 
+@final
 class GeminiObservation(Observation):
     """A Gemini-specific extension of the Observation class.
     """
 
     @with_igrins_cal
     def total_used(self) -> timedelta:
         """Override total_used method from Observation.
```

### Comparing `lucupy-0.1.9/lucupy/sky/__init__.py` & `lucupy-0.1.90/lucupy/sky/__init__.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.9/lucupy/sky/altitude.py` & `lucupy-0.1.90/lucupy/sky/altitude.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,35 @@
 # https://github.com/jrthorstensen/thorsky/blob/master/thorskyutil.py
 #
 # utility and miscellaneous time and the sky routines built mostly on astropy.
 #
 # Copyright John Thorstensen, 2018, who graciously has allowed Gemini to use this code under the BSD-3 Clause license.
 # For license information see LICENSE or https://opensource.org/licenses/BSD-3-Clause
 
-from typing import Tuple, TypeVar, Union
+from typing import Tuple, TypeAlias, TypeVar, final
 
 import astropy.units as u
 import numpy as np
 import numpy.typing as npt
 from astropy.coordinates import Angle, Longitude
 
+__all__ = [
+    'Altitude',
+    'AngleParam',
+    'ScalarOrArray',
+]
+
+
 T = TypeVar('T')
 U = TypeVar('U')
-ScalarOrArray = Union[T, U, npt.NDArray[U]]
-AngleParam = ScalarOrArray[Angle, float]
+ScalarOrArray: TypeAlias = T | U | npt.NDArray[U]
+AngleParam: TypeAlias = ScalarOrArray[Angle, float]
 
 
+@final
 class Altitude:
     def __init__(self):
         raise NotImplementedError('Use static method Altitude.above.')
 
     @staticmethod
     def above(dec: AngleParam,
               ha: AngleParam,
@@ -54,16 +62,16 @@
             lat: Latitude of site.
 
         Returns:
             tuple of (altitude, azimuth, parallactic), all of which are Angles.
 
         """
 
-        dec = np.asarray(dec.to_value(u.rad).data) * u.rad
-        ha = np.asarray(ha.to_value(u.rad)) * u.rad
+        dec = np.asarray(dec.to_value(u.rad).data) * u.rad  # type: ignore
+        ha = np.asarray(ha.to_value(u.rad)) * u.rad  # type: ignore
         scalar_input = False
         if dec.ndim == 0 and ha.ndim == 0:
             scalar_input = True
         if dec.ndim == 0:
             dec = dec[None]
         if ha.ndim == 0:
             ha = ha[None]
```

### Comparing `lucupy-0.1.9/lucupy/sky/brightness.py` & `lucupy-0.1.90/lucupy/sky/brightness.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 from astropy.units import Quantity
 
 from lucupy.minimodel import SkyBackground
 
 from .constants import EQUAT_RAD, KZEN
 from .utils import xair, ztwilight
 
+__all__ = [
+    'calculate_sky_brightness',
+    'calculate_sky_brightness_qpt',
+    'convert_to_sky_background',
+]
+
 
 def calculate_sky_brightness(moon_phase_angle: Angle,
                              target_moon_angdist: Distance,
                              earth_moon_dist: Distance,
                              moon_zenith_distang: Angle,
                              target_zenith_distang: Angle,
                              sun_zenith_distang: Angle,
@@ -29,15 +35,15 @@
 
     """Calculate sky brightness based on formulas from Krisciunas & Schaefer 1991.
     Uses array processing
 
     Args:
         moon_phase_angle: Moon phase angles in degrees
         target_moon_angdist: Angular distances between target and moon
-        earth_moon_dist: Distances from the Earth to the Moon
+        earth_moon_dist: Distances from the Earth to the Moon in m
         moon_zenith_distang: Moon zenith distance angles
         target_zenith_distang: Target zenith distance angles
         sun_zenith_distang: Sun zenith distance angles
         verbose: Verbose output flag
 
     Returns:
         array of float:  Numpy array of sky background magnitudes at target location
@@ -59,15 +65,15 @@
     n = len(target_zenith_distang)
 
     # Dark sky zenith V surface brightness
     v_zen = np.ones(n) * 21.587
 
     # Correction for twilight
     i = np.where(sun_alt > -18.5 * u.deg)[0][:]
-    if len(i) != 0:
+    if len(i):
         v_zen[i] = v_zen[i] - ztwilight(sun_alt[i])
 
     # zenith sky brightness
     b_zen = 0.263 * a ** (q - v_zen)
 
     # Sky brightness with no moon at target, scattering due to airmass
     b_sky = b_zen * xair(target_zenith_distang) * 10.0 ** (
```

### Comparing `lucupy-0.1.9/lucupy/sky/events.py` & `lucupy-0.1.90/lucupy/sky/events.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,30 +4,34 @@
 #
 # utility and miscellaneous time and the sky routines built mostly on astropy.
 #
 # Copyright John Thorstensen, 2018, who graciously has allowed Gemini to use this code under the BSD-3 Clause license.
 # For license information see LICENSE or https://opensource.org/licenses/BSD-3-Clause
 
 from typing import Tuple
+from zoneinfo import ZoneInfo
 
 import astropy.units as u
 import numpy as np
 from astropy.coordinates import Angle, EarthLocation
 from astropy.time import Time
-from pytz import timezone
 
 from lucupy.types import TimeScalarOrNDArray
 
 from .constants import EQUAT_RAD
 from .moon import Moon
 from .sun import Sun
 from .utils import local_midnight_time
 
+__all__ = [
+    'night_events',
+]
 
-def night_events(time: Time, location: EarthLocation, localtzone: timezone) -> Tuple[Time,
+
+def night_events(time: Time, location: EarthLocation, localtzone: ZoneInfo) -> Tuple[Time,
                                                                                      TimeScalarOrNDArray,
                                                                                      TimeScalarOrNDArray,
                                                                                      TimeScalarOrNDArray,
                                                                                      TimeScalarOrNDArray,
                                                                                      TimeScalarOrNDArray,
                                                                                      TimeScalarOrNDArray]:
     """Compute phenomena for a given night.
```

### Comparing `lucupy-0.1.9/lucupy/sky/moon.py` & `lucupy-0.1.90/lucupy/sky/moon.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,35 @@
 # https://github.com/jrthorstensen/thorsky/blob/master/thorskyutil.py
 #
 # utility and miscellaneous time and the sky routines built mostly on astropy.
 #
 # Copyright John Thorstensen, 2018, who graciously has allowed Gemini to use this code under the BSD-3 Clause license.
 # For license information see LICENSE or https://opensource.org/licenses/BSD-3-Clause
 
-from typing import NoReturn, Optional, Tuple
+from typing import Optional, Tuple, final
 
 import astropy.units as u
 import numpy as np
 from astropy.coordinates import (Angle, Distance, EarthLocation,
                                  GeocentricTrueEcliptic, SkyCoord)
 from astropy.time import Time, TimeDelta
 
 from .altitude import Altitude
-from .constants import EQUAT_RAD, J2000
+from .constants import EQUAT_RAD, J2000, JYEAR, JYEAR_100
 from .utils import (current_geocent_frame, geocentric_coors,
                     hour_angle_to_angle, local_sidereal_time)
 
+__all__ = [
+    'Moon',
+]
 
+
+@final
 class Moon:
-    """Interface for night events for the moon an other calculations.
+    """Interface for night events for the moon on other calculations.
 
     To use this is required to chain the `at` method at the beginning.
     If not unhandled errors would happen.
 
     Attributes:
         time (Time): regular Time in UTC.
         time_jd (Time): Time on Julian day.
@@ -43,15 +48,15 @@
         self.time_jd = None
         self.time_ttjd = None  # important to use correct time argument for this!!
         self.scalar_input = False
         self.pie = None
         self.lambd = None
         self.beta = None
 
-    def at(self, time: Time) -> "Moon":
+    def at(self, time: Time) -> 'Moon':
         """Set time values for other calculations.
 
            This method is meant to be called with:
             - location methods (either low or accurate).
             - time_by_altitude
             - rise_and_set
 
@@ -67,18 +72,18 @@
         self.scalar_input = False
         if self.time_ttjd.ndim == 0:
             self.time_ttjd = self.time_ttjd[None]  # Makes 1D
             self.scalar_input = True
 
         return self
 
-    def _low_precision_calculations(self) -> NoReturn:
+    def _low_precision_calculations(self) -> None:
         """Compute low precision values for the moon location method calculations.
         """
-        t = (self.time_jd - J2000) / 36525.  # jul cent. since J2000.0
+        t = (self.time_jd - J2000) / JYEAR_100  # jul cent. since J2000.0
 
         lambd = (218.32 + 481267.883 * t
                  + 6.29 * np.sin(np.deg2rad(134.9 + 477198.85 * t))
                  - 1.27 * np.sin(np.deg2rad(259.2 - 413335.38 * t))
                  + 0.66 * np.sin(np.deg2rad(235.7 + 890534.23 * t))
                  + 0.21 * np.sin(np.deg2rad(269.9 + 954397.70 * t))
                  - 0.19 * np.sin(np.deg2rad(357.5 + 35999.05 * t))
@@ -93,33 +98,33 @@
 
         pie = (0.9508 + 0.0518 * np.cos(np.deg2rad(134.9 + 477198.85 * t))
                + 0.0095 * np.cos(np.deg2rad(259.2 - 413335.38 * t))
                + 0.0078 * np.cos(np.deg2rad(235.7 + 890534.23 * t))
                + 0.0028 * np.cos(np.deg2rad(269.9 + 954397.70 * t)))
         self.pie = np.deg2rad(pie)
 
-    def _high_precision_calculations(self) -> NoReturn:
+    def _high_precision_calculations(self) -> None:
         """Compute accurate precession values for the moon location method calculations.
         """
-        t = (self.time_ttjd - 2415020.) / 36525.  # this based around 1900 ... */
+        t = (self.time_ttjd - 2415020.) / JYEAR_100  # this based around 1900 ... */
         t_2 = t * t
         t_3 = t_2 * t
         lpr = 270.434164 + 481267.8831 * t - 0.001133 * t_2 + 0.0000019 * t_3
         m = 358.475833 + 35999.0498 * t - 0.000150 * t_2 - 0.0000033 * t_3
         mpr = 296.104608 + 477198.8491 * t + 0.009192 * t_2 + 0.0000144 * t_3
         d = 350.737486 + 445267.1142 * t - 0.001436 * t_2 + 0.0000019 * t_3
         f = 11.250889 + 483202.0251 * t - 0.003211 * t_2 - 0.0000003 * t_3
         om = 259.183275 - 1934.1420 * t + 0.002078 * t_2 + 0.0000022 * t_3
 
-        lpr = lpr % 360.
-        mpr = mpr % 360.
-        m = m % 360.
-        d = d % 360.
-        f = f % 360.
-        om = om % 360.
+        lpr %= 360.
+        mpr %= 360.
+        m %= 360.
+        d %= 360.
+        f %= 360.
+        om %= 360.
 
         sinx = np.sin(np.deg2rad(51.2 + 20.2 * t))
         lpr = lpr + 0.000233 * sinx
         m = m - 0.001778 * sinx
         mpr = mpr + 0.000817 * sinx
         d = d + 0.002011 * sinx
 
@@ -278,24 +283,24 @@
                     + e * e * 0.000026 * np.cos(2 * d - 2 * m)
                     - 0.000023 * np.cos(2 * f - 2 * d + mpr)
                     + e * 0.000019 * np.cos(4 * d - m - mpr))
 
         self.beta = Angle(np.deg2rad(beta), unit=u.rad)
         self.lambd = Angle(np.deg2rad(lambd), unit=u.rad)
 
-    def low_precision_location(self, obs: EarthLocation) -> Tuple[SkyCoord, float]:
+    def low_precision_location(self, obs: EarthLocation) -> Tuple[SkyCoord, Distance]:
         """This is the same as the high precision method, but with a different set of coefficients.
         The difference is small. Good to about 0.1 deg, from the 1992 Astronomical Almanac, p. D46.
-        Note that input time is a float.
+        Note that input time is a float. It also only calculates the sky coordinates.
 
         Args:
             obs: Earth location of the observation.
 
         Returns:
-            Tuple[SkyCoord, float]: Moon coordinates and topographic distance.
+            SkyCoord: Moon coordinates.
         """
         self._low_precision_calculations()
 
         # Terrestrial time with julian day
         sid = local_sidereal_time(self.time, obs)
         lat = obs.lat
         distance = 1. / np.sin(self.pie)
@@ -319,17 +324,18 @@
         n = z / topo_dist
 
         alpha = np.arctan2(m, ell)
         delta = np.arcsin(n)
         distancemultiplier = Distance(EQUAT_RAD, unit=u.m)
 
         fr = current_geocent_frame(self.time)
-        return SkyCoord(alpha, delta, topo_dist * distancemultiplier, frame=fr), topo_dist
+        final_dist = topo_dist * distancemultiplier
+        return SkyCoord(alpha, delta, final_dist, frame=fr), final_dist
 
-    def accurate_location(self, obs: EarthLocation) -> Tuple[SkyCoord, float]:
+    def accurate_location(self, obs: EarthLocation) -> Tuple[SkyCoord, Distance]:
         """Compute topocentric location and distance of moon to better accuracy.
 
         This is good to about 0.01 degrees.
 
         Args:
             obs: location on earth.
 
@@ -339,16 +345,16 @@
         """
         self._high_precision_calculations()
         dist = Distance(1. / np.sin(np.deg2rad(self.pie)) * EQUAT_RAD)
 
         # place these in a skycoord in ecliptic coords of date.  Handle distance
         # separately since it does not transform properly for some reason.
 
-        # eq = 'J{:7.2f}'.format(2000. + (time_ttjd[0] - _Constants.J2000) / 365.25)
-        equinox = f'J{2000. + (self.time_ttjd[0] - J2000) / 365.25:7.2f}'
+        # eq = 'J{:7.2f}'.format(2000. + (time_ttjd[0] - _Constants.J2000) / JYEAR)
+        equinox = f'J{2000. + (self.time_ttjd[0] - J2000) / JYEAR:7.2f}'
         frame = GeocentricTrueEcliptic(equinox=equinox)
         inecl = SkyCoord(lon=Angle(self.lambd, unit=u.rad), lat=Angle(self.beta, unit=u.rad), frame=frame)
 
         # Transform into geocentric equatorial.
         geocen = inecl.transform_to(current_geocent_frame(self.time))
 
         # Do the topo correction yourself. First form xyz coords in equatorial syst of date
@@ -360,41 +366,41 @@
         # equatorial system of date, which one can do simply by replacing the west longitude
         # with the sidereal time
 
         # Exact match with thorskyutil/skycalc with the line below
         xobs, yobs, zobs = geocentric_coors(local_sidereal_time(self.time, obs), obs.lat, obs.height)
 
         # recenter moon's cartesian coordinates on position of obs
-        x = x - xobs
-        y = y - yobs
-        z = z - zobs
+        x -= xobs
+        y -= yobs
+        z -= zobs
 
         # form the toposcentric ra and dec and bundle them into a skycoord of epoch of date.
-        topo_dist = np.sqrt(x ** 2 + y ** 2 + z ** 2)
+        topo_dist = np.sqrt(x * x + y * y + z * z)
         raout = np.arctan2(y, x)
         decout = np.arcsin(z / topo_dist)
 
         if self.scalar_input:
             raout = np.squeeze(raout)
             decout = np.squeeze(decout)
             topo_dist = np.squeeze(topo_dist)
 
-        return SkyCoord(raout, decout, unit=u.rad, frame=current_geocent_frame(self.time)), topo_dist
+        return SkyCoord(raout, decout, unit=u.rad, frame=current_geocent_frame(self.time)), Distance(topo_dist)
 
     @staticmethod
     def time_by_altitude(alt: Angle,
                          time_guess: Time,
                          location: EarthLocation) -> Optional[Time]:
         """Time at which moon passes a given altitude.
 
         This really does have to be iterated since the moon moves fairly
         quickly.
 
         Args:
-            alt: If array, then must be the same length as time_guess desired altitude.
+            alt: If it is an array, then it must be the same length as time_guess desired altitude.
             time_guess : Initial guess; this needs to be fairly close.
             location : EarthLocation
 
         Returns:
             Optional[Time]: a Time, or None if non-convergent.
         """
```

### Comparing `lucupy-0.1.9/lucupy/sky/sun.py` & `lucupy-0.1.90/lucupy/sky/sun.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,34 @@
 # https://github.com/jrthorstensen/thorsky/blob/master/thorskyutil.py
 #
 # utility and miscellaneous time and the sky routines built mostly on astropy.
 #
 # Copyright John Thorstensen, 2018, who graciously has allowed Gemini to use this code under the BSD-3 Clause license.
 # For license information see LICENSE or https://opensource.org/licenses/BSD-3-Clause
 
-from typing import Optional, Tuple
+from typing import Optional, Tuple, final
 
 import astropy.units as u
 import numpy as np
 from astropy.coordinates import Angle, EarthLocation, SkyCoord
 from astropy.time import Time, TimeDelta
 
 from .altitude import Altitude
 from .constants import J2000
 from .utils import (current_geocent_frame, hour_angle_to_angle,
                     local_sidereal_time)
 
+__all__ = [
+    'Sun',
+]
 
+
+@final
 class Sun:
-    """A interface to calculate different night events regarding the Sun.
+    """An interface to calculate different night events regarding the Sun.
 
     To use this is required to chain the `at` method at the beginning.
     If not unhandled errors would happen.
     """
     @staticmethod
     def at(time: Time) -> SkyCoord:
         """Low-precision position of the sun.
@@ -87,48 +92,49 @@
         This uses the low-precision sun location, which is typically good to 0.01 degree.
         That's plenty good enough for computing rise, set, and twilight times.
 
         Args:
             alt: Desired altitude. If array, then must be the same length as time_guess.
             time_guess: Is a Time approximating the answer.
             location: EarthLocation
+            timestep: The timestep to use.
 
         Raises:
             ValueError: Different lengths for Altitude and time_guess
             ArithmeticError: Sunrise, set, or twilight calculation not converging
 
         Returns:
-            Time if convergent None if non-convergent
+            Time if convergent, None if non-convergent
         """
         time_guess = Time(np.asarray(time_guess.jd), format='jd')
         alt = Angle(np.asarray(alt.to_value(u.rad)), unit=u.rad)
         scalar_input = False
         if time_guess.ndim == 0 and alt.ndim == 0:
             scalar_input = True
         if time_guess.ndim == 0:
             time_guess = time_guess[None]  # Makes 1D
         if alt.ndim == 0:
             alt = alt[None]
 
         if len(time_guess) == 1 and len(alt) > 1:
             time_guess = Time(time_guess.jd * np.ones(len(alt)), format='jd')
         elif len(time_guess) > 1 and len(alt) == 1:
-            alt = alt * np.ones(len(time_guess))
+            alt *= np.ones(len(time_guess))
         elif len(time_guess) != len(alt):
             raise ValueError('Error: alt and time_guess have incompatible lengths')
 
         sun_pos = Sun.at(time_guess)
         tolerance = Angle(1.0e-4, unit=u.rad)
 
         delta = TimeDelta(timestep, format='jd')
 
         ha = local_sidereal_time(time_guess, location) - sun_pos.ra
         alt2, az, parang = Altitude.above(sun_pos.dec, Angle(ha, unit=u.hourangle), location.lat)
 
-        time_guess = time_guess + delta
+        time_guess += delta
         sun_pos = Sun.at(time_guess)
 
         alt3, az, parang = Altitude.above(sun_pos.dec,
                                           local_sidereal_time(time_guess, location) - sun_pos.ra,
                                           location.lat)
         err = alt3 - alt
         deriv = (alt3 - alt2) / delta
@@ -138,15 +144,15 @@
         while len(kk) != 0:
             time_guess[kk] = time_guess[kk] - err[kk] / deriv[kk]
             sun_pos = Sun.at(time_guess[kk])
             alt3[kk], az[kk], parang[kk] = Altitude.above(sun_pos.dec,
                                                           local_sidereal_time(time_guess[kk], location) - sun_pos.ra,
                                                           location.lat)
             err[kk] = alt3[kk] - alt[kk]
-            kount[kk] = kount[kk] + 1
+            kount[kk] += 1
             ii = np.where(kount >= 9)[0][:]
             if len(ii) != 0:
                 raise ArithmeticError("Sunrise, set, or twilight calculation not converging.")
             kk = np.where(np.logical_and(abs(err) > tolerance, kount < 10))[0][:]
 
         if scalar_input:
             time_guess = np.squeeze(time_guess)
```

### Comparing `lucupy-0.1.9/lucupy/sky/utils.py` & `lucupy-0.1.90/lucupy/sky/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,39 +5,51 @@
 # utility and miscellaneous time and the sky routines built mostly on astropy.
 #
 # Copyright John Thorstensen, 2018, who graciously has allowed Gemini to use this code under the BSD-3 Clause license.
 # For license information see LICENSE or https://opensource.org/licenses/BSD-3-Clause
 
 from datetime import datetime, timedelta
 from typing import Tuple
+from zoneinfo import ZoneInfo
 
 import astropy.units as u
 import numpy as np
 import numpy.typing as npt
 from astropy.coordinates import (Angle, BaseRADecFrame, EarthLocation,
                                  PrecessedGeocentric)
 from astropy.time import Time
 from astropy.units import Quantity
-from pytz import timezone
 
 from .altitude import AngleParam
-from .constants import EQUAT_RAD, FLATTEN, J2000
+from .constants import EQUAT_RAD, FLATTEN, J2000, JYEAR, JYEAR_100
+
+__all__ = [
+    'current_geocent_frame',
+    'geocentric_coors',
+    'hour_angle_to_angle',
+    'local_midnight_time',
+    'local_sidereal_time',
+    'min_max_alt',
+    'true_airmass',
+    'xair',
+    'ztwilight',
+]
 
 
 def current_geocent_frame(time: Time) -> BaseRADecFrame:
     """Get current frame for the equinox specified by the time.
 
     Args:
         time: If an array then the first entry is used
 
     Returns:
         an astropy PrecessedGeocentric time.
     """
     # Generate a PrecessedGeocentric frame for the current equinox.
-    time_ep = 2000. + (np.asarray(time.jd) - J2000) / 365.25
+    time_ep = 2000. + (np.asarray(time.jd) - J2000) / JYEAR
     if time_ep.ndim == 0:
         time_ep = time_ep[None]  # Makes 1D
     equinox = Time(f'J{time_ep[0]:7.2f}')
 
     return PrecessedGeocentric(equinox=equinox)
 
 
@@ -95,15 +107,15 @@
        minalt, maxalt (Tuple[Angle, Angle]): tuple of minimum and maximum altitudes.
     """
 
     # arguments are Angles; returns (minalt, maxalt) as Angles
     # where min and max are the minimum and maximum altitude
     # an object at declination dec reaches at this latitude.
 
-    dec = np.asarray(dec.to_value(u.rad).data)
+    dec = np.asarray(dec.to_value(u.rad).data)  # type: ignore
     scalar_input = False
     if dec.ndim == 0:
         dec = dec[None]
         scalar_input = True
 
     maxalt = np.zeros(len(dec))
     minalt = np.zeros(len(dec))
@@ -120,15 +132,15 @@
 
     if scalar_input:
         minalt = np.squeeze(minalt)
         maxalt = np.squeeze(maxalt)
     return Angle(minalt, unit=u.rad), Angle(maxalt, unit=u.rad)
 
 
-def local_midnight_time(time: Time, localtzone: timezone) -> Time:
+def local_midnight_time(time: Time, localtzone: ZoneInfo) -> Time:
     """Find nearest local midnight (UT).
 
     If it's before noon local time, returns previous midnight;
     if after noon, return next midnight.
 
     Args:
         time (Time): astropy Time object
@@ -152,15 +164,15 @@
     datetmid = []
     for time in time:
         datet = time.to_datetime(timezone=localtzone)
 
         # if before midnight, add 12 hours
         if datet.hour >= 12:
             datet = datet + timedelta(hours=12.)
-        datetmid.append(localtzone.localize(datetime(datet.year, datet.month, datet.day, 0, 0, 0)))
+        datetmid.append(datetime(datet.year, datet.month, datet.day, 0, 0, 0, tzinfo=localtzone))
 
     if scalar_input:
         result = Time(datetmid[0])
     else:
         result = Time(datetmid)
     return result
 
@@ -192,15 +204,15 @@
     mid = julian_int + 0.5
     ut = fraction - 0.5
     less_than_half = np.where(fraction < 0.5)[0][:]
     if len(less_than_half) != 0:
         mid[less_than_half] = julian_int[less_than_half] - 0.5
         ut[less_than_half] = fraction[less_than_half] + 0.5  # as fraction of a day.
 
-    t = (mid - J2000) / 36525.
+    t = (mid - J2000) / JYEAR_100
 
     sidereal = (24110.54841 + 8640184.812866 * t + 0.093104 * t ** 2 - 6.2e-6 * t ** 3) / 86400.
     # at Greenwich
     sid_int = sidereal.astype(np.int64)
     sidereal = sidereal - sid_int
     # longitude is measured east so add.
     sidereal = sidereal + 1.0027379093 * ut + location.lon.hour / 24.
@@ -254,15 +266,15 @@
     if len(ii) != 0:
         ret[ii] = 1. / np.sin(altit[ii])  # sec z = 1/sin (altit)
 
     kk = np.where(np.logical_and(ret >= 0.0, ret < 12.))[0][:]
     if len(kk) != 0:
         seczmin1 = ret[kk] - 1.
         coefs = np.array([-4.716679E-5, 1.351167E-3, 3.033104E-3, 2.879465E-3, 0.])
-        ret[kk] = ret[kk] - np.polyval(coefs, seczmin1)
+        ret[kk] -= np.polyval(coefs, seczmin1)
 
     if scalar_input:
         return np.squeeze(ret)
     return ret
 
 
 def hour_angle_to_angle(dec: AngleParam,
@@ -288,29 +300,29 @@
 
     """
 
     # Arguments are all angles.
     # returns hour angle at which object at dec is at altitude alt for a
     # latitude lat.
 
-    dec = np.asarray(dec.to_value(u.rad).data) * u.rad
-    alt = np.asarray(alt.to_value(u.rad)) * u.rad
+    dec = np.asarray(dec.to_value(u.rad).data) * u.rad  # type: ignore
+    alt = np.asarray(alt.to_value(u.rad)) * u.rad  # type: ignore
 
     scalar_input = False
     if dec.ndim == 0 and alt.ndim == 0:
         scalar_input = True
     if dec.ndim == 0:
         dec = dec[None]
     if alt.ndim == 0:
         alt = alt[None]
 
     if len(dec) == 1 and len(alt) > 1:
-        dec = dec * np.ones(len(alt))
+        dec *= np.ones(len(alt))
     elif len(dec) > 1 and len(alt) == 1:
-        alt = alt * np.ones(len(dec))
+        alt *= np.ones(len(dec))
     elif len(dec) != len(alt):
         raise ValueError('Error: dec and alt have incompatible lengths')
 
     x = np.zeros(len(dec))
     codec = np.zeros(len(dec))
     zdist = np.zeros(len(dec))
```

### Comparing `lucupy-0.1.9/lucupy/timeutils/__init__.py` & `lucupy-0.1.90/lucupy/timeutils/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,168 +1,167 @@
-# Copyright (c) 2016-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
+# Copyright (c) 2016-2023 Association of Universities for Research in Astronomy, Inc. (AURA)
 # For license information see LICENSE or https://opensource.org/licenses/BSD-3-Clause
 
-import sys
-from datetime import datetime
+from datetime import datetime, timedelta
+from math import ceil
 from typing import Tuple
 
 
+def hms2dec(hours: float, minutes: float, seconds: float, to_degree: bool = False) -> float:
+    """
+    Convert hours, minutes, and seconds to decimal.
+
+    Args:
+        hours (float): the number of hours
+        minutes (float): the number of minutes
+        seconds (float): the number of seconds
+        to_degree (bool, optional): option to convert to degree, with default False
+
+    Returns:
+        float: the decimal equivalent
+    """
+    factor = 15.0 if to_degree else 1.0
+    sign = -1.0 if hours < 0 else 1.0
+    return sign * factor * (abs(hours) + minutes / 60.0 + seconds / 3600.0)
+
+
 def sex2dec(stime: str,
-            todegree: bool = False,
+            to_degree: bool = False,
             sep: str = ':') -> float:
-    """"Sexadecimal to decimal
+    """Sexadecimal to decimal
 
     Args:
-        stime (str): A string of format "HR:MIN:SEC
-        todegree (bool, optional): Option to convert to degree. Defaults to False.
+        stime (str): A string of format "HR:MIN:SEC"
+        to_degree (bool, optional): Option to convert to degree. Defaults to False.
         sep (str, optional): Separator. Defaults to ':'.
 
     Raises:
         ValueError: Wrong format for not following the separator convention.
 
     Returns:
         float: The decimal equivalent
     """
-    l_stime = str(stime).replace("+", "")
-    if sep not in l_stime:
-        raise ValueError(f'Separator {sep} not found in {stime}. Input must be in the format "HR<sep>MIN<sep>SEC"')
-
-    f = 1.0
-    if todegree:
-        f = 15.0
-
-    result = 0.0
-    exp = 0
-    sign = 1.
-    for val in l_stime.split(sep):
-        x = float(val)
-        if x < 0.0:
-            sign = -1.
-        result = result + abs(x) / 60. ** exp
-        exp = exp + 1
-    return sign * f * result
+    try:
+        hours, minutes, seconds = map(float, stime.split(sep))
+        return hms2dec(hours, minutes, seconds, to_degree)
+    except ValueError:
+        raise ValueError(f'Input must be in the format "HR{sep}MIN{sep}SEC"')
 
 
-def dtsex2dec(dt: datetime,
-              todegree: bool = False) -> float:
+def dt2dec(dt: datetime,
+           to_degree: bool = False) -> float:
 
     """Datetime to decimals
 
     Returns:
         float: The decimal equivalent
     """
-    f = 1.0
-    if todegree:
-        f = 15.0
-
-    sign = 1.
-    if dt.hour < 0:
-        sign = -1.
-    return sign * f * (abs(dt.hour) + dt.minute / 60. + dt.second / 3600.)
+    return hms2dec(dt.hour, dt.minute, dt.second, to_degree)
 
 
-def sixty(dd: float) -> Tuple[int, int, int]:
-    """Sixty
+def days2dms(days: float) -> Tuple[float, float, float]:
+    """Convert days into degrees, minutes, and seconds of arc.
 
     Args:
-        dd (float): Days
+        days (float): Days
 
     Returns:
-        Tuple[int, int, int]: Degrees, minutes and seconds
+        Tuple[float, float, float]: Degrees, minutes, and seconds
     """
-    is_positive = dd >= 0
-    l_dd = abs(dd)
-    minutes, seconds = divmod(l_dd * 3600, 60)
-    degrees, minutes = divmod(minutes, 60)
-    if degrees > 0.:
-        degrees = degrees if is_positive else -degrees
-    elif minutes > 0.:
-        minutes = minutes if is_positive else -minutes
-    else:
-        seconds = seconds if is_positive else -seconds
-    return degrees, minutes, seconds
-
-
-def dec2sex(d: float,
-            p: int = 3,
-            cutsec: bool = False,
-            hour: bool = False,
-            tohour: bool = False,
-            sep: str = ':',
-            leadzero: int = 0,
-            round_min: bool = False) -> str:
+    is_positive = days >= 0
+    l_dd = abs(days)
+    total_seconds = l_dd * 3600.0
+    degrees, remainder = divmod(total_seconds, 3600)
+    minutes, seconds = divmod(remainder, 60)
+    return (degrees if is_positive else -degrees,
+            minutes if is_positive else -minutes,
+            seconds if is_positive else -seconds)
+
+
+def dec2sex(
+    degrees: float,
+    precision: int = 3,
+    cut_seconds: bool = False,
+    input_is_hours: bool = False,
+    to_hours: bool = False,
+    separator: str = ':',
+    leading_zeros: int = 0,
+    round_minutes: bool = False,
+) -> str:
     """Convert decimal degrees/hours to a formatted sexigesimal string.
 
     Args:
-        d: Input in degrees
-        p: Digits for seconds
-        cutsec: Cut seconds, just display, e.g. DD:MM
-        hour: d is decimal hours, so must be <=24
-        tohour: Convert from degress to hours (divide by 15.)
-        sep: Separator string
-        leadzero: If >0 display leading 0's, e.g. -05:25. The value is the number of digits for the DD or HR field.
-        round_min: When cutsec, round to the nearest minute rather than truncate
-    Returns:
-        str: That modify string
-    """
-    l_d = float(d)
-    sign = ''
-    maxdg = 360.
-
-    if tohour:
-        l_d = l_d / 15.0
-        hour = True
-
-    if hour and (abs(l_d) > 24.):
-        print('Input in hours must be less than or equal to 24.0.')
-        sys.exit(1)
-
-    if hour:
-        maxdg = 24.0
-
-    n = 2 if p == 0 else 3
-    secstr = '{:0' + '{:1d}'.format(n + p) + '.' + '{:1d}'.format(p) + 'f}'
-
-    six = sixty(l_d)
-
-    dg = abs(int(six[0]))
-    if six[0] < 0:
-        sign = '-'
-
-    if leadzero > 0:
-        sldg = '0' + str(leadzero)
-    else:
-        sldg = str(len(str(dg)))
-
-    mn = abs(int(six[1]))
-    if six[1] < 0:
-        sign = '-'
-
-    sc = float(secstr.format(abs(six[2])))
-    if six[2] < 0.0:
-        sign = '-'
-
-    if sc >= 60.0:
-        sc -= 60.0
-        mn = mn + 1
-
-    if cutsec:
-        if round_min and sc >= 30.:
-            # Round to the nearest minute, otherwise truncate
-            mn += 1
-        sc = 0.0
-
-    if mn >= 60:
-        mn -= 60
-        dg = dg + 1
-
-    if dg >= int(maxdg):
-        dg = dg - int(maxdg)
-
-    if cutsec and sc == 0.0:
-        fmt = '{:1s}{:' + sldg + 'd}' + sep + '{:02d}'
-        s = fmt.format(sign, dg, mn)
-    else:
-        fmt = '{:1s}{:' + sldg + 'd}' + sep + '{:02d}' + sep + secstr
-        s = fmt.format(sign, dg, mn, sc)
+        degrees (float): Input in degrees
+        precision (int, optional): Digits for seconds. Defaults to 3.
+        cut_seconds (bool, optional): Cut seconds, just display, e.g. DD:MM. Defaults to False.
+        input_is_hours (bool, optional): If True, input is in decimal hours, must be <=24. Defaults to False.
+        to_hours (bool, optional): Convert from degrees to hours (divide by 15.). Defaults to False.
+        separator (str, optional): Separator string. Defaults to ':'.
+        leading_zeros (int, optional): If > 0, display leading 0's. Defaults to 0.
+        round_minutes (bool, optional): When cut_seconds, round to the nearest minute rather than truncate.
+            Defaults to False.
+
+    Returns:
+        str: The modified string
+    """
+    if to_hours:
+        degrees /= 15.0
+        input_is_hours = True
+
+    if input_is_hours and abs(degrees) > 24.0:
+        raise ValueError(f'Input in hours must be less than or equal to 24: {abs(degrees)}')
+
+    max_degrees = 360.0 if not input_is_hours else 24.0
+
+    # Determine the number of decimal places for seconds
+    seconds_format = f'{{:0.{precision}f}}'
+
+    # Convert the degrees to degrees, minutes, and seconds
+    degrees, minutes, seconds = days2dms(degrees if not input_is_hours else degrees * 15)
+
+    # Handle negative values
+    sign = '-' if degrees < 0 else ''
+    degrees = abs(int(degrees))
+    minutes = abs(int(minutes))
+    seconds = float(seconds_format.format(abs(seconds)))
+
+    # Handle rounding or truncating seconds
+    if cut_seconds:
+        if round_minutes and seconds >= 30.0:
+            minutes += 1
+        seconds = 0.0
+
+    # Handle minutes and hours overflow
+    if minutes >= 60:
+        minutes -= 60
+        degrees += 1
+
+    if degrees >= max_degrees:
+        degrees -= max_degrees
+
+    # Format the result string
+    degrees_format = f'{{:0{leading_zeros}d}}'
+    result_format = f'{sign}{degrees_format}{separator}{minutes:02d}'
+
+    if not cut_seconds or seconds != 0.0:
+        result_format += f'{separator}{seconds}'
+
+    return result_format
+
+
+def time2slots(time_slot_length: timedelta, time_quantity: timedelta) -> int:
+    """
+    Convert time_quantity into the number of time slots given the time slot length.
+    This takes the ceil, so it ensures that the time_quantity supplied fits into
+    the number of time slots returned.
+
+    Notes:
+        The units in the actual time_quantities are unimportant: the return type is without unit.
+
+    Args:
+        time_slot_length: the length of a time slot as a timedelta
+        time_quantity: the amount of time as a timedelta that we want to know in terms of time slots
 
-    return s.strip()
+    Returns:
+        the ceiling of the number of time slots required to accommodate the time quantity (unitless)
+    """
+    return ceil(time_quantity / time_slot_length)
```

### Comparing `lucupy-0.1.9/pyproject.toml` & `lucupy-0.1.90/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [tool.poetry]
 name = "lucupy"
-version = "0.1.9"
+version = "0.1.90"
 description = "Lucuma core package for the Gemini Automated Scheduler at: https://github.com/gemini-hlsw/scheduler"
-authors = ["Sergio Troncoso <sergio.troncoso@noirlab.edu>",
-           "Sebastian Raaphorst <sebastian.raaphorst@noirlab.edu>",
-           "Bryan Miller <bryan.miller@noirlab.edu"]
+authors = [
+    "Sebastian Raaphorst <sebastian.raaphorst@noirlab.edu>",
+    "Sergio Troncoso <sergio.troncoso@noirlab.edu>",
+    "Bryan Miller <bryan.miller@noirlab.edu>"
+]
 readme = "README.rst"
 homepage = "https://github.com/gemini-hlsw/lucupy"
 repository = "https://github.com/gemini-hlsw/lucupy"
 keywords = ["lucuma", "scheudule", "gpp"]
 classifiers = [
    "Environment :: Web Environment",
    "Framework :: Hypothesis",
@@ -33,15 +35,16 @@
 mkdocs-section-index = "^0.3.4"
 mkdocstrings = {extras = ["python"], version = "^0.19.0"}
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 astropy = "^5.1"
-pytz = "^2022.2"
+gelidum = "^0.5.8"
+matplotlib = "^3.7.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 hypothesis = "6.54.2"
 pre-commit = "^2.20.0"
 pytest-xdist = "^2.5.0"
```

### Comparing `lucupy-0.1.9/PKG-INFO` & `lucupy-0.1.90/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: lucupy
-Version: 0.1.9
+Version: 0.1.90
 Summary: Lucuma core package for the Gemini Automated Scheduler at: https://github.com/gemini-hlsw/scheduler
 Home-page: https://github.com/gemini-hlsw/lucupy
 Keywords: lucuma,scheudule,gpp
-Author: Sergio Troncoso
-Author-email: sergio.troncoso@noirlab.edu
+Author: Sebastian Raaphorst
+Author-email: sebastian.raaphorst@noirlab.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Hypothesis
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Utilities
 Requires-Dist: astropy (>=5.1,<6.0)
-Requires-Dist: pytz (>=2022.2,<2023.0)
+Requires-Dist: gelidum (>=0.5.8,<0.6.0)
+Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Project-URL: Repository, https://github.com/gemini-hlsw/lucupy
 Description-Content-Type: text/x-rst
 
 Lucupy
 #########
 
 This package contains data structures and functions to support all the microservices that make up the Schedule app
```


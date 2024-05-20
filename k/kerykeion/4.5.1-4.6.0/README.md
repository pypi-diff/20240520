# Comparing `tmp/kerykeion-4.5.1.tar.gz` & `tmp/kerykeion-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerykeion-4.5.1.tar", max compression
+gzip compressed data, was "kerykeion-4.6.0.tar", max compression
```

## Comparing `kerykeion-4.5.1.tar` & `kerykeion-4.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    34273 2024-03-05 19:55:06.854597 kerykeion-4.5.1/LICENSE
--rw-r--r--   0        0        0     8634 2024-03-05 19:55:06.855014 kerykeion-4.5.1/README.md
--rw-r--r--   0        0        0     3917 2024-05-13 20:03:16.435516 kerykeion-4.5.1/kerykeion/__init__.py
--rw-r--r--   0        0        0      293 2024-03-05 19:18:31.414757 kerykeion-4.5.1/kerykeion/aspects/__init__.py
--rw-r--r--   0        0        0     5832 2024-03-05 19:18:31.414940 kerykeion-4.5.1/kerykeion/aspects/aspects_utils.py
--rw-r--r--   0        0        0     4507 2024-03-05 19:18:31.415083 kerykeion-4.5.1/kerykeion/aspects/natal_aspects.py
--rw-r--r--   0        0        0     3993 2024-03-05 19:18:31.415179 kerykeion-4.5.1/kerykeion/aspects/synastry_aspects.py
--rw-r--r--   0        0        0    25678 2024-05-16 19:08:55.018893 kerykeion-4.5.1/kerykeion/astrological_subject.py
--rw-r--r--   0        0        0      127 2024-03-05 19:18:31.415447 kerykeion-4.5.1/kerykeion/charts/__init__.py
--rw-r--r--   0        0        0     3197 2024-03-05 19:18:31.415523 kerykeion-4.5.1/kerykeion/charts/charts_utils.py
--rwxr-xr-x   0        0        0    65295 2024-03-19 11:01:58.830365 kerykeion-4.5.1/kerykeion/charts/kerykeion_chart_svg.py
--rwxr-xr-x   0        0        0    69874 2024-03-05 19:18:31.416341 kerykeion-4.5.1/kerykeion/charts/templates/chart.xml
--rw-r--r--   0        0        0      965 2024-05-13 20:03:16.436187 kerykeion-4.5.1/kerykeion/enums.py
--rw-r--r--   0        0        0     4444 2024-03-05 19:18:31.416503 kerykeion-4.5.1/kerykeion/fetch_geonames.py
--rw-r--r--   0        0        0      205 2024-03-05 19:18:31.416620 kerykeion-4.5.1/kerykeion/kr_types/__init__.py
--rw-r--r--   0        0        0     1945 2024-03-05 19:18:31.416709 kerykeion-4.5.1/kerykeion/kr_types/chart_types.py
--rw-r--r--   0        0        0      314 2024-03-05 19:18:31.416783 kerykeion-4.5.1/kerykeion/kr_types/kerykeion_exception.py
--rw-r--r--   0        0        0     1034 2024-03-05 19:18:31.416860 kerykeion-4.5.1/kerykeion/kr_types/kr_literals.py
--rw-r--r--   0        0        0     4106 2024-05-16 19:08:55.019127 kerykeion-4.5.1/kerykeion/kr_types/kr_models.py
--rw-r--r--   0        0        0    12737 2024-03-05 19:18:31.417044 kerykeion-4.5.1/kerykeion/kr_types/settings_models.py
--rw-r--r--   0        0        0     6794 2024-03-05 19:18:31.417198 kerykeion-4.5.1/kerykeion/relationship_score.py
--rw-r--r--   0        0        0     2565 2024-03-05 19:18:31.417278 kerykeion-4.5.1/kerykeion/report.py
--rw-r--r--   0        0        0       69 2024-03-05 19:18:31.417375 kerykeion-4.5.1/kerykeion/settings/__init__.py
--rw-r--r--   0        0        0     2341 2024-03-05 19:18:31.417455 kerykeion-4.5.1/kerykeion/settings/kerykeion_settings.py
--rw-r--r--   0        0        0    12282 2024-03-05 19:18:31.417645 kerykeion-4.5.1/kerykeion/settings/kr.config.json
--rw-r--r--   0        0        0       73 2024-03-05 19:18:31.417768 kerykeion-4.5.1/kerykeion/sweph/README.md
--rw-r--r--   0        0        0   223002 2024-03-05 19:18:31.418653 kerykeion-4.5.1/kerykeion/sweph/seas_18.se1
--rw-r--r--   0        0        0     6207 2024-05-13 20:03:16.436971 kerykeion-4.5.1/kerykeion/utilities.py
--rw-r--r--   0        0        0     2354 2024-05-16 19:08:55.019261 kerykeion-4.5.1/pyproject.toml
--rw-r--r--   0        0        0    10311 1970-01-01 00:00:00.000000 kerykeion-4.5.1/PKG-INFO
+-rw-r--r--   0        0        0    34273 2024-03-05 19:55:06.854597 kerykeion-4.6.0/LICENSE
+-rw-r--r--   0        0        0     8634 2024-03-05 19:55:06.855014 kerykeion-4.6.0/README.md
+-rw-r--r--   0        0        0     3917 2024-05-20 21:44:34.775470 kerykeion-4.6.0/kerykeion/__init__.py
+-rw-r--r--   0        0        0      293 2024-05-20 21:44:34.775703 kerykeion-4.6.0/kerykeion/aspects/__init__.py
+-rw-r--r--   0        0        0     5832 2024-05-20 21:44:34.775937 kerykeion-4.6.0/kerykeion/aspects/aspects_utils.py
+-rw-r--r--   0        0        0     4507 2024-05-20 21:44:34.776153 kerykeion-4.6.0/kerykeion/aspects/natal_aspects.py
+-rw-r--r--   0        0        0     3993 2024-05-20 21:44:34.776366 kerykeion-4.6.0/kerykeion/aspects/synastry_aspects.py
+-rw-r--r--   0        0        0    22965 2024-05-20 21:44:34.776635 kerykeion-4.6.0/kerykeion/astrological_subject.py
+-rw-r--r--   0        0        0      127 2024-05-20 21:44:34.776876 kerykeion-4.6.0/kerykeion/charts/__init__.py
+-rw-r--r--   0        0        0     3197 2024-03-05 19:18:31.415523 kerykeion-4.6.0/kerykeion/charts/charts_utils.py
+-rwxr-xr-x   0        0        0    65295 2024-05-20 21:44:34.777228 kerykeion-4.6.0/kerykeion/charts/kerykeion_chart_svg.py
+-rwxr-xr-x   0        0        0    69874 2024-03-05 19:18:31.416341 kerykeion-4.6.0/kerykeion/charts/templates/chart.xml
+-rw-r--r--   0        0        0      965 2024-05-13 20:03:16.436187 kerykeion-4.6.0/kerykeion/enums.py
+-rw-r--r--   0        0        0     4444 2024-05-20 21:44:34.777442 kerykeion-4.6.0/kerykeion/fetch_geonames.py
+-rw-r--r--   0        0        0      295 2024-05-20 21:44:34.777647 kerykeion-4.6.0/kerykeion/kr_types/__init__.py
+-rw-r--r--   0        0        0     1945 2024-03-05 19:18:31.416709 kerykeion-4.6.0/kerykeion/kr_types/chart_types.py
+-rw-r--r--   0        0        0      314 2024-05-20 21:44:34.777837 kerykeion-4.6.0/kerykeion/kr_types/kerykeion_exception.py
+-rw-r--r--   0        0        0     1267 2024-05-20 21:44:34.778024 kerykeion-4.6.0/kerykeion/kr_types/kr_literals.py
+-rw-r--r--   0        0        0     4260 2024-05-20 21:44:34.778212 kerykeion-4.6.0/kerykeion/kr_types/kr_models.py
+-rw-r--r--   0        0        0    12743 2024-05-20 21:44:34.778431 kerykeion-4.6.0/kerykeion/kr_types/settings_models.py
+-rw-r--r--   0        0        0     6794 2024-05-20 21:44:34.778633 kerykeion-4.6.0/kerykeion/relationship_score.py
+-rw-r--r--   0        0        0     2565 2024-03-05 19:18:31.417278 kerykeion-4.6.0/kerykeion/report.py
+-rw-r--r--   0        0        0       69 2024-03-05 19:18:31.417375 kerykeion-4.6.0/kerykeion/settings/__init__.py
+-rw-r--r--   0        0        0     2347 2024-05-20 21:44:34.778844 kerykeion-4.6.0/kerykeion/settings/kerykeion_settings.py
+-rw-r--r--   0        0        0    12282 2024-03-05 19:18:31.417645 kerykeion-4.6.0/kerykeion/settings/kr.config.json
+-rw-r--r--   0        0        0       73 2024-03-05 19:18:31.417768 kerykeion-4.6.0/kerykeion/sweph/README.md
+-rw-r--r--   0        0        0   223002 2024-03-05 19:18:31.418653 kerykeion-4.6.0/kerykeion/sweph/seas_18.se1
+-rw-r--r--   0        0        0    10822 2024-05-20 21:44:34.779112 kerykeion-4.6.0/kerykeion/utilities.py
+-rw-r--r--   0        0        0     2354 2024-05-20 21:46:45.144735 kerykeion-4.6.0/pyproject.toml
+-rw-r--r--   0        0        0    10311 1970-01-01 00:00:00.000000 kerykeion-4.6.0/PKG-INFO
```

### Comparing `kerykeion-4.5.1/LICENSE` & `kerykeion-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.1/README.md` & `kerykeion-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.1/kerykeion/__init__.py` & `kerykeion-4.6.0/kerykeion/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    This is part of Kerykeion (C) 2023 Giacomo Battaglia
+    This is part of Kerykeion (C) 2024 Giacomo Battaglia
 
     Kerykeion is a python library for Astrology.
     It can calculate all the planet and house position,
     also it can calculate the aspects of a single persone or between two, you can set how many planets you
     need in the settings in the utility module.
     It also can generate an SVG of a birthchart, a synastry chart or a transit chart.
```

### Comparing `kerykeion-4.5.1/kerykeion/aspects/aspects_utils.py` & `kerykeion-4.6.0/kerykeion/aspects/aspects_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    This is part of Kerykeion (C) 2023 Giacomo Battaglia
+    This is part of Kerykeion (C) 2024 Giacomo Battaglia
 """
 # TODO: Better documentation and unit tests
 
 from kerykeion import AstrologicalSubject
 from kerykeion.settings import KerykeionSettingsModel
 from swisseph import difdeg2n
 from typing import Union
```

### Comparing `kerykeion-4.5.1/kerykeion/aspects/natal_aspects.py` & `kerykeion-4.6.0/kerykeion/aspects/natal_aspects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    This is part of Kerykeion (C) 2023 Giacomo Battaglia
+    This is part of Kerykeion (C) 2024 Giacomo Battaglia
 """
 
 from pathlib import Path
 from kerykeion import AstrologicalSubject
 import logging
 from typing import Union
 from kerykeion.settings.kerykeion_settings import get_settings
```

### Comparing `kerykeion-4.5.1/kerykeion/aspects/synastry_aspects.py` & `kerykeion-4.6.0/kerykeion/aspects/synastry_aspects.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    This is part of Kerykeion (C) 2023 Giacomo Battaglia
+    This is part of Kerykeion (C) 2024 Giacomo Battaglia
 """
 
 from kerykeion import AstrologicalSubject
 from pathlib import Path
 from typing import Union
 from functools import cached_property
```

### Comparing `kerykeion-4.5.1/kerykeion/astrological_subject.py` & `kerykeion-4.6.0/kerykeion/astrological_subject.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 # -*- coding: utf-8 -*-
 """
-    This is part of Kerykeion (C) 2023 Giacomo Battaglia
+    This is part of Kerykeion (C) 2024 Giacomo Battaglia
 """
 
-import math
 import pytz
 import swisseph as swe
 import logging
 
 from datetime import datetime
 from kerykeion.fetch_geonames import FetchGeonames
 from kerykeion.kr_types import (
     KerykeionException,
     ZodiacType,
     AstrologicalSubjectModel,
     LunarPhaseModel,
     KerykeionPointModel,
 )
-from kerykeion.utilities import get_number_from_name, calculate_position
+from kerykeion.utilities import (
+    get_number_from_name, 
+    calculate_position, 
+    get_planet_house,
+    get_moon_emoji_from_phase_int,
+    get_moon_phase_name_from_phase_int,
+)
 from pathlib import Path
 from typing import Union, Literal
 
 DEFAULT_GEONAMES_USERNAME = "century.boy"
 
 
 class AstrologicalSubject:
@@ -427,72 +432,29 @@
         else:
             self.chiron = None
 
     def _planets_in_houses(self) -> None:
         """Calculates the house of the planet and updates
         the planets dictionary."""
 
-        def for_every_planet(planet, planet_deg):
-            """Function to do the calculation.
-            Args: planet dictionary, planet degree"""
-
-            def point_between(p1, p2, p3):
-                """Finds if a point is between two other in a circle
-                args: first point, second point, point in the middle"""
-                p1_p2 = math.fmod(p2 - p1 + 360, 360)
-                p1_p3 = math.fmod(p3 - p1 + 360, 360)
-                if (p1_p2 <= 180) != (p1_p3 > p1_p2):
-                    return True
-                else:
-                    return False
-
-            if point_between(self.houses_degree_ut[0], self.houses_degree_ut[1], planet_deg) == True:
-                planet["house"] = "First_House"
-            elif point_between(self.houses_degree_ut[1], self.houses_degree_ut[2], planet_deg) == True:
-                planet["house"] = "Second_House"
-            elif point_between(self.houses_degree_ut[2], self.houses_degree_ut[3], planet_deg) == True:
-                planet["house"] = "Third_House"
-            elif point_between(self.houses_degree_ut[3], self.houses_degree_ut[4], planet_deg) == True:
-                planet["house"] = "Fourth_House"
-            elif point_between(self.houses_degree_ut[4], self.houses_degree_ut[5], planet_deg) == True:
-                planet["house"] = "Fifth_House"
-            elif point_between(self.houses_degree_ut[5], self.houses_degree_ut[6], planet_deg) == True:
-                planet["house"] = "Sixth_House"
-            elif point_between(self.houses_degree_ut[6], self.houses_degree_ut[7], planet_deg) == True:
-                planet["house"] = "Seventh_House"
-            elif point_between(self.houses_degree_ut[7], self.houses_degree_ut[8], planet_deg) == True:
-                planet["house"] = "Eighth_House"
-            elif point_between(self.houses_degree_ut[8], self.houses_degree_ut[9], planet_deg) == True:
-                planet["house"] = "Ninth_House"
-            elif point_between(self.houses_degree_ut[9], self.houses_degree_ut[10], planet_deg) == True:
-                planet["house"] = "Tenth_House"
-            elif point_between(self.houses_degree_ut[10], self.houses_degree_ut[11], planet_deg) == True:
-                planet["house"] = "Eleventh_House"
-            elif point_between(self.houses_degree_ut[11], self.houses_degree_ut[0], planet_deg) == True:
-                planet["house"] = "Twelfth_House"
-            else:
-                planet["house"] = "error!"
-
-            return planet
-
-        self.sun = for_every_planet(self.sun, self.planets_degrees_ut[0])
-        self.moon = for_every_planet(self.moon, self.planets_degrees_ut[1])
-        self.mercury = for_every_planet(self.mercury, self.planets_degrees_ut[2])
-        self.venus = for_every_planet(self.venus, self.planets_degrees_ut[3])
-        self.mars = for_every_planet(self.mars, self.planets_degrees_ut[4])
-        self.jupiter = for_every_planet(self.jupiter, self.planets_degrees_ut[5])
-        self.saturn = for_every_planet(self.saturn, self.planets_degrees_ut[6])
-        self.uranus = for_every_planet(self.uranus, self.planets_degrees_ut[7])
-        self.neptune = for_every_planet(self.neptune, self.planets_degrees_ut[8])
-        self.pluto = for_every_planet(self.pluto, self.planets_degrees_ut[9])
-        self.mean_node = for_every_planet(self.mean_node, self.planets_degrees_ut[10])
-        self.true_node = for_every_planet(self.true_node, self.planets_degrees_ut[11])
+        self.sun.house = get_planet_house(self.planets_degrees_ut[0], self.houses_degree_ut)
+        self.moon.house = get_planet_house(self.planets_degrees_ut[1], self.houses_degree_ut)
+        self.mercury.house = get_planet_house(self.planets_degrees_ut[2], self.houses_degree_ut)
+        self.venus.house = get_planet_house(self.planets_degrees_ut[3], self.houses_degree_ut)
+        self.mars.house = get_planet_house(self.planets_degrees_ut[4], self.houses_degree_ut)
+        self.jupiter.house = get_planet_house(self.planets_degrees_ut[5], self.houses_degree_ut)
+        self.saturn.house = get_planet_house(self.planets_degrees_ut[6], self.houses_degree_ut)
+        self.uranus.house = get_planet_house(self.planets_degrees_ut[7], self.houses_degree_ut)
+        self.neptune.house = get_planet_house(self.planets_degrees_ut[8], self.houses_degree_ut)
+        self.pluto.house = get_planet_house(self.planets_degrees_ut[9], self.houses_degree_ut)
+        self.mean_node.house = get_planet_house(self.planets_degrees_ut[10], self.houses_degree_ut)
+        self.true_node.house = get_planet_house(self.planets_degrees_ut[11], self.houses_degree_ut)
 
         if not self.disable_chiron:
-            self.chiron = for_every_planet(self.chiron, self.planets_degrees_ut[12])
+            self.chiron.house = get_planet_house(self.planets_degrees_ut[12], self.houses_degree_ut)
         else:
             self.chiron = None
 
         self.planets_list = [
             self.sun,
             self.moon,
             self.mercury,
@@ -579,41 +541,20 @@
             if x == 27:
                 high = 360
             else:
                 high = sunstep[x + 1]
             if degrees_between >= low and degrees_between < high:
                 sun_phase = x + 1
 
-        def moon_emoji(phase):
-            if phase == 1:
-                result = "🌑"
-            elif phase < 7:
-                result = "🌒"
-            elif 7 <= phase <= 9:
-                result = "🌓"
-            elif phase < 14:
-                result = "🌔"
-            elif phase == 14:
-                result = "🌕"
-            elif phase < 20:
-                result = "🌖"
-            elif 20 <= phase <= 22:
-                result = "🌗"
-            elif phase <= 28:
-                result = "🌘"
-            else:
-                result = phase
-
-            return result
-
         lunar_phase_dictionary = {
             "degrees_between_s_m": degrees_between,
             "moon_phase": moon_phase,
             "sun_phase": sun_phase,
-            "moon_emoji": moon_emoji(moon_phase),
+            "moon_emoji": get_moon_emoji_from_phase_int(moon_phase),
+            "moon_phase_name": get_moon_phase_name_from_phase_int(moon_phase)
         }
 
         self.lunar_phase = LunarPhaseModel(**lunar_phase_dictionary)
 
     def _check_if_poles(self):
         """
             Utility function to check if the location is in the polar circle.
```

### Comparing `kerykeion-4.5.1/kerykeion/charts/charts_utils.py` & `kerykeion-4.6.0/kerykeion/charts/charts_utils.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.1/kerykeion/charts/kerykeion_chart_svg.py` & `kerykeion-4.6.0/kerykeion/charts/kerykeion_chart_svg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    This is part of Kerykeion (C) 2023 Giacomo Battaglia
+    This is part of Kerykeion (C) 2024 Giacomo Battaglia
 """
 
 
 import pytz
 import logging
 
 from datetime import datetime
```

### Comparing `kerykeion-4.5.1/kerykeion/charts/templates/chart.xml` & `kerykeion-4.6.0/kerykeion/charts/templates/chart.xml`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.1/kerykeion/enums.py` & `kerykeion-4.6.0/kerykeion/enums.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.1/kerykeion/fetch_geonames.py` & `kerykeion-4.6.0/kerykeion/fetch_geonames.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    This is part of Kerykeion (C) 2023 Giacomo Battaglia
+    This is part of Kerykeion (C) 2024 Giacomo Battaglia
 """
 
 
 import logging
 from requests import Request
 from requests_cache import CachedSession
 from typing import Union
```

### Comparing `kerykeion-4.5.1/kerykeion/kr_types/chart_types.py` & `kerykeion-4.6.0/kerykeion/kr_types/chart_types.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.1/kerykeion/kr_types/kr_literals.py` & `kerykeion-4.6.0/kerykeion/kr_types/kr_literals.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    This is part of Kerykeion (C) 2023 Giacomo Battaglia
+    This is part of Kerykeion (C) 2024 Giacomo Battaglia
 """
 
 
 from typing import Literal
 
 # Zodiac Types:
 ZodiacType = Literal["Tropic", "Sidereal"]
@@ -52,7 +52,17 @@
     "Fixed",
     "Mutable",
 ]
 
 ChartType = Literal["Natal", "ExternalNatal", "Synastry", "Transit"]
 
 LunarPhaseEmoji = Literal["🌑", "🌒", "🌓", "🌔", "🌕", "🌖", "🌗", "🌘"]
+LunarPhaseName = Literal[
+        "New Moon", 
+        "Waxing Crescent", 
+        "First Quarter", 
+        "Waxing Gibbous", 
+        "Full Moon", 
+        "Waning Gibbous", 
+        "Last Quarter", 
+        "Waning Crescent"
+    ]
```

### Comparing `kerykeion-4.5.1/kerykeion/kr_types/kr_models.py` & `kerykeion-4.6.0/kerykeion/kr_types/kr_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # -*- coding: utf-8 -*-
 """
-    This is part of Kerykeion (C) 2023 Giacomo Battaglia
+    This is part of Kerykeion (C) 2024 Giacomo Battaglia
 """
 
 
 from typing import Literal, Union, Optional
 from pydantic import BaseModel
 
-from .kr_literals import *
+from kerykeion.kr_types import LunarPhaseEmoji, LunarPhaseName, Planet, Houses, Quality, Element, Sign, ZodiacType
 
 
 class LunarPhaseModel(BaseModel):
     degrees_between_s_m: Union[float, int]
     moon_phase: int
     sun_phase: int
     moon_emoji: LunarPhaseEmoji
+    moon_phase_name: LunarPhaseName
 
     def __str__(self):
         return (
             super()
-            .dict(
+            .model_dump(
                 exclude_none=True,
                 exclude_unset=True,
                 exclude_defaults=True,
                 by_alias=False,
             )
             .__str__()
         )
@@ -69,27 +70,27 @@
     point_type: Literal["Planet", "House"]
     house: Optional[Literal[1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]] = None
     retrograde: Optional[bool] = None
 
     def __str__(self):
         return (
             super()
-            .dict(
+            .model_dump(
                 exclude_none=True,
                 exclude_unset=True,
                 exclude_defaults=True,
                 by_alias=False,
             )
             .__str__()
         )
 
     def __repr__(self):
         return (
             super()
-            .dict(
+            .model_dump(
                 exclude_none=True,
                 exclude_unset=True,
                 exclude_defaults=True,
                 by_alias=False,
             )
             .__str__()
         )
@@ -158,23 +159,24 @@
 
     # Lunar Phase
     lunar_phase: LunarPhaseModel
 
 
 if __name__ == "__main__":
     from kerykeion.utilities import setup_logging
+
     setup_logging(level="debug")
 
     sun = KerykeionPointModel(
         name="Sun",
         element="Air",
         quality="Fixed",
         sign="Aqu",
         sign_num=1,
         position=0,
         abs_pos=12.123123,
         emoji="♈",
         point_type="Planet",
     )
 
-    print(sun.json())
+    print(sun.model_dump_json())
     print(sun)
```

### Comparing `kerykeion-4.5.1/kerykeion/kr_types/settings_models.py` & `kerykeion-4.6.0/kerykeion/kr_types/settings_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    This is part of Kerykeion (C) 2023 Giacomo Battaglia
+    This is part of Kerykeion (C) 2024 Giacomo Battaglia
 """
 
 
 from json import load
 from pydantic import BaseModel, Field
 from pathlib import Path
 from typing import Dict, List, Union
@@ -18,15 +18,15 @@
     def __init__(self, **data):
         super().__init__(**data)
 
     def __getitem__(self, item):
         return getattr(self, item)
     
     def __str__(self) -> str:
-        return str(self.dict())
+        return str(self.model_dump())
 
     def get(self, item, default=None):
         return getattr(self, item, default)
 
 
 class KerykeionSettingsCelestialPointModel(CustomBaseModel):
     """
```

### Comparing `kerykeion-4.5.1/kerykeion/relationship_score.py` & `kerykeion-4.6.0/kerykeion/relationship_score.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    This is part of Kerykeion (C) 2023 Giacomo Battaglia
+    This is part of Kerykeion (C) 2024 Giacomo Battaglia
 """
 
 from kerykeion import AstrologicalSubject
 from kerykeion.aspects.synastry_aspects import SynastryAspects
 import logging
 from pathlib import Path
 from typing import Union
```

### Comparing `kerykeion-4.5.1/kerykeion/report.py` & `kerykeion-4.6.0/kerykeion/report.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.1/kerykeion/settings/kerykeion_settings.py` & `kerykeion-4.6.0/kerykeion/settings/kerykeion_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    This is part of Kerykeion (C) 2023 Giacomo Battaglia
+    This is part of Kerykeion (C) 2024 Giacomo Battaglia
 """
 
 
 from json import load
 import logging
 from pathlib import Path
 from typing import Dict, Union
@@ -56,15 +56,15 @@
     Args:
         settings (KerykeionSettingsModel): The default settings
         new_settings (Dict): The new settings to add to the default ones
         
     Returns:
         KerykeionSettingsModel: The new settings
     """
-    new_settings_dict = settings.dict() | new_settings
+    new_settings_dict = settings.model_dump() | new_settings
     return KerykeionSettingsModel(**new_settings_dict)
 
 
 if __name__ == "__main__":
     from kerykeion.utilities import setup_logging
     setup_logging(level="debug")
```

### Comparing `kerykeion-4.5.1/kerykeion/settings/kr.config.json` & `kerykeion-4.6.0/kerykeion/settings/kr.config.json`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.1/kerykeion/sweph/seas_18.se1` & `kerykeion-4.6.0/kerykeion/sweph/seas_18.se1`

 * *Files identical despite different names*

### Comparing `kerykeion-4.5.1/pyproject.toml` & `kerykeion-4.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kerykeion"
-version = "4.5.1"
+version = "4.6.0"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>"]
 description = "A python library for astrology."
 license = "AGPL-3.0"
 homepage = "https://github.com/g-battaglia/kerykeion"
 repository = "https://github.com/g-battaglia/kerykeion"
 keywords = [
     "astrology",
```

### Comparing `kerykeion-4.5.1/PKG-INFO` & `kerykeion-4.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerykeion
-Version: 4.5.1
+Version: 4.6.0
 Summary: A python library for astrology.
 Home-page: https://github.com/g-battaglia/kerykeion
 License: AGPL-3.0
 Keywords: astrology,ephemeris,astrology library,birtchart,svg,zodiac,zodiac-sing,astronomical-algorithms,synastry,astrology-calculator
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kerykeion Version: 4.5.1 Summary: A python library
+Metadata-Version: 2.1 Name: kerykeion Version: 4.6.0 Summary: A python library
 for astrology. Home-page: https://github.com/g-battaglia/kerykeion License:
 AGPL-3.0 Keywords: astrology,ephemeris,astrology
 library,birtchart,svg,zodiac,zodiac-sing,astronomical-
 algorithms,synastry,astrology-calculator Author: Giacomo Battaglia Author-
 email: battaglia.giacomo@yahoo.it Requires-Python: >=3.9,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
```


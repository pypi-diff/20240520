# Comparing `tmp/grassland_production-0.3.4.tar.gz` & `tmp/grassland_production-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grassland_production-0.3.4.tar", max compression
+gzip compressed data, was "grassland_production-0.3.5.tar", max compression
```

## Comparing `grassland_production-0.3.4.tar` & `grassland_production-0.3.5.tar`

### file list

```diff
@@ -1,30 +1,33 @@
--rw-r--r--   0        0        0     1088 2023-05-25 19:51:14.000000 grassland_production-0.3.4/LICENSE
--rw-r--r--   0        0        0     5216 2024-04-29 07:11:43.031249 grassland_production-0.3.4/README.md
--rw-r--r--   0        0        0      522 2024-05-14 10:30:50.857386 grassland_production-0.3.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-23 08:43:36.000000 grassland_production-0.3.4/src/grassland_production/__init__.py
--rw-r--r--   0        0        0      222 2024-02-21 12:18:55.520411 grassland_production-0.3.4/src/grassland_production/database/__init__.py
--rw-r--r--   0        0        0   114688 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/database/grassland_management_database.db
--rw-r--r--   0        0        0    36812 2024-05-14 10:30:50.857386 grassland_production-0.3.4/src/grassland_production/dry_matter.py
--rw-r--r--   0        0        0    17071 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/farm_data_generation.py
--rw-r--r--   0        0        0    20504 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/fertilisation.py
--rw-r--r--   0        0        0        0 2024-02-21 12:18:55.532411 grassland_production-0.3.4/src/grassland_production/geo_grassland_production/__init__.py
--rw-r--r--   0        0        0     7884 2024-02-21 12:18:55.532411 grassland_production-0.3.4/src/grassland_production/geo_grassland_production/catchment_grassland.py
--rw-r--r--   0        0        0    20198 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_farm_data_generation.py
--rw-r--r--   0        0        0    12515 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_fertilisation.py
--rw-r--r--   0        0        0    12382 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_grass_yield.py
--rw-r--r--   0        0        0     6878 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_grassland_output.py
--rw-r--r--   0        0        0     6264 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_grassland_soils.py
--rw-r--r--   0        0        0    12577 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_spared_area.py
--rw-r--r--   0        0        0    12359 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/grass_yield.py
--rw-r--r--   0        0        0     8887 2024-02-21 12:18:55.532411 grassland_production-0.3.4/src/grassland_production/grassland_area.py
--rw-r--r--   0        0        0     6758 2024-01-11 17:45:50.600301 grassland_production-0.3.4/src/grassland_production/grassland_output.py
--rw-r--r--   0        0        0     6235 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/grassland_soils.py
--rw-r--r--   0        0        0        0 2024-02-21 12:18:55.532411 grassland_production-0.3.4/src/grassland_production/resource_manager/__init__.py
--rw-r--r--   0        0        0    11395 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/resource_manager/data_loader.py
--rw-r--r--   0        0        0    12745 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/resource_manager/database_manager.py
--rw-r--r--   0        0        0    13171 2024-03-28 08:10:44.380066 grassland_production-0.3.4/src/grassland_production/resource_manager/grassland_data_manager.py
--rw-r--r--   0        0        0     4894 2024-02-21 12:18:55.536411 grassland_production-0.3.4/src/grassland_production/resource_manager/scenario_data_fetcher.py
--rw-r--r--   0        0        0    12602 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/spared_area.py
--rw-r--r--   0        0        0    14033 2024-02-28 12:18:46.717106 grassland_production-0.3.4/src/grassland_production/stocking_rate.py
--rw-r--r--   0        0        0    18369 2024-02-28 12:18:46.721106 grassland_production-0.3.4/src/grassland_production/utilisation_rate.py
--rw-r--r--   0        0        0     5890 1970-01-01 00:00:00.000000 grassland_production-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-25 19:51:14.000000 grassland_production-0.3.5/LICENSE
+-rw-r--r--   0        0        0     5216 2024-04-29 07:11:43.031249 grassland_production-0.3.5/README.md
+-rw-r--r--   0        0        0      522 2024-05-20 07:28:36.824791 grassland_production-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-23 08:43:36.000000 grassland_production-0.3.5/src/grassland_production/__init__.py
+-rw-r--r--   0        0        0      222 2024-02-21 12:18:55.520411 grassland_production-0.3.5/src/grassland_production/database/__init__.py
+-rw-r--r--   0        0        0   114688 2024-05-20 07:28:36.824791 grassland_production-0.3.5/src/grassland_production/database/grassland_management_database.db
+-rw-r--r--   0        0        0    37454 2024-05-20 07:28:36.824791 grassland_production-0.3.5/src/grassland_production/dry_matter.py
+-rw-r--r--   0        0        0    17067 2024-05-20 07:28:36.824791 grassland_production-0.3.5/src/grassland_production/farm_data_generation.py
+-rw-r--r--   0        0        0    20504 2024-05-20 05:58:57.846803 grassland_production-0.3.5/src/grassland_production/fertilisation.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:18:55.532411 grassland_production-0.3.5/src/grassland_production/geo_grassland_production/__init__.py
+-rw-r--r--   0        0        0     7885 2024-05-20 07:28:36.824791 grassland_production-0.3.5/src/grassland_production/geo_grassland_production/catchment_grassland.py
+-rw-r--r--   0        0        0    19320 2024-05-20 07:28:36.824791 grassland_production-0.3.5/src/grassland_production/geo_grassland_production/geo_dry_matter.py
+-rw-r--r--   0        0        0    20214 2024-05-20 07:28:36.824791 grassland_production-0.3.5/src/grassland_production/geo_grassland_production/geo_farm_data_generation.py
+-rw-r--r--   0        0        0    12524 2024-05-20 07:28:36.824791 grassland_production-0.3.5/src/grassland_production/geo_grassland_production/geo_fertilisation.py
+-rw-r--r--   0        0        0     8693 2024-05-20 07:28:36.824791 grassland_production-0.3.5/src/grassland_production/geo_grassland_production/geo_grass_yield.py
+-rw-r--r--   0        0        0     6965 2024-05-20 07:28:36.824791 grassland_production-0.3.5/src/grassland_production/geo_grassland_production/geo_grassland_output.py
+-rw-r--r--   0        0        0     4056 2024-05-20 07:28:36.824791 grassland_production-0.3.5/src/grassland_production/geo_grassland_production/geo_grassland_soils.py
+-rw-r--r--   0        0        0     8830 2024-05-20 07:28:36.828791 grassland_production-0.3.5/src/grassland_production/geo_grassland_production/geo_spared_area.py
+-rw-r--r--   0        0        0     7517 2024-05-20 07:28:36.828791 grassland_production-0.3.5/src/grassland_production/geo_grassland_production/geo_stocking_rate.py
+-rw-r--r--   0        0        0     9268 2024-05-20 07:28:36.828791 grassland_production-0.3.5/src/grassland_production/geo_grassland_production/geo_utilisation_rate.py
+-rw-r--r--   0        0        0    12682 2024-05-20 07:28:36.828791 grassland_production-0.3.5/src/grassland_production/grass_yield.py
+-rw-r--r--   0        0        0     8886 2024-05-20 07:28:36.828791 grassland_production-0.3.5/src/grassland_production/grassland_area.py
+-rw-r--r--   0        0        0     6757 2024-05-20 07:28:36.828791 grassland_production-0.3.5/src/grassland_production/grassland_output.py
+-rw-r--r--   0        0        0     6648 2024-05-20 07:28:36.828791 grassland_production-0.3.5/src/grassland_production/grassland_soils.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:18:55.532411 grassland_production-0.3.5/src/grassland_production/resource_manager/__init__.py
+-rw-r--r--   0        0        0    11395 2024-02-28 12:18:46.717106 grassland_production-0.3.5/src/grassland_production/resource_manager/data_loader.py
+-rw-r--r--   0        0        0    12745 2024-02-28 12:18:46.717106 grassland_production-0.3.5/src/grassland_production/resource_manager/database_manager.py
+-rw-r--r--   0        0        0    13171 2024-03-28 08:10:44.380066 grassland_production-0.3.5/src/grassland_production/resource_manager/grassland_data_manager.py
+-rw-r--r--   0        0        0     4894 2024-02-21 12:18:55.536411 grassland_production-0.3.5/src/grassland_production/resource_manager/scenario_data_fetcher.py
+-rw-r--r--   0        0        0    13533 2024-05-20 07:28:36.828791 grassland_production-0.3.5/src/grassland_production/spared_area.py
+-rw-r--r--   0        0        0    14690 2024-05-20 07:28:36.828791 grassland_production-0.3.5/src/grassland_production/stocking_rate.py
+-rw-r--r--   0        0        0    19309 2024-05-20 07:28:36.828791 grassland_production-0.3.5/src/grassland_production/utilisation_rate.py
+-rw-r--r--   0        0        0     5890 1970-01-01 00:00:00.000000 grassland_production-0.3.5/PKG-INFO
```

### Comparing `grassland_production-0.3.4/LICENSE` & `grassland_production-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.4/README.md` & `grassland_production-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.4/pyproject.toml` & `grassland_production-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grassland_production"
-version = "0.3.4"
+version = "0.3.5"
 description = "Computation of grassland area and production based on animal energy calculations and grassland inputs"
 authors = ["Colm Duffy"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `grassland_production-0.3.4/src/grassland_production/database/grassland_management_database.db` & `grassland_production-0.3.5/src/grassland_production/database/grassland_management_database.db`

 * *Files 1% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -163,14 +163,18 @@
 INSERT INTO CSO_agricultural_areas VALUES('ireland',2013,4477.80000000000018);
 INSERT INTO CSO_agricultural_areas VALUES('ireland',2014,4465.80000000000018);
 INSERT INTO CSO_agricultural_areas VALUES('ireland',2015,4431.39999999999963);
 INSERT INTO CSO_agricultural_areas VALUES('ireland',2016,4461.19999999999981);
 INSERT INTO CSO_agricultural_areas VALUES('ireland',2017,4489.5);
 INSERT INTO CSO_agricultural_areas VALUES('ireland',2018,4516.30000000000018);
 INSERT INTO CSO_agricultural_areas VALUES('ireland',2019,4524.39999999999963);
+INSERT INTO CSO_agricultural_areas VALUES('ireland',2020,4511.60000000000036);
+INSERT INTO CSO_agricultural_areas VALUES('ireland',2021,4337.39999999999963);
+INSERT INTO CSO_agricultural_areas VALUES('ireland',2022,4347.89999999999963);
+INSERT INTO CSO_agricultural_areas VALUES('ireland',2023,4189.19999999999981);
 CREATE TABLE IF NOT EXISTS "CSO_cropland_areas" (
 	"ef_country"	TEXT,
 	"Year"	INTEGER,
 	"Cropland area (ha)"	REAL
 );
 INSERT INTO CSO_cropland_areas VALUES('ireland',1926,627848.0);
 INSERT INTO CSO_cropland_areas VALUES('ireland',1933,588913.0);
@@ -215,14 +219,18 @@
 INSERT INTO CSO_cropland_areas VALUES('ireland',2013,377200.0);
 INSERT INTO CSO_cropland_areas VALUES('ireland',2014,367700.0);
 INSERT INTO CSO_cropland_areas VALUES('ireland',2015,361600.0);
 INSERT INTO CSO_cropland_areas VALUES('ireland',2016,365800.0);
 INSERT INTO CSO_cropland_areas VALUES('ireland',2017,365600.0);
 INSERT INTO CSO_cropland_areas VALUES('ireland',2018,357000.0);
 INSERT INTO CSO_cropland_areas VALUES('ireland',2019,356700.0);
+INSERT INTO CSO_cropland_areas VALUES('ireland',2020,359600.0);
+INSERT INTO CSO_cropland_areas VALUES('ireland',2021,362600.0);
+INSERT INTO CSO_cropland_areas VALUES('ireland',2022,381500.0);
+INSERT INTO CSO_cropland_areas VALUES('ireland',2023,372400.0);
 CREATE TABLE IF NOT EXISTS "CSO_grassland_areas" (
 	"Year"	INTEGER,
 	"Pasture"	REAL,
 	"Hay"	REAL,
 	"Grass silage"	REAL,
 	"Rough grazing in use"	REAL
 );
@@ -250,14 +258,19 @@
 INSERT INTO CSO_grassland_areas VALUES(2012,2391.0,203.5,1075.0,481.199999999999988);
 INSERT INTO CSO_grassland_areas VALUES(2013,2337.69999999999981,218.400000000000005,1071.0,473.5);
 INSERT INTO CSO_grassland_areas VALUES(2014,2308.40000000000009,217.900000000000005,1077.5999999999999,494.199999999999988);
 INSERT INTO CSO_grassland_areas VALUES(2015,2299.40000000000009,195.699999999999988,1071.0999999999999,503.600000000000022);
 INSERT INTO CSO_grassland_areas VALUES(2016,2307.80000000000018,188.400000000000005,1066.79999999999995,532.399999999999977);
 INSERT INTO CSO_grassland_areas VALUES(2017,2322.69999999999981,192.099999999999994,1088.90000000000009,520.200000000000045);
 INSERT INTO CSO_grassland_areas VALUES(2018,2378.69999999999981,191.900000000000005,1064.5,524.100000000000022);
+INSERT INTO CSO_grassland_areas VALUES(2019,2376.69999999999981,180.800000000000011,1088.70000000000004,521.5);
+INSERT INTO CSO_grassland_areas VALUES(2020,2311.5,169.699999999999988,1199.0,471.800000000000011);
+INSERT INTO CSO_grassland_areas VALUES(2021,2186.0999999999999,124.799999999999997,1216.5999999999999,447.399999999999977);
+INSERT INTO CSO_grassland_areas VALUES(2022,2043.70000000000004,132.5,1187.70000000000004,602.5);
+INSERT INTO CSO_grassland_areas VALUES(2023,1785.20000000000004,107.099999999999994,1103.79999999999995,820.700000000000045);
 CREATE TABLE IF NOT EXISTS "utilisation_rate_calculated_from_nfs" (
 	"index"	INTEGER,
 	"Dairy"	REAL,
 	"Cattle"	REAL,
 	"Sheep"	REAL
 );
 INSERT INTO utilisation_rate_calculated_from_nfs VALUES(2005,0.805619602951088031,0.553909745563900046,0.247720783847681008);
```

### Comparing `grassland_production-0.3.4/src/grassland_production/dry_matter.py` & `grassland_production-0.3.5/src/grassland_production/dry_matter.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,18 @@
     Args:
         ef_country (str): The country for which the analysis is performed.
         calibration_year (int): The calibration year.
         target_year (int): The target year for future scenario projections.
         scenario_inputs_df (DataFrame): DataFrame containing scenario input variables data.
         scenario_animals_df (DataFrame): DataFrame containing scenario animal data.
         baseline_animals_df (DataFrame): DataFrame containing baseline animal data.
-
+        yield_class (Yield, optional): An instance of the Yield class. If not provided, a new instance 
+            is created with default parameters.
+        fertiliser_class (Fertilisation, optional): An instance of the Fertilisation class. If not 
+            provided, a new instance is created with default parameters.
 
     Attributes:
         sc_class (ScenarioDataFetcher): Fetches scenario data.
         scenario_list (list): List of scenarios.
         data_manager_class (DataManager): Manages the data retrieval for various scenarios.
         calibration_year (int): The year used for calibrating data.
         target_year (int): The year for which the scenario is targeted.
@@ -88,45 +91,57 @@
         self,
         ef_country,
         calibration_year,
         target_year,
         scenario_data,
         scenario_animals_df,
         baseline_animals_df,
+        yield_class=None,
+        fertiliser_class=None,
     ):
         self.sc_class = ScenarioDataFetcher(scenario_data)
         self.scenario_list = self.sc_class.get_scenario_list()
         self.data_manager_class = DataManager(
             calibration_year,
             target_year,
             scenario_animals_df,
             baseline_animals_df,
         )
         self.calibration_year = self.data_manager_class.get_calibration_year()
         self.target_year = self.data_manager_class.get_target_year()
         self.default_calibration_year = self.data_manager_class.get_default_calibration_year()
-        self.yield_class = Yield(
-            ef_country,
-            calibration_year,
-            target_year,
-            scenario_data,
-            scenario_animals_df,
-            baseline_animals_df,
-        )
+
+        if yield_class is None:
+            self.yield_class = Yield(
+                ef_country,
+                calibration_year,
+                target_year,
+                scenario_data,
+                scenario_animals_df,
+                baseline_animals_df,
+            )
+        else:
+            self.yield_class = yield_class
+
         self.areas_class = Areas(
             target_year, calibration_year, self.default_calibration_year
         )
-        self.fertiliser_class = Fertilisation(
-            ef_country,
-            calibration_year,
-            target_year,
-            scenario_data,
-            scenario_animals_df,
-            baseline_animals_df,
-        )
+
+        if fertiliser_class is None:
+            self.fertiliser_class = Fertilisation(
+                ef_country,
+                calibration_year,
+                target_year,
+                scenario_data,
+                scenario_animals_df,
+                baseline_animals_df,
+            )
+        else:
+            self.fertiliser_class = fertiliser_class
+
         self.loader_class = Loader()
         self.grass_feed_class = cattle_lca.GrassFeed(ef_country)
         self.sheep_grass_feed_class = sheep_lca.GrassFeed(ef_country)
 
 
 
     def get_actual_dry_matter_produced(self):
```

### Comparing `grassland_production-0.3.4/src/grassland_production/farm_data_generation.py` & `grassland_production-0.3.5/src/grassland_production/farm_data_generation.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,25 +31,28 @@
     Args:
         ef_country (str): The country for which the analysis is performed.
         calibration_year (int): The calibration year.
         target_year (int): The target year for future scenario projections.
         scenario_inputs_df (DataFrame): DataFrame containing scenario input variables data.
         scenario_animals_df (DataFrame): DataFrame containing scenario animal data.
         baseline_animals_df (DataFrame): DataFrame containing baseline animal data.
+        
 
     Attributes:
-        loader_class (Loader): Instance of Loader to load various datasets.
-        sc_class (ScenarioDataFetcher): Instance of ScenarioDataFetcher for fetching scenario data.
-        scenario_list (list): List of scenarios for analysis.
-        data_manager_class (DataManager): Instance of DataManager for managing scenario and baseline data.
-        areas_class (Areas): Instance of Areas for calculating areas-related data.
-        grassland_class (Grasslands): Instance for calculating grassland related data.
-        fertiliser_class (Fertilisation): Instance for handling fertilization-related calculations.
-        calibration_year (int): The base year for data calibration.
-        target_year (int): The target year for future scenario projections.
+        loader_class (Loader): An instance of the Loader class.
+        sc_class (ScenarioDataFetcher): An instance of the ScenarioDataFetcher class.
+        scenario_list (list): A list of scenarios for analysis.
+        data_manager_class (DataManager): An instance of the DataManager class.
+        calibration_year (int): The calibration year.
+        default_calibration_year (int): The default calibration year.
+        default_grassland_year (int): The default grassland year.
+        target_year (int): The target year.
+        areas_class (Areas): An instance of the Areas class.
+        grassland_class (Grasslands): An instance of the Grasslands class.
+        fertiliser_class (Fertilisation): An instance of the Fertilisation class.
 
     Methods:
         compute_fertilization_total():
             Calculates the total fertilization rates across different scenarios, considering various livestock 
             systems and grassland types.
 
         compute_farm_data_in_scenarios():
```

### Comparing `grassland_production-0.3.4/src/grassland_production/fertilisation.py` & `grassland_production-0.3.5/src/grassland_production/fertilisation.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.4/src/grassland_production/geo_grassland_production/catchment_grassland.py` & `grassland_production-0.3.5/src/grassland_production/geo_grassland_production/catchment_grassland.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
         'Rough grazing in use', calculated separately.
 
         Returns:
             pandas.DataFrame: A DataFrame with each row representing a grassland cover type and 
                             its calculated area in hectares ('area_ha').
         """
         catchment_grassland_area = self.get_catchment_grassland_areas()
+
         grassland_proprotions = self.loader_class.cso_grassland_area_percent()
 
         data =[]
 
         mask = (catchment_grassland_area.index == "Pasture")
         for col in grassland_proprotions.columns:
```

### Comparing `grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_farm_data_generation.py` & `grassland_production-0.3.5/src/grassland_production/geo_grassland_production/geo_farm_data_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-==================
+====================
 Geo Farm Data Module
-==================
+====================
 
 This module includes the FarmData class which is responsible for computing various aspects of farm data, 
 such as fertilization totals and farm data in different scenarios in a specific catchment. This data is essential for lifecycle 
 assessment calculations and agricultural planning.
 
 Classes:
     FarmData: Manages the computation of farm data for lifecycle assessments and scenario analysis.
@@ -13,16 +13,16 @@
 
 import pandas as pd
 import itertools
 from grassland_production.resource_manager.data_loader import Loader
 from grassland_production.resource_manager.grassland_data_manager import DataManager
 from grassland_production.resource_manager.scenario_data_fetcher import ScenarioDataFetcher
 from grassland_production.grassland_area import Areas
-from grassland_production.geo_grassland_production.geo_spared_area import Grasslands
-from grassland_production.geo_grassland_production.geo_fertilisation import Fertilisation
+from grassland_production.geo_grassland_production.geo_spared_area import GeoGrasslands
+from grassland_production.geo_grassland_production.geo_fertilisation import GeoFertilisation
 
 
 class FarmData:
     """
     The FarmData class handles the computation of various farm-related data elements, including 
     fertilization rates and overall farm data for baseline and future scenarios in specific catchments. This class plays 
     a pivotal role in lifecycle assessment and agricultural scenario analysis by providing essential 
@@ -96,23 +96,23 @@
         self.target_year = self.data_manager_class.get_target_year()
         self.default_urea = self.data_manager_class.get_default_urea_proportion()
         self.default_urea_abated = self.data_manager_class.get_default_urea_abated_proportion()
 
         self.areas_class = Areas(
             self.target_year, self.calibration_year, self.default_calibration_year
         )
-        self.grassland_class = Grasslands(
+        self.grassland_class = GeoGrasslands(
             ef_country,
             calibration_year,
             target_year,
             scenario_data,
             scenario_animals_df,
             baseline_animals_df,
         )
-        self.fertiliser_class = Fertilisation(
+        self.fertiliser_class = GeoFertilisation(
             ef_country,
             calibration_year,
             target_year,
             scenario_data,
             scenario_animals_df,
             baseline_animals_df,
         )
```

### Comparing `grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_fertilisation.py` & `grassland_production-0.3.5/src/grassland_production/geo_grassland_production/geo_fertilisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 """
-======================
-Fertilisation Module
-======================
+========================
+Geo Fertilisation Module
+========================
 
-This module encompasses the Fertilisation classes (both geo_fertilisation and fertilisation), which is focused on computing various fertilisation 
+This module encompasses the GeoFertilisation classes (both geo_fertilisation and fertilisation), which is focused on computing various fertilisation 
 rates and their distribution across different farm systems and scenarios. This class is used in the calculation of 
 grassland production for catchments.
 
 Classes:
-    Fertilisation: Manages the computation of fertilization-related data for different farm systems and scenarios.
+    GeoFertilisation: Manages the computation of fertilization-related data for different farm systems and scenarios.
 """
 
 from itertools import product
-import pandas as pd
 from grassland_production.resource_manager.data_loader import Loader
 from grassland_production.resource_manager.grassland_data_manager import DataManager
 from grassland_production.resource_manager.scenario_data_fetcher import ScenarioDataFetcher
-
 from grassland_production.grassland_area import Areas
-from grassland_production.fertilisation import Fertilisation as Fert
+from grassland_production.fertilisation import Fertilisation
 from cattle_lca.lca import DailySpread
 from grassland_production.geo_grassland_production.catchment_grassland import CatchmentGrass
 
 
-class Fertilisation:
+class GeoFertilisation:
     """
-    The Fertilisation class is responsible for calculating both inorganic and organic fertilization rates 
+    The GeoFertilisation class is responsible for calculating both inorganic and organic fertilization rates 
     and their application across various farm systems and scenarios. This class plays a crucial role in 
     the calculation of grassland production, providing insights into the environmental impact of fertilization 
     practices and aiding in the development of sustainable agricultural strategies.
 
     Args:
         ef_country (str): The country for which the analysis is performed.
         calibration_year (int): The calibration year for historical data.
@@ -99,15 +97,15 @@
         self.default_grassland_year = self.data_manager_class.get_default_grassland_year()
         self.target_year = self.data_manager_class.get_target_year()
 
         self.loader_class = Loader()
         self.areas_class = Areas(
             self.target_year, calibration_year, self.default_calibration_year
         )
-        self.fert_class = Fert(ef_country,
+        self.fert_class = Fertilisation(ef_country,
                                 calibration_year,
                                 target_year,
                                 scenario_data,
                                 scenario_animals_df,
                                 baseline_animals_df)
 
         self.cattle_spread_class = DailySpread(ef_country)
@@ -183,14 +181,15 @@
 
         Notes:
             - Sheep systems are excluded from this calculation.
             - If data for the calibration year is not present, a default year is used.
         """
         spread_dict = self.compute_organic_fertilization_rate()
         grassland_areas = self.catchment_grass.get_catchment_grassland_area_caluclated()
+        
         nfs_system_proportions = self.areas_class.get_nfs_system_proportions()
         
         dairy_nfs_system_proportions = nfs_system_proportions[0]
         beef_nfs_system_proportions = nfs_system_proportions[1]
 
         systems_dict = {
             "dairy": dairy_nfs_system_proportions,
```

### Comparing `grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_grass_yield.py` & `grassland_production-0.3.5/src/grassland_production/grass_yield.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,110 +1,96 @@
 """
 ====================
 Grass Yield Module
 ====================
 
 This module includes the Yield class, which calculates grass yield per hectare for various farm systems 
-and scenarios for the selected catchment. 
-The class uses models and data to estimate yields based on different fertilization strategies 
+and scenarios. The class uses models and data to estimate yields based on different fertilization strategies 
 and soil conditions.
 
 Classes:
     Yield: Manages the computation of grass yield for different farm systems and scenarios.
 """
-
 import pandas as pd
 from itertools import product
 from grassland_production.resource_manager.data_loader import Loader
 from grassland_production.resource_manager.grassland_data_manager import DataManager
 from grassland_production.resource_manager.scenario_data_fetcher import ScenarioDataFetcher
-from grassland_production.geo_grassland_production.geo_fertilisation import Fertilisation
-from grassland_production.grass_yield import Yield as GrasslandYield
+from grassland_production.fertilisation import Fertilisation
+
 
 class Yield:
     """
-    The Yield class is responsible for calculating grass yield per hectare for various farm systems (dairy, beef, sheep)
-    under different scenarios for the specified catchment. This calculation takes into account factors such as fertilization (both inorganic and organic),
-    clover proportion, soil types, and other variables, to estimate the impact on grass yield.
-
-    This class integrates data from multiple sources, including fertilization rates and soil characteristics, to provide 
-    a comprehensive analysis of grassland production potential under varying agricultural practices and environmental conditions.
-
-    Args:
-        ef_country (str): The country for which the analysis is performed.
-        calibration_year (int): The calibration year for historical data reference.
-        target_year (int): The target year for projecting future scenarios.
-        scenario_inputs_df (DataFrame): DataFrame containing input variables for different scenarios.
-        scenario_animals_df (DataFrame): DataFrame containing data on animals involved in different scenarios.
-        baseline_animals_df (DataFrame): DataFrame containing baseline data on animal populations.
-
-    Attributes:
-        sc_class (ScenarioDataFetcher): Instance of ScenarioDataFetcher for fetching scenario data.
-        scenario_list (list): List of scenarios for which the analysis is performed.
-        data_manager_class (DataManager): Instance of DataManager for managing data related to grass yield.
-        geo_fertiliser_class (Fertilisation): Instance of Fertilisation for handling geo-specific fertilization data.
-        grass_yield_class (GrasslandYield): Instance of Yield class from the grassland_production lib.
-        loader_class (Loader): Instance of Loader to load various necessary datasets.
-        calibration_year (int): The base year for data calibration and historical reference.
-        target_year (int): The target year for future scenario projections.
-        soil_class_yield_gap (dict): A dictionary mapping soil types to their respective yield gaps.
-        soil_class_prop (DataFrame): A DataFrame indicating the proportion of different soil types across scenarios.
-
-    Methods:
-        get_clover_parameters():
-            Retrieves clover parameters, such as proportion and fertilization rate, for each scenario, differentiating between 
-            conventional yield response curves and clover-grass systems.
-
-        get_yield():
-            Calculates the grass yield per hectare for each grassland type, farm system, and scenario. This method takes into 
-            account various factors including fertilization rates, soil properties, and clover parameters.
-
-        _yield_response_function_to_fertilizer(fertilizer, grassland, clover_prop=0, clover_fert=0, manure_spread=0):
-            An internal method that models the yield response to various factors including fertilizer application, clover proportion,
-            and organic manure spread. This function is critical in determining the yield per hectare under different scenarios.
-
-    Note:
-        This class is part of a broader framework aimed at understanding and optimizing grassland production. It should be used 
-        in conjunction with other related classes to gain a holistic view of the agricultural systems under study.
-    """
+        The Yield class is dedicated to calculating grass yield per hectare for different farm systems (dairy, beef, 
+        sheep) under various scenarios. It considers the impact of fertilization (both inorganic and organic), 
+        clover proportion, soil types, and other factors on grass yield.
+
+        Args:
+            ef_country (str): The country for which the analysis is performed.
+            calibration_year (int): The calibration year.
+            target_year (int): The target year for future scenario projections.
+            scenario_inputs_df (DataFrame): DataFrame containing scenario input variables data.
+            scenario_animals_df (DataFrame): DataFrame containing scenario animal data.
+            baseline_animals_df (DataFrame): DataFrame containing baseline animal data.
+            fertiliser_class (Fertilisation, optional): Instance of Fertilisation for handling fertilization-related data.
+
+        Attributes:
+            sc_class (ScenarioDataFetcher): Instance of ScenarioDataFetcher for fetching scenario data.
+            scenario_list (list): List of scenarios.
+            data_manager_class (DataManager): Instance of DataManager for managing data related to yield.
+            fertiliser_class (Fertilisation): Instance of Fertilisation for handling fertilization-related data.
+            loader_class (Loader): Instance of Loader to load various datasets.
+            calibration_year (int): The base year for data calibration.
+            target_year (int): The target year for future scenario projections.
+            soil_class_yield_gap (dict): A dictionary mapping soil types to yield gaps.
+            soil_class_prop (DataFrame): A DataFrame indicating the proportion of different soil types.
+
+        Methods:
+            get_clover_parameters():
+                Defines clover proportion and rate for different scenarios to differentiate between conventional 
+                yield response curves and clover-grass systems.
+
+            get_yield():
+                Calculates the yield per hectare for each grassland type, farm system, and scenario.
+
+            _yield_response_function_to_fertilizer():
+                Internal method to model the yield response to fertilizer application.
+        """
     def __init__(
         self,
         ef_country,
         calibration_year,
         target_year,
         scenario_data,
         scenario_animals_df,
         baseline_animals_df,
+        fertiliser_class = None
     ):
         self.sc_class = ScenarioDataFetcher(scenario_data)
         self.scenario_list = self.sc_class.get_scenario_list()
 
         self.data_manager_class = DataManager(
             calibration_year,
             target_year,
             scenario_animals_df,
             baseline_animals_df,
         )
-        self.geo_fertiliser_class = Fertilisation(
-            ef_country,
-            calibration_year,
-            target_year,
-            scenario_data,
-            scenario_animals_df,
-            baseline_animals_df,
-        )
 
-        #Classes from Main Model    
-        self.grass_yield_class = GrasslandYield(ef_country,
-                        calibration_year,
-                        target_year,
-                        scenario_data,
-                        scenario_animals_df,
-                        baseline_animals_df)
-        
+        if fertiliser_class is None:
+            self.fertiliser_class = Fertilisation(
+                ef_country,
+                calibration_year,
+                target_year,
+                scenario_data,
+                scenario_animals_df,
+                baseline_animals_df,
+            )
+        else: 
+            self.fertiliser_class = fertiliser_class 
+            
         self.loader_class = Loader()
         self.calibration_year = self.data_manager_class.get_calibration_year()
         self.target_year = self.data_manager_class.get_target_year()
 
         self.soil_class_yield_gap = self.data_manager_class.get_yield_gap()
 
         self.soil_class_prop = self.data_manager_class.get_soil_properties()
@@ -123,22 +109,51 @@
             dict: A dictionary containing clover parameters for different scenarios and farm systems.
 
         The clover parameters include:
             - Clover proportion: The proportion of clover in the pasture.
             - Clover fertilisation rate: The rate of clover fertilisation.
 
         """
-        clover_dict = self.grass_yield_class.get_clover_parameters()
+        scenario_df = self.sc_class.get_scenario_dataframe()
+
+        keys = ["dairy", "beef", "sheep"]
+        inner_keys = ["proportion", "fertilisation"]
+
+        clover_dict = {key: {inner_key: {} for inner_key in inner_keys} for key in keys}
+
+        conditions = {
+            "dairy": (
+                    (scenario_df["Cattle systems"] == "Dairy")
+                    & (scenario_df["Manure management"] == "tank liquid")
+            ),
+            "beef": (
+                    (scenario_df["Cattle systems"] == "Beef")
+                    & (scenario_df["Manure management"] == "tank liquid")
+            ),
+            "sheep": (
+                    (scenario_df["Cattle systems"] == "Lowland sheep")
+                    & (scenario_df["Manure management"] == "solid")
+            )
+        }
+
+        for key in keys:
+            for sc in scenario_df["Scenarios"].unique():
+                mask = (scenario_df["Scenarios"] == sc) & conditions[key]
+                clover_proportion = self.sc_class.get_clover_proportion_value(mask)
+                clover_fertilisation = self.sc_class.get_clover_fertilisation_value(mask)
+                clover_dict[key]["proportion"][sc] = clover_proportion
+                clover_dict[key]["fertilisation"][sc] = clover_fertilisation
+
 
         return clover_dict
        
 
     def get_yield(self):
         """
-        Calculates the yield per hectare for different scenarios and farm systems for the catchment based on fertilization and other factors.
+        Calculates the yield per hectare for different scenarios and farm systems based on fertilization and other factors.
         The method computes yield values for dairy, beef, and sheep farm systems under various scenarios.
 
         The method utilizes information on fertilization rates, organic manure spread, soil properties, and clover parameters
         to calculate yields for each scenario and farm system. It iterates through different combinations of scenarios,
         farm systems, grassland types, and soil groups to compute yields.
 
         Returns:
@@ -149,18 +164,19 @@
                 - Values: Pandas DataFrames containing yield values for different grassland types (e.g., "Pasture," "Grass silage").
                     - The DataFrame's rows correspond to grassland types.
                     - The DataFrame's columns correspond to calibration and target years.
         """
         fertilization_by_system_data_frame = (
             self.loader_class.grassland_fertilization_by_system()
         )
-        fert_rate = self.geo_fertiliser_class.compute_inorganic_fertilization_rate()
+        fert_rate = self.fertiliser_class.compute_inorganic_fertilization_rate()
+
+
+        organic_manure = self.fertiliser_class.organic_fertilisation_per_ha()
 
-        #Catchment specific
-        organic_manure = self.geo_fertiliser_class.organic_fertilisation_per_ha()
 
         year_list = [self.calibration_year, self.target_year]
         scenario_list = self.scenario_list
 
         clover_parameters_dict = self.get_clover_parameters()
 
         keys = ["dairy", "beef", "sheep"]
@@ -179,14 +195,15 @@
 
         for sc, farm_type, grassland_type, soil_group in product(
             scenario_list,
             keys,
             fertilization_by_system_data_frame.index.levels[0],
             self.soil_class_yield_gap.keys(),
         ):
+            
             yield_per_ha_df = yield_per_ha[farm_type][sc]
             soil_class_prop = self.soil_class_prop[farm_type].loc[
                 int(self.calibration_year), soil_group
             ]
 
             yield_per_ha_df.loc[grassland_type, int(self.calibration_year)] += (
                 self._yield_response_function_to_fertilizer(
@@ -195,14 +212,15 @@
                     ],
                     grassland_type,
                     manure_spread=organic_manure[sc].loc[int(self.calibration_year), farm_type],
                 )
                 * self.soil_class_yield_gap[soil_group]
             ) * soil_class_prop
 
+
             clover_prop = clover_parameters_dict[farm_type]["proportion"][sc]
             clover_fert = clover_parameters_dict[farm_type]["fertilisation"][sc]
 
             yield_per_ha_df.loc[grassland_type, int(self.target_year)] += (
                 self._yield_response_function_to_fertilizer(
                     fert_rate[farm_type][sc].loc[grassland_type, str(self.target_year)],
                     grassland_type,
@@ -244,12 +262,25 @@
         Returns:
             float: The estimated yield response to the specified fertilizer application (in metric tons per hectare).
 
 
         Note: The result is converted to metric tons per hectare using the factor 1e-3.
 
         """
-        yield_response = self.grass_yield_class._yield_response_function_to_fertilizer(
-            fertilizer, grassland, clover_prop, clover_fert, manure_spread
-        )
+
+        kg_to_t = 1e-3
+        if grassland == "Grass silage" or grassland == "Pasture":
+         
+            yield_response_default = ((-0.0444 * ((fertilizer + manure_spread) ** 2)
+                + 38.419 * (fertilizer + manure_spread)
+                + 6257) * (1 - clover_prop)) 
+            
+            yield_response_clover = (0.7056 * (clover_fert + manure_spread) + 12829) * clover_prop
+
+            yield_response = yield_response_default + yield_response_clover
+
+        else:
+            yield_response = -0.0444 * (fertilizer**2) + 38.419 * fertilizer + 6257
+
+        yield_response = yield_response * kg_to_t
 
         return yield_response
```

### Comparing `grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_grassland_output.py` & `grassland_production-0.3.5/src/grassland_production/geo_grassland_production/geo_grassland_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """
-=================================
+===============================
 Grassland Output Manager Module
-=================================
+===============================
 This module contains the GrasslandOutput class, which is responsible for managing and
 processing various outputs related to grassland production and management. The class
 integrates different aspects of grassland management, such as grasslands, farm data,
 soil groups, dry matter production, and stocking rates, to provide easy retrieval of grassland
 scenario results.
 
 Classes:
     GrasslandOutput: Manages and computes outputs for grassland management for catchment analysis.
 
 """
-
-from grassland_production.geo_grassland_production.geo_spared_area import Grasslands
+from grassland_production.geo_grassland_production.geo_spared_area import GeoGrasslands
 from grassland_production.geo_grassland_production.geo_farm_data_generation import FarmData
-from grassland_production.geo_grassland_production.geo_grassland_soils import SoilGroups
-from grassland_production.dry_matter import DryMatter
-from grassland_production.stocking_rate import StockingRate
+from grassland_production.geo_grassland_production.geo_grassland_soils import GeoSoilGroups
+from grassland_production.geo_grassland_production.geo_dry_matter import GeoDryMatter
+from grassland_production.geo_grassland_production.geo_stocking_rate import GeoStockingRate
 
 import pandas as pd
 
 class GrasslandOutput:
     """
     A class to manage and format outputs related to grassland production and management.
 
@@ -36,16 +35,16 @@
         scenario_inputs_df (DataFrame): DataFrame containing scenario input variables data.
         scenario_animals_df (DataFrame): DataFrame containing scenario animal data.
         baseline_animals_df (DataFrame): DataFrame containing baseline animal data.
 
     Attributes:
         grassland_class (Grasslands): An instance of the (geo) Grasslands class.
         farm_data_class (FarmData): An instance of the FarmData class.
-        soil_groups_class (SoilGroups): An instance of the SoilGroups class.
-        dm_class (DryMatter): An instance of the DryMatter class.
+        soil_groups_class (GeoSoilGroups): An instance of the GeoSoilGroups class.
+        dm_class ( GeoDryMatter): An instance of the DryMatter class.
         stock_class (StockingRate): An instance of the StockingRate class.
 
     Methods:
         total_spared_area(): Returns the total area spared (former grassland).
         total_grassland_area(): Returns the total area of grassland (remaining).
         total_spared_area_breakdown(): Provides a breakdown of spared areas by soil group.
         farm_inputs_data(): Computes and returns farm data for different scenarios.
@@ -58,15 +57,15 @@
         ef_country,
         calibration_year,
         target_year,
         scenario_data,
         scenario_animals_df,
         baseline_animals_df,
     ):
-        self.grassland_class = Grasslands(
+        self.grassland_class = GeoGrasslands(
             ef_country,
             calibration_year,
             target_year,
             scenario_data,
             scenario_animals_df,
             baseline_animals_df,
         )
@@ -75,33 +74,33 @@
             calibration_year,
             target_year,
             scenario_data,
             scenario_animals_df,
             baseline_animals_df,
         )
 
-        self.soil_groups_class = SoilGroups(
+        self.soil_groups_class = GeoSoilGroups(
             ef_country,
             calibration_year,
             target_year,
             scenario_data,
             scenario_animals_df,
             baseline_animals_df,
         )
 
-        self.dm_class = DryMatter(
+        self.dm_class = GeoDryMatter(
             ef_country,
             calibration_year,
             target_year,
             scenario_data,
             scenario_animals_df,
             baseline_animals_df,
         )
 
-        self.stock_class = StockingRate(
+        self.stock_class = GeoStockingRate(
             ef_country,
             calibration_year,
             target_year,
             scenario_data,
             scenario_animals_df,
             baseline_animals_df,
         )
```

### Comparing `grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_grassland_soils.py` & `grassland_production-0.3.5/src/grassland_production/grassland_soils.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,18 @@
 The module utilizes several components from the grassland_production package to 
 compute and provide detailed insights into soil group distributions for grassland management.
 
 Classes:
     SoilGroups: Manages soil group data.
 
 """
-
 import pandas as pd
 from grassland_production.resource_manager.data_loader import Loader
 from grassland_production.resource_manager.grassland_data_manager import DataManager
-from grassland_production.geo_grassland_production.geo_spared_area import Grasslands
+from grassland_production.spared_area import Grasslands
 import itertools
 
 class SoilGroups:
     """
     A class to manage and analyze soil group data for different grassland cohorts.
 
     The SoilGroups class integrates data from various sources to provide a comprehensive
@@ -31,14 +30,16 @@
     Args:
         ef_country (str): The country for which the analysis is performed.
         calibration_year (int): The calibration year.
         target_year (int): The target year for future scenario projections.
         scenario_inputs_df (DataFrame): DataFrame containing scenario input variables data.
         scenario_animals_df (DataFrame): DataFrame containing scenario animal data.
         baseline_animals_df (DataFrame): DataFrame containing baseline animal data.
+        grassland_class (Grasslands, optional): An instance of the Grassland class. If not 
+            provided, a new instance is created with default parameters.
 
     Attributes:
         data_manager_class (DataManager): Manages and processes grassland data.
         calibration_year (int): Year of data calibration.
         target_year (int): Target year for data analysis.
         default_calibration_year (int): Default year used for calibration in case of data discrepancies.
         loader_class (Loader): Class for loading necessary data.
@@ -48,28 +49,38 @@
         beef_soil_distribution (DataFrame): Soil distribution data for beef grasslands.
         sheep_soil_distribution (DataFrame): Soil distribution data for sheep grasslands.
         grassland_class (Grasslands): Class for managing grassland data.
 
     Methods:
         get_cohort_soil_groups(): Computes and returns the soil group distribution for spared (destocked) areas.
     """
-    def __init__(self, ef_country, calibration_year, target_year, scenario_data, scenario_animals_df,baseline_animals_df):
+    def __init__(self, 
+                 ef_country,
+                 calibration_year, 
+                 target_year,
+                 scenario_data,
+                 scenario_animals_df,
+                 baseline_animals_df,
+                 grassland_class=None):
 
         self.data_manager_class = DataManager(calibration_year, target_year, scenario_animals_df,baseline_animals_df)
         self.calibration_year = self.data_manager_class.get_calibration_year()
         self.target_year = self.data_manager_class.get_target_year()
         self.default_calibration_year = self.data_manager_class.get_default_calibration_year()
         self.loader_class = Loader()
         self.scenario_animals_df = scenario_animals_df
         self.baseline_animals_df = baseline_animals_df
         self.dairy_soil_distribution = self.loader_class.dairy_soil_group()
         self.beef_soil_distribution = self.loader_class.cattle_soil_group()
         self.sheep_soil_distribution = self.loader_class.sheep_soil_group()
-        self.grassland_class = Grasslands(ef_country, self.calibration_year, target_year, scenario_data, scenario_animals_df, baseline_animals_df)
 
+        if grassland_class is None:
+            self.grassland_class = Grasslands(ef_country, self.calibration_year, target_year, scenario_data, scenario_animals_df, baseline_animals_df)
+        else:
+            self.grassland_class = grassland_class
 
 
     def get_cohort_soil_groups(self):
         """
         Computes and returns a detailed breakdown of soil groups across different livestock cohorts for spared areas.
 
         This method analyzes soil distribution among various cohorts (such as dairy, beef,
```

### Comparing `grassland_production-0.3.4/src/grassland_production/geo_grassland_production/geo_spared_area.py` & `grassland_production-0.3.5/src/grassland_production/spared_area.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,38 +7,40 @@
 data related to grassland areas, specifically focusing on calculating the total 
 grassland area and spared area under various scenarios. It utilizes classes from 
 the grassland_production package for detailed analysis and computations.
 
 Classes:
     Grasslands: Manages and computes grassland and spared area data.
 """
-
 import pandas as pd
 from grassland_production.resource_manager.data_loader import Loader
 from grassland_production.resource_manager.grassland_data_manager import DataManager
 from grassland_production.resource_manager.scenario_data_fetcher import ScenarioDataFetcher
-from grassland_production.geo_grassland_production.geo_grass_yield import Yield
+from grassland_production.grass_yield import Yield
 from grassland_production.dry_matter import DryMatter
 from grassland_production.grassland_area import Areas
 from grassland_production.utilisation_rate import UtilisationRate
 
 class Grasslands:
     """
-    A class to manage and compute catchment grassland and spared area data under various scenarios.
+    A class to manage and compute grassland and spared area data under various scenarios.
 
     This class integrates data from various sources to assess the total area of grasslands 
     and the spared area (destocked grassland) for different scenarios.
 
     Args:
         ef_country (str): The country for which the analysis is performed.
         calibration_year (int): The calibration year.
         target_year (int): The target year for future scenario projections.
         scenario_inputs_df (DataFrame): DataFrame containing scenario input variables data.
         scenario_animals_df (DataFrame): DataFrame containing scenario animal data.
         baseline_animals_df (DataFrame): DataFrame containing baseline animal data.
+        yield_class (Yield, optional): An instance of the Yield class. If not provided, a new instance is created with default parameters.
+        dry_matter_class (DryMatter, optional): An instance of the DryMatter class. If not provided, a new instance is created with default parameters.
+        utilisation_class (UtilisationRate, optional): An instance of the UtilisationRate class. If not provided, a new instance is created with default parameters.
 
     Attributes:
         sc_class (ScenarioDataFetcher): Fetches scenario data.
         scenario_list (list): List of scenarios.
         data_manager_class (DataManager): Manages and processes grassland data.
         calibration_year (int): Year of data calibration.
         target_year (int): Target year for data analysis.
@@ -59,54 +61,69 @@
         self,
         ef_country,
         calibration_year,
         target_year,
         scenario_data,
         scenario_animals_df,
         baseline_animals_df,
+        yield_class = None,
+        dry_matter_class = None,
+        utilisation_class = None
     ):
         self.sc_class = ScenarioDataFetcher(scenario_data)
         self.scenario_list = self.sc_class.get_scenario_list()
 
         self.data_manager_class = DataManager(
             calibration_year,
             target_year,
             scenario_animals_df,
             baseline_animals_df,
         )
         self.calibration_year = self.data_manager_class.get_calibration_year()
         self.target_year = self.data_manager_class.get_target_year()
-        self.default_calibration_year = self.data_manager_class.get_default_calibration_year()
+        self.default_calibration_year = self.data_manager_class.get_default_calibration_year()  
         self.loader_class = Loader()
-        self.yield_class = Yield(
-            ef_country,
-            calibration_year,
-            target_year,
-            scenario_data,
-            scenario_animals_df,
-            baseline_animals_df,
-        )
+
+        if yield_class is None:
+            self.yield_class = Yield(
+                ef_country,
+                calibration_year,
+                target_year,
+                scenario_data,
+                scenario_animals_df,
+                baseline_animals_df,
+            )
+        else:
+            self.yield_class = yield_class 
+
         self.areas_class = Areas(
             self.target_year, self.calibration_year, self.default_calibration_year
         )
-        self.dm_class = DryMatter(
-            ef_country,
-            self.calibration_year,
-            target_year,
-            scenario_data,
-            scenario_animals_df,
-            baseline_animals_df,
-        )
 
-        self.farm_based_UR = UtilisationRate(ef_country,
-            self.calibration_year,
-            target_year,
-            scenario_data,
-            scenario_animals_df,
-            baseline_animals_df,)
+        if dry_matter_class is None:
+            self.dm_class = DryMatter(
+                ef_country,
+                self.calibration_year,
+                target_year,
+                scenario_data,
+                scenario_animals_df,
+                baseline_animals_df,
+            )
+        else:
+            self.dm_class = dry_matter_class
+
+        if utilisation_class is None:
+            self.farm_based_UR = UtilisationRate(ef_country,
+                self.calibration_year,
+                target_year,
+                scenario_data,
+                scenario_animals_df,
+                baseline_animals_df,)
+        else:
+            self.farm_based_UR = utilisation_class
 
     def get_grass_total_area(self):
         """
         Calculates and returns the total grassland area for each scenario and system over specified years.
 
         This method computes the total area of grasslands required to meet the dry matter requirements
         for dairy, beef and sheep. It uses a weighted average yield of different grassland types within each 
@@ -129,14 +146,16 @@
         # grass drymatter requirement for cattle and sheep, is dictionary
         year_list = [self.calibration_year, self.target_year]
         scenario_list = self.scenario_list
 
         keys = self.data_manager_class.get_farming_systems()
 
         transposed_yield_per_ha = self.yield_class.get_yield()
+
+
         dry_matter_req = self.dm_class.actual_dry_matter_required()
 
         farm_based_UR = self.farm_based_UR.get_farm_based_utilisation_rate()
 
         nfs_within_grassland_proportions = (
             self.areas_class.get_nfs_within_system_grassland_distribution()
         )
@@ -237,16 +256,17 @@
         spared_area = self.get_non_grass_total_area()
 
         cohort_spared_area = {}
 
         for sc in cohort_weights.keys():
             cohort_spared_area[sc] = {}
             for cohort in cohort_weights[sc].keys():
-                cohort_spared_area[sc][cohort] = spared_area.loc[self.target_year, sc].item() * cohort_weights[sc][cohort]
-
+                if cohort != "total":
+                    
+                    cohort_spared_area[sc][cohort] = spared_area.loc[self.target_year, sc].item() * cohort_weights[sc][cohort]
 
         return cohort_spared_area
     
 
     def get_cohort_grassland_area(self):
         """
         Calculates and returns the grassland area for each cohort within each scenario.
```

### Comparing `grassland_production-0.3.4/src/grassland_production/grass_yield.py` & `grassland_production-0.3.5/src/grassland_production/geo_grassland_production/geo_grass_yield.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,97 @@
 """
-====================
-Grass Yield Module
-====================
-
-This module includes the Yield class, which calculates grass yield per hectare for various farm systems 
-and scenarios. The class uses models and data to estimate yields based on different fertilization strategies 
+======================
+Geo Grass Yield Module
+======================
+
+This module includes the GeoYield class, which calculates grass yield per hectare for various farm systems 
+and scenarios for the selected catchment. 
+The class uses models and data to estimate yields based on different fertilization strategies 
 and soil conditions.
 
 Classes:
-    Yield: Manages the computation of grass yield for different farm systems and scenarios.
+    GeoYield: Manages the computation of grass yield for different farm systems and scenarios.
 """
+from grassland_production.geo_grassland_production.geo_fertilisation import GeoFertilisation
+from grassland_production.grass_yield import Yield
 
-import pandas as pd
-from itertools import product
-from grassland_production.resource_manager.data_loader import Loader
-from grassland_production.resource_manager.grassland_data_manager import DataManager
-from grassland_production.resource_manager.scenario_data_fetcher import ScenarioDataFetcher
-from grassland_production.fertilisation import Fertilisation
-
-
-class Yield:
+class GeoYield:
+    """
+    The Yield class is responsible for calculating grass yield per hectare for various farm systems (dairy, beef, sheep)
+    under different scenarios for the specified catchment. This calculation takes into account factors such as fertilization (both inorganic and organic),
+    clover proportion, soil types, and other variables, to estimate the impact on grass yield.
+
+    This class integrates data from multiple sources, including fertilization rates and soil characteristics, to provide 
+    a comprehensive analysis of grassland production potential under varying agricultural practices and environmental conditions.
+
+    Args:
+        ef_country (str): The country for which the analysis is performed.
+        calibration_year (int): The calibration year for historical data reference.
+        target_year (int): The target year for projecting future scenarios.
+        scenario_inputs_df (DataFrame): DataFrame containing input variables for different scenarios.
+        scenario_animals_df (DataFrame): DataFrame containing data on animals involved in different scenarios.
+        baseline_animals_df (DataFrame): DataFrame containing baseline data on animal populations.
+
+    Attributes:
+        sc_class (ScenarioDataFetcher): Instance of ScenarioDataFetcher for fetching scenario data.
+        scenario_list (list): List of scenarios for which the analysis is performed.
+        data_manager_class (DataManager): Instance of DataManager for managing data related to grass yield.
+        geo_fertiliser_class (Fertilisation): Instance of Fertilisation for handling geo-specific fertilization data.
+        grass_yield_class (GrasslandYield): Instance of Yield class from the grassland_production lib.
+        loader_class (Loader): Instance of Loader to load various necessary datasets.
+        calibration_year (int): The base year for data calibration and historical reference.
+        target_year (int): The target year for future scenario projections.
+        soil_class_yield_gap (dict): A dictionary mapping soil types to their respective yield gaps.
+        soil_class_prop (DataFrame): A DataFrame indicating the proportion of different soil types across scenarios.
+
+    Methods:
+        get_clover_parameters():
+            Retrieves clover parameters, such as proportion and fertilization rate, for each scenario, differentiating between 
+            conventional yield response curves and clover-grass systems.
+
+        get_yield():
+            Calculates the grass yield per hectare for each grassland type, farm system, and scenario. This method takes into 
+            account various factors including fertilization rates, soil properties, and clover parameters.
+
+        _yield_response_function_to_fertilizer(fertilizer, grassland, clover_prop=0, clover_fert=0, manure_spread=0):
+            An internal method that models the yield response to various factors including fertilizer application, clover proportion,
+            and organic manure spread. This function is critical in determining the yield per hectare under different scenarios.
+
+    Note:
+        This class is part of a broader framework aimed at understanding and optimizing grassland production. It should be used 
+        in conjunction with other related classes to gain a holistic view of the agricultural systems under study.
     """
-        The Yield class is dedicated to calculating grass yield per hectare for different farm systems (dairy, beef, 
-        sheep) under various scenarios. It considers the impact of fertilization (both inorganic and organic), 
-        clover proportion, soil types, and other factors on grass yield.
-
-        Args:
-            ef_country (str): The country for which the analysis is performed.
-            calibration_year (int): The calibration year.
-            target_year (int): The target year for future scenario projections.
-            scenario_inputs_df (DataFrame): DataFrame containing scenario input variables data.
-            scenario_animals_df (DataFrame): DataFrame containing scenario animal data.
-            baseline_animals_df (DataFrame): DataFrame containing baseline animal data.
-
-        Attributes:
-            sc_class (ScenarioDataFetcher): Instance of ScenarioDataFetcher for fetching scenario data.
-            scenario_list (list): List of scenarios.
-            data_manager_class (DataManager): Instance of DataManager for managing data related to yield.
-            fertiliser_class (Fertilisation): Instance of Fertilisation for handling fertilization-related data.
-            loader_class (Loader): Instance of Loader to load various datasets.
-            calibration_year (int): The base year for data calibration.
-            target_year (int): The target year for future scenario projections.
-            soil_class_yield_gap (dict): A dictionary mapping soil types to yield gaps.
-            soil_class_prop (DataFrame): A DataFrame indicating the proportion of different soil types.
-
-        Methods:
-            get_clover_parameters():
-                Defines clover proportion and rate for different scenarios to differentiate between conventional 
-                yield response curves and clover-grass systems.
-
-            get_yield():
-                Calculates the yield per hectare for each grassland type, farm system, and scenario.
-
-            _yield_response_function_to_fertilizer():
-                Internal method to model the yield response to fertilizer application.
-        """
     def __init__(
         self,
         ef_country,
         calibration_year,
         target_year,
         scenario_data,
         scenario_animals_df,
         baseline_animals_df,
     ):
-        self.sc_class = ScenarioDataFetcher(scenario_data)
-        self.scenario_list = self.sc_class.get_scenario_list()
 
-        self.data_manager_class = DataManager(
-            calibration_year,
-            target_year,
-            scenario_animals_df,
-            baseline_animals_df,
-        )
-        self.fertiliser_class = Fertilisation(
+        fertiliser_class = GeoFertilisation(
             ef_country,
             calibration_year,
             target_year,
             scenario_data,
             scenario_animals_df,
             baseline_animals_df,
         )
-        self.loader_class = Loader()
-        self.calibration_year = self.data_manager_class.get_calibration_year()
-        self.target_year = self.data_manager_class.get_target_year()
-
-        self.soil_class_yield_gap = self.data_manager_class.get_yield_gap()
 
-        self.soil_class_prop = self.data_manager_class.get_soil_properties()
+        self.grass_yield_class = Yield(ef_country,
+                        calibration_year,
+                        target_year,
+                        scenario_data,
+                        scenario_animals_df,
+                        baseline_animals_df,
+                        fertiliser_class=fertiliser_class
+                        )
+        
 
 
     def get_clover_parameters(self):
         """
         Defines clover proportion and rate for each scenario, differentiating between conventional
         yield response curves and clover-grass systems. This method considers scenarios for dairy,
         beef, and sheep farm systems with specific manure management practices.
@@ -103,51 +103,20 @@
             dict: A dictionary containing clover parameters for different scenarios and farm systems.
 
         The clover parameters include:
             - Clover proportion: The proportion of clover in the pasture.
             - Clover fertilisation rate: The rate of clover fertilisation.
 
         """
-        scenario_df = self.sc_class.get_scenario_dataframe()
-
-        keys = ["dairy", "beef", "sheep"]
-        inner_keys = ["proportion", "fertilisation"]
-
-        clover_dict = {key: {inner_key: {} for inner_key in inner_keys} for key in keys}
-
-        conditions = {
-            "dairy": (
-                    (scenario_df["Cattle systems"] == "Dairy")
-                    & (scenario_df["Manure management"] == "tank liquid")
-            ),
-            "beef": (
-                    (scenario_df["Cattle systems"] == "Beef")
-                    & (scenario_df["Manure management"] == "tank liquid")
-            ),
-            "sheep": (
-                    (scenario_df["Cattle systems"] == "Lowland sheep")
-                    & (scenario_df["Manure management"] == "solid")
-            )
-        }
-
-        for key in keys:
-            for sc in scenario_df["Scenarios"].unique():
-                mask = (scenario_df["Scenarios"] == sc) & conditions[key]
-                clover_proportion = self.sc_class.get_clover_proportion_value(mask)
-                clover_fertilisation = self.sc_class.get_clover_fertilisation_value(mask)
-                clover_dict[key]["proportion"][sc] = clover_proportion
-                clover_dict[key]["fertilisation"][sc] = clover_fertilisation
-
-
-        return clover_dict
+        return self.grass_yield_class.get_clover_parameters()
        
 
     def get_yield(self):
         """
-        Calculates the yield per hectare for different scenarios and farm systems based on fertilization and other factors.
+        Calculates the yield per hectare for different scenarios and farm systems for the catchment based on fertilization and other factors.
         The method computes yield values for dairy, beef, and sheep farm systems under various scenarios.
 
         The method utilizes information on fertilization rates, organic manure spread, soil properties, and clover parameters
         to calculate yields for each scenario and farm system. It iterates through different combinations of scenarios,
         farm systems, grassland types, and soil groups to compute yields.
 
         Returns:
@@ -155,81 +124,15 @@
             - Keys: Farm system types ("dairy," "beef," "sheep").
             - Values: Nested dictionaries, where each inner dictionary represents a scenario with the following structure:
                 - Keys: Scenario names.
                 - Values: Pandas DataFrames containing yield values for different grassland types (e.g., "Pasture," "Grass silage").
                     - The DataFrame's rows correspond to grassland types.
                     - The DataFrame's columns correspond to calibration and target years.
         """
-        fertilization_by_system_data_frame = (
-            self.loader_class.grassland_fertilization_by_system()
-        )
-        fert_rate = self.fertiliser_class.compute_inorganic_fertilization_rate()
-        organic_manure = self.fertiliser_class.organic_fertilisation_per_ha()
-
-        year_list = [self.calibration_year, self.target_year]
-        scenario_list = self.scenario_list
-
-        clover_parameters_dict = self.get_clover_parameters()
-
-        keys = ["dairy", "beef", "sheep"]
-
-        yield_per_ha = {
-            farm_type: {
-                sc: pd.DataFrame(
-                    0.0,
-                    index=fertilization_by_system_data_frame.index.levels[0],
-                    columns=year_list,
-                )
-                for sc in scenario_list
-            }
-            for farm_type in keys
-        }
-
-        for sc, farm_type, grassland_type, soil_group in product(
-            scenario_list,
-            keys,
-            fertilization_by_system_data_frame.index.levels[0],
-            self.soil_class_yield_gap.keys(),
-        ):
-            yield_per_ha_df = yield_per_ha[farm_type][sc]
-            soil_class_prop = self.soil_class_prop[farm_type].loc[
-                int(self.calibration_year), soil_group
-            ]
-
-            yield_per_ha_df.loc[grassland_type, int(self.calibration_year)] += (
-                self._yield_response_function_to_fertilizer(
-                    fert_rate[farm_type][sc].loc[
-                        grassland_type, str(self.calibration_year)
-                    ],
-                    grassland_type,
-                    manure_spread=organic_manure[sc].loc[int(self.calibration_year), farm_type],
-                )
-                * self.soil_class_yield_gap[soil_group]
-            ) * soil_class_prop
-
-            clover_prop = clover_parameters_dict[farm_type]["proportion"][sc]
-            clover_fert = clover_parameters_dict[farm_type]["fertilisation"][sc]
-
-            yield_per_ha_df.loc[grassland_type, int(self.target_year)] += (
-                self._yield_response_function_to_fertilizer(
-                    fert_rate[farm_type][sc].loc[grassland_type, str(self.target_year)],
-                    grassland_type,
-                    clover_prop=clover_prop,
-                    clover_fert=clover_fert,
-                    manure_spread=organic_manure[sc].loc[int(self.target_year), farm_type],
-                )
-                * self.soil_class_yield_gap[soil_group]
-            ) * soil_class_prop
-
-        transposed_yield_per_ha = {
-            sc: {farm_type: yield_per_ha[farm_type][sc].T for farm_type in keys}
-            for sc in scenario_list
-        }
-
-        return transposed_yield_per_ha
+        return self.grass_yield_class.get_yield()
 
 
     def _yield_response_function_to_fertilizer(
         self, fertilizer, grassland, clover_prop=0, clover_fert=0, manure_spread=0
     ):
         """
         Calculate the yield response to fertilizer application based on the specified parameters.
@@ -251,25 +154,8 @@
         Returns:
             float: The estimated yield response to the specified fertilizer application (in metric tons per hectare).
 
 
         Note: The result is converted to metric tons per hectare using the factor 1e-3.
 
         """
-
-        kg_to_t = 1e-3
-        if grassland == "Grass silage" or grassland == "Pasture":
-         
-            yield_response_default = ((-0.0444 * ((fertilizer + manure_spread) ** 2)
-                + 38.419 * (fertilizer + manure_spread)
-                + 6257) * (1 - clover_prop)) 
-            
-            yield_response_clover = (0.7056 * (clover_fert + manure_spread) + 12829) * clover_prop
-
-            yield_response = yield_response_default + yield_response_clover
-
-        else:
-            yield_response = -0.0444 * (fertilizer**2) + 38.419 * fertilizer + 6257
-
-        yield_response = yield_response * kg_to_t
-
-        return yield_response
+        return self.grass_yield_class._yield_response_function_to_fertilizer(fertilizer, grassland, clover_prop, clover_fert, manure_spread)
```

### Comparing `grassland_production-0.3.4/src/grassland_production/grassland_area.py` & `grassland_production-0.3.5/src/grassland_production/grassland_area.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 =======================
 Grassland Area Module
 =======================
 The Grassland Area Module is a part of the grassland production system that deals with calculating and managing 
 the proportions and distributions of grassland areas within different farming systems. 
 It is designed to provide essential data for grassland production analysis, taking into account various factors and scenarios.
 """
-
 import pandas as pd
 from itertools import product
 from grassland_production.resource_manager.data_loader import Loader
 
 
 class Areas:
     """
```

### Comparing `grassland_production-0.3.4/src/grassland_production/grassland_output.py` & `grassland_production-0.3.5/src/grassland_production/grassland_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 soil groups, dry matter production, and stocking rates, to provide easy retrieval of grassland
 scenario results.
 
 Classes:
     GrasslandOutput: Manages and computes outputs for grassland management.
 
 """
-
 from grassland_production.spared_area import Grasslands
 from grassland_production.farm_data_generation import FarmData
 from grassland_production.grassland_soils import SoilGroups
 from grassland_production.dry_matter import DryMatter
 from grassland_production.stocking_rate import StockingRate
 
 import pandas as pd
```

### Comparing `grassland_production-0.3.4/src/grassland_production/resource_manager/data_loader.py` & `grassland_production-0.3.5/src/grassland_production/resource_manager/data_loader.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.4/src/grassland_production/resource_manager/database_manager.py` & `grassland_production-0.3.5/src/grassland_production/resource_manager/database_manager.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.4/src/grassland_production/resource_manager/grassland_data_manager.py` & `grassland_production-0.3.5/src/grassland_production/resource_manager/grassland_data_manager.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.4/src/grassland_production/resource_manager/scenario_data_fetcher.py` & `grassland_production-0.3.5/src/grassland_production/resource_manager/scenario_data_fetcher.py`

 * *Files identical despite different names*

### Comparing `grassland_production-0.3.4/src/grassland_production/stocking_rate.py` & `grassland_production-0.3.5/src/grassland_production/stocking_rate.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 the livestock units and stocking rates for various farm types and scenarios. This class is 
 part of the grassland_production package and utilizes other components within the package 
 to analyze and compute essential data related to livestock management.
 
 Classes:
     StockingRate: Manages livestock units and stocking rates.
 """
-
 import pandas as pd
 import itertools
 from grassland_production.resource_manager.data_loader import Loader
 from grassland_production.resource_manager.grassland_data_manager import DataManager
 from grassland_production.resource_manager.scenario_data_fetcher import ScenarioDataFetcher
 from grassland_production.spared_area import Grasslands
 
@@ -31,14 +30,16 @@
     Args:
         ef_country (str): The country for which the analysis is performed.
         calibration_year (int): The calibration year.
         target_year (int): The target year for future scenario projections.
         scenario_inputs_df (DataFrame): DataFrame containing scenario input variables data.
         scenario_animals_df (DataFrame): DataFrame containing scenario animal data.
         baseline_animals_df (DataFrame): DataFrame containing baseline animal data.
+        grassland_class (Grasslands, optional): An instance of the Grassland class. If not 
+            provided, a new instance is created with default parameters.
         
     Attributes:
         sc_class (ScenarioDataFetcher): Fetches scenario data.
         scenario_list (list): List of scenarios.
         data_manager_class (DataManager): Manages and processes grassland and livestock data.
         calibration_year (int): Year of data calibration.
         target_year (int): Target year for data analysis.
@@ -49,25 +50,40 @@
 
     Methods:
         get_livestock_units_past(): Calculates livestock units for past scenarios based on baseline data.
         get_livestock_units_future(): Calculates livestock units for future scenarios.
         get_livestock_units(): Aggregates livestock units for past and future scenarios.
         get_stocking_rate(): Computes stocking rates for different farm types and scenarios.
     """
-    def __init__(self,ef_country, calibration_year, target_year, scenario_data, scenario_animals_df,baseline_animals_df):
+    def __init__(self,
+                 ef_country, 
+                 calibration_year, 
+                 target_year, 
+                 scenario_data, 
+                 scenario_animals_df,
+                 baseline_animals_df,
+                 grassland_class = None):
+        
         self.sc_class = ScenarioDataFetcher(scenario_data)
         self.scenario_list = self.sc_class.get_scenario_list()
         self.data_manager_class = DataManager(calibration_year, target_year, scenario_animals_df,baseline_animals_df)
         self.calibration_year = self.data_manager_class.get_calibration_year()
         self.target_year = self.data_manager_class.get_target_year()
         self.default_calibration_year = self.data_manager_class.get_default_calibration_year()
         self.loader_class = Loader()
         self.livestock_unit_values = self.loader_class.livestock_units()
-        self.grassland_class = Grasslands(ef_country, calibration_year, target_year, scenario_data, scenario_animals_df,baseline_animals_df)
-
+        if grassland_class is None:
+            self.grassland_class = Grasslands(ef_country,
+                                              calibration_year,
+                                              target_year,
+                                              scenario_data,
+                                              scenario_animals_df,
+                                              baseline_animals_df)
+        else:
+            self.grassland_class = grassland_class
 
     def get_livestock_units_past(self):
         """
         Calculates and returns the livestock units for the baseline scenario for each farm type.
 
         This method processes the baseline data to compute the livestock units present on dairy, beef, 
         and sheep farm types for the calibration year. It takes into account the different types of animals
```

### Comparing `grassland_production-0.3.4/src/grassland_production/utilisation_rate.py` & `grassland_production-0.3.5/src/grassland_production/utilisation_rate.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,17 @@
     Args:
         ef_country (str): The country for which the analysis is performed.
         calibration_year (int): The calibration year.
         target_year (int): The target year for future scenario projections.
         scenario_inputs_df (DataFrame): DataFrame containing scenario input variables data.
         scenario_animals_df (DataFrame): DataFrame containing scenario animal data.
         baseline_animals_df (DataFrame): DataFrame containing baseline animal data.
+        yield_class (Yield, optional): An instance of the Yield class. If not provided, a new instance is created with default parameters.
+        fertilisation_class (Fertilisation, optional): An instance of the Fertilisation class. If not provided, a new instance is created with default parameters.
+        dry_matter_class (DryMatter, optional): An instance of the DryMatter class. If not provided, a new instance is created with default parameters.
 
     Attributes:
         sc_class (ScenarioDataFetcher): Fetches scenario data.
         scenario_list (list): List of scenarios.
         data_manager_class (DataManager): Manages and processes grassland and livestock data.
         calibration_year (int): Year of data calibration.
         target_year (int): Target year for data analysis.
@@ -67,55 +70,71 @@
         self,
         ef_country,
         calibration_year,
         target_year,
         scenario_data,
         scenario_animals_df,
         baseline_animals_df,
+        yield_class=None,
+        fertilisation_class=None,
+        dry_matter_class=None,
     ):
         self.sc_class = ScenarioDataFetcher(scenario_data)
         self.scenario_list = self.sc_class.get_scenario_list()
 
         self.data_manager_class = DataManager(
             calibration_year,
             target_year,
             scenario_animals_df,
             baseline_animals_df,
         )
         self.calibration_year = self.data_manager_class.get_calibration_year()
         self.target_year = self.data_manager_class.get_target_year()
         self.default_calibration_year = self.data_manager_class.get_default_calibration_year()
-        self.yield_class = Yield(
-            ef_country,
-            calibration_year,
-            target_year,
-            scenario_data,
-            scenario_animals_df,
-            baseline_animals_df,
-        )
+
+        if yield_class is None:
+
+            self.yield_class = Yield(
+                ef_country,
+                calibration_year,
+                target_year,
+                scenario_data,
+                scenario_animals_df,
+                baseline_animals_df,
+            )
+        else:
+            self.yield_class = yield_class
+
         self.areas_class = Areas(
             target_year, calibration_year, self.default_calibration_year
         )
-        self.fertiliser_class = Fertilisation(
-            ef_country,
-            calibration_year,
-            target_year,
-            scenario_data,
-            scenario_animals_df,
-            baseline_animals_df,
-        )
 
-        self.dm_class = DryMatter(
-            ef_country,
-            calibration_year,
-            target_year,
-            scenario_data,
-            scenario_animals_df,
-            baseline_animals_df,
-        )
+        if fertilisation_class is None:
+            self.fertiliser_class = Fertilisation(
+                ef_country,
+                calibration_year,
+                target_year,
+                scenario_data,
+                scenario_animals_df,
+                baseline_animals_df,
+            )
+        else:
+            self.fertiliser_class = fertilisation_class
+
+        if dry_matter_class is None:
+            self.dm_class = DryMatter(
+                ef_country,
+                calibration_year,
+                target_year,
+                scenario_data,
+                scenario_animals_df,
+                baseline_animals_df,
+            )
+        else:
+            self.dm_class = dry_matter_class
 
         self.loader_class = Loader()
         self.cattle_grass_feed_class = cattle_lca.GrassFeed(ef_country)
         self.sheep_grass_feed_class = sheep_lca.GrassFeed(ef_country)
         self.concentrate_feed_class = cattle_lca.Energy(ef_country)
         self.sheep_concentrate_feed_class = sheep_lca.Energy(ef_country)
```

### Comparing `grassland_production-0.3.4/PKG-INFO` & `grassland_production-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grassland_production
-Version: 0.3.4
+Version: 0.3.5
 Summary: Computation of grassland area and production based on animal energy calculations and grassland inputs
 License: MIT
 Author: Colm Duffy
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```


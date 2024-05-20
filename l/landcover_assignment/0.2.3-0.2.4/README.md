# Comparing `tmp/landcover_assignment-0.2.3.tar.gz` & `tmp/landcover_assignment-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landcover_assignment-0.2.3.tar", max compression
+gzip compressed data, was "landcover_assignment-0.2.4.tar", max compression
```

## Comparing `landcover_assignment-0.2.3.tar` & `landcover_assignment-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1088 2023-05-25 19:51:14.000000 landcover_assignment-0.2.3/LICENSE
--rw-r--r--   0        0        0     5207 2024-04-29 07:30:36.759766 landcover_assignment-0.2.3/README.md
--rw-r--r--   0        0        0      479 2024-05-14 07:59:52.528765 landcover_assignment-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-21 12:33:17.659500 landcover_assignment-0.2.3/src/landcover_assignment/__init__.py
--rw-r--r--   0        0        0     7671 2024-02-21 12:33:17.659500 landcover_assignment-0.2.3/src/landcover_assignment/afforestation.py
--rw-r--r--   0        0        0      222 2024-02-21 12:33:17.659500 landcover_assignment-0.2.3/src/landcover_assignment/database/__init__.py
--rw-r--r--   0        0        0   102400 2024-04-29 07:30:36.775766 landcover_assignment-0.2.3/src/landcover_assignment/database/land_use_database.db
--rw-r--r--   0        0        0    10270 2024-02-21 12:33:17.659500 landcover_assignment-0.2.3/src/landcover_assignment/distribution.py
--rw-r--r--   0        0        0        0 2024-02-21 12:33:17.659500 landcover_assignment-0.2.3/src/landcover_assignment/geo_landcover_assignment/__init__.py
--rw-r--r--   0        0        0    26151 2024-05-13 10:41:12.665489 landcover_assignment-0.2.3/src/landcover_assignment/geo_landcover_assignment/catchment_landcover.py
--rw-r--r--   0        0        0     7652 2024-02-21 12:33:17.659500 landcover_assignment-0.2.3/src/landcover_assignment/geo_landcover_assignment/geo_afforestation.py
--rw-r--r--   0        0        0     9690 2024-02-21 12:33:17.659500 landcover_assignment-0.2.3/src/landcover_assignment/geo_landcover_assignment/geo_distribution.py
--rw-r--r--   0        0        0    20183 2024-02-21 12:33:17.659500 landcover_assignment-0.2.3/src/landcover_assignment/geo_landcover_assignment/geo_landcover.py
--rw-r--r--   0        0        0     8483 2024-02-21 12:33:17.659500 landcover_assignment-0.2.3/src/landcover_assignment/geo_landcover_assignment/geo_transition_matrix.py
--rw-r--r--   0        0        0    22423 2024-02-21 12:33:17.659500 landcover_assignment-0.2.3/src/landcover_assignment/landcover.py
--rw-r--r--   0        0        0     4390 2024-02-21 12:33:17.663500 landcover_assignment-0.2.3/src/landcover_assignment/landcover_data_manager.py
--rw-r--r--   0        0        0    31010 2024-02-21 12:33:17.663500 landcover_assignment-0.2.3/src/landcover_assignment/national_landcover.py
--rw-r--r--   0        0        0        0 2024-02-21 12:33:17.663500 landcover_assignment-0.2.3/src/landcover_assignment/resource_manager/__init__.py
--rw-r--r--   0        0        0     3516 2024-02-21 12:33:17.663500 landcover_assignment-0.2.3/src/landcover_assignment/resource_manager/data_loader.py
--rw-r--r--   0        0        0     5746 2024-02-21 12:33:17.663500 landcover_assignment-0.2.3/src/landcover_assignment/resource_manager/database_manager.py
--rw-r--r--   0        0        0     5994 2024-02-21 12:33:17.663500 landcover_assignment-0.2.3/src/landcover_assignment/resource_manager/scenario_data_fetcher.py
--rw-r--r--   0        0        0    17134 2024-02-21 12:33:17.663500 landcover_assignment-0.2.3/src/landcover_assignment/resource_manager/transition_data_fetcher.py
--rw-r--r--   0        0        0     8034 2024-02-12 13:07:15.410030 landcover_assignment-0.2.3/src/landcover_assignment/transition_matrix.py
--rw-r--r--   0        0        0     5842 1970-01-01 00:00:00.000000 landcover_assignment-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-25 19:51:14.000000 landcover_assignment-0.2.4/LICENSE
+-rw-r--r--   0        0        0     5207 2024-04-29 07:30:36.759766 landcover_assignment-0.2.4/README.md
+-rw-r--r--   0        0        0      479 2024-05-20 07:50:57.119742 landcover_assignment-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-21 12:33:17.659500 landcover_assignment-0.2.4/src/landcover_assignment/__init__.py
+-rw-r--r--   0        0        0     7671 2024-02-21 12:33:17.659500 landcover_assignment-0.2.4/src/landcover_assignment/afforestation.py
+-rw-r--r--   0        0        0      222 2024-02-21 12:33:17.659500 landcover_assignment-0.2.4/src/landcover_assignment/database/__init__.py
+-rw-r--r--   0        0        0   102400 2024-04-29 07:30:36.775766 landcover_assignment-0.2.4/src/landcover_assignment/database/land_use_database.db
+-rw-r--r--   0        0        0    10270 2024-02-21 12:33:17.659500 landcover_assignment-0.2.4/src/landcover_assignment/distribution.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:33:17.659500 landcover_assignment-0.2.4/src/landcover_assignment/geo_landcover_assignment/__init__.py
+-rw-r--r--   0        0        0    26174 2024-05-20 07:50:57.119742 landcover_assignment-0.2.4/src/landcover_assignment/geo_landcover_assignment/catchment_landcover.py
+-rw-r--r--   0        0        0     7652 2024-02-21 12:33:17.659500 landcover_assignment-0.2.4/src/landcover_assignment/geo_landcover_assignment/geo_afforestation.py
+-rw-r--r--   0        0        0     9690 2024-02-21 12:33:17.659500 landcover_assignment-0.2.4/src/landcover_assignment/geo_landcover_assignment/geo_distribution.py
+-rw-r--r--   0        0        0    20183 2024-02-21 12:33:17.659500 landcover_assignment-0.2.4/src/landcover_assignment/geo_landcover_assignment/geo_landcover.py
+-rw-r--r--   0        0        0     8483 2024-02-21 12:33:17.659500 landcover_assignment-0.2.4/src/landcover_assignment/geo_landcover_assignment/geo_transition_matrix.py
+-rw-r--r--   0        0        0    22423 2024-02-21 12:33:17.659500 landcover_assignment-0.2.4/src/landcover_assignment/landcover.py
+-rw-r--r--   0        0        0     4390 2024-02-21 12:33:17.663500 landcover_assignment-0.2.4/src/landcover_assignment/landcover_data_manager.py
+-rw-r--r--   0        0        0    31010 2024-02-21 12:33:17.663500 landcover_assignment-0.2.4/src/landcover_assignment/national_landcover.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:33:17.663500 landcover_assignment-0.2.4/src/landcover_assignment/resource_manager/__init__.py
+-rw-r--r--   0        0        0     3516 2024-02-21 12:33:17.663500 landcover_assignment-0.2.4/src/landcover_assignment/resource_manager/data_loader.py
+-rw-r--r--   0        0        0     5746 2024-02-21 12:33:17.663500 landcover_assignment-0.2.4/src/landcover_assignment/resource_manager/database_manager.py
+-rw-r--r--   0        0        0     5994 2024-02-21 12:33:17.663500 landcover_assignment-0.2.4/src/landcover_assignment/resource_manager/scenario_data_fetcher.py
+-rw-r--r--   0        0        0    17134 2024-02-21 12:33:17.663500 landcover_assignment-0.2.4/src/landcover_assignment/resource_manager/transition_data_fetcher.py
+-rw-r--r--   0        0        0     8034 2024-02-12 13:07:15.410030 landcover_assignment-0.2.4/src/landcover_assignment/transition_matrix.py
+-rw-r--r--   0        0        0     5842 1970-01-01 00:00:00.000000 landcover_assignment-0.2.4/PKG-INFO
```

### Comparing `landcover_assignment-0.2.3/LICENSE` & `landcover_assignment-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.3/README.md` & `landcover_assignment-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.3/src/landcover_assignment/afforestation.py` & `landcover_assignment-0.2.4/src/landcover_assignment/afforestation.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.3/src/landcover_assignment/database/land_use_database.db` & `landcover_assignment-0.2.4/src/landcover_assignment/database/land_use_database.db`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.3/src/landcover_assignment/distribution.py` & `landcover_assignment-0.2.4/src/landcover_assignment/distribution.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.3/src/landcover_assignment/geo_landcover_assignment/catchment_landcover.py` & `landcover_assignment-0.2.4/src/landcover_assignment/geo_landcover_assignment/catchment_landcover.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
                 'share_organic': 0,
                 'share_organic_mineral': 0,
                 'share_burnt': 0  # Assuming a default value; replace with an appropriate call if needed
             }
             return pd.DataFrame([summary_data])
 
         # Filter for specific types of forests and then group
-        forest_types = ['Broadleaved Forest and Woodland', 'Coniferous Forest', 'Mixed Forest']
+        forest_types = ['Broadleaved Forest and Woodland', 'Coniferous Forest', 'Mixed Forest', 'Transitional Forest']
         filtered_df = forest_df[forest_df['cover_type'].isin(forest_types)]
         grouped_df = filtered_df.groupby(['cover_type', 'soil_type']).sum()
 
         # Safely get totals for different soil types, using 0 if the category is missing
         total_area = grouped_df['total_hectares'].sum()
         total_mineral = grouped_df.xs('mineral', level='soil_type')['total_hectares'].sum() if 'mineral' in grouped_df.index.get_level_values('soil_type') else 0
         total_mineral += grouped_df.xs('misc', level='soil_type')['total_hectares'].sum() if 'misc' in grouped_df.index.get_level_values('soil_type') else 0
```

### Comparing `landcover_assignment-0.2.3/src/landcover_assignment/geo_landcover_assignment/geo_afforestation.py` & `landcover_assignment-0.2.4/src/landcover_assignment/geo_landcover_assignment/geo_afforestation.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.3/src/landcover_assignment/geo_landcover_assignment/geo_distribution.py` & `landcover_assignment-0.2.4/src/landcover_assignment/geo_landcover_assignment/geo_distribution.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.3/src/landcover_assignment/geo_landcover_assignment/geo_landcover.py` & `landcover_assignment-0.2.4/src/landcover_assignment/geo_landcover_assignment/geo_landcover.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.3/src/landcover_assignment/geo_landcover_assignment/geo_transition_matrix.py` & `landcover_assignment-0.2.4/src/landcover_assignment/geo_landcover_assignment/geo_transition_matrix.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.3/src/landcover_assignment/landcover.py` & `landcover_assignment-0.2.4/src/landcover_assignment/landcover.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.3/src/landcover_assignment/landcover_data_manager.py` & `landcover_assignment-0.2.4/src/landcover_assignment/landcover_data_manager.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.3/src/landcover_assignment/national_landcover.py` & `landcover_assignment-0.2.4/src/landcover_assignment/national_landcover.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.3/src/landcover_assignment/resource_manager/data_loader.py` & `landcover_assignment-0.2.4/src/landcover_assignment/resource_manager/data_loader.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.3/src/landcover_assignment/resource_manager/database_manager.py` & `landcover_assignment-0.2.4/src/landcover_assignment/resource_manager/database_manager.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.3/src/landcover_assignment/resource_manager/scenario_data_fetcher.py` & `landcover_assignment-0.2.4/src/landcover_assignment/resource_manager/scenario_data_fetcher.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.3/src/landcover_assignment/resource_manager/transition_data_fetcher.py` & `landcover_assignment-0.2.4/src/landcover_assignment/resource_manager/transition_data_fetcher.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.3/src/landcover_assignment/transition_matrix.py` & `landcover_assignment-0.2.4/src/landcover_assignment/transition_matrix.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.3/PKG-INFO` & `landcover_assignment-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landcover_assignment
-Version: 0.2.3
+Version: 0.2.4
 Summary: A goblin tool for the generation of areas of alternative land uses based on spared area available
 License: MIT
 Author: Colm Duffy
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```


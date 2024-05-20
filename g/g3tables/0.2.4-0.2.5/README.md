# Comparing `tmp/g3tables-0.2.4.tar.gz` & `tmp/g3tables-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g3tables-0.2.4.tar", last modified: Fri May 17 06:51:40 2024, max compression
+gzip compressed data, was "g3tables-0.2.5.tar", last modified: Mon May 20 14:17:00 2024, max compression
```

## Comparing `g3tables-0.2.4.tar` & `g3tables-0.2.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.027411 g3tables-0.2.4/
--rw-rw-rw-   0        0        0     1091 2024-04-29 08:48:33.000000 g3tables-0.2.4/LICENCE
--rw-rw-rw-   0        0        0     1325 2024-05-17 06:51:40.026394 g3tables-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       81 2024-04-29 08:48:33.000000 g3tables-0.2.4/README.md
--rw-rw-rw-   0        0        0     1679 2024-05-17 06:30:23.000000 g3tables-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 06:51:40.027411 g3tables-0.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:39.944073 g3tables-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:39.958897 g3tables-0.2.4/src/g3tables/
--rw-rw-rw-   0        0        0      550 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:39.974540 g3tables-0.2.4/src/g3tables/plc_composition_io_table/
--rw-rw-rw-   0        0        0      361 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/plc_composition_io_table/__init__.py
--rw-rw-rw-   0        0        0    14539 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/plc_composition_io_table/_extend_table.py
--rw-rw-rw-   0        0        0    21360 2024-04-30 11:02:43.000000 g3tables-0.2.4/src/g3tables/plc_composition_io_table/_table.py
--rw-rw-rw-   0        0        0     5780 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/plc_composition_io_table/io_signals.json
--rw-rw-rw-   0        0        0        0 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:39.974540 g3tables-0.2.4/src/g3tables/sw_definition_table/
--rw-rw-rw-   0        0        0      182 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/sw_definition_table/__init__.py
--rw-rw-rw-   0        0        0    54470 2024-05-16 21:09:28.000000 g3tables-0.2.4/src/g3tables/sw_definition_table/_table.py
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.005803 g3tables-0.2.4/src/g3tables/system_config/
--rw-rw-rw-   0        0        0      225 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/system_config/__init__.py
--rw-rw-rw-   0        0        0    15259 2024-05-13 09:37:18.000000 g3tables-0.2.4/src/g3tables/system_config/_cli.py
--rw-rw-rw-   0        0        0    22338 2024-04-30 11:02:43.000000 g3tables-0.2.4/src/g3tables/system_config/_g3core_updater.py
--rw-rw-rw-   0        0        0      972 2024-04-30 11:02:43.000000 g3tables-0.2.4/src/g3tables/system_config/_hw_connections.py
--rw-rw-rw-   0        0        0    12584 2024-05-17 06:27:59.000000 g3tables-0.2.4/src/g3tables/system_config/_iomap_updater.py
--rw-rw-rw-   0        0        0       74 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/system_config/_logger.py
--rw-rw-rw-   0        0        0     7323 2024-05-16 16:24:24.000000 g3tables-0.2.4/src/g3tables/system_config/_sw_system_dict_wrapper.py
--rw-rw-rw-   0        0        0     4132 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/system_config/_system_config_processor.py
--rw-rw-rw-   0        0        0     1192 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/system_config/type_hinting.py
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.005803 g3tables-0.2.4/src/g3tables/utils/
--rw-rw-rw-   0        0        0      146 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/utils/__init__.py
--rw-rw-rw-   0        0        0     1552 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/utils/_d2nd.py
--rw-rw-rw-   0        0        0     3706 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/utils/_interval.py
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.005803 g3tables-0.2.4/src/g3tables/utils/gdrive/
--rw-rw-rw-   0        0        0      365 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/utils/gdrive/__init__.py
--rw-rw-rw-   0        0        0     5172 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/utils/gdrive/_gdrive.py
--rw-rw-rw-   0        0        0     1263 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/utils/gdrive/_update_creds.py
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.021412 g3tables-0.2.4/src/g3tables/visualization_table/
--rw-rw-rw-   0        0        0      207 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/visualization_table/__init__.py
--rw-rw-rw-   0        0        0    14812 2024-05-16 16:24:45.000000 g3tables-0.2.4/src/g3tables/visualization_table/_table.py
-drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.021412 g3tables-0.2.4/src/g3tables.egg-info/
--rw-rw-rw-   0        0        0     1325 2024-05-17 06:51:39.000000 g3tables-0.2.4/src/g3tables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1290 2024-05-17 06:51:39.000000 g3tables-0.2.4/src/g3tables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 06:51:39.000000 g3tables-0.2.4/src/g3tables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      207 2024-05-17 06:51:39.000000 g3tables-0.2.4/src/g3tables.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2024-05-17 06:51:39.000000 g3tables-0.2.4/src/g3tables.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-17 06:51:39.000000 g3tables-0.2.4/src/g3tables.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 14:17:00.618146 g3tables-0.2.5/
+-rw-rw-rw-   0        0        0     1091 2024-04-29 08:48:33.000000 g3tables-0.2.5/LICENCE
+-rw-rw-rw-   0        0        0     1325 2024-05-20 14:17:00.618146 g3tables-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       81 2024-04-29 08:48:33.000000 g3tables-0.2.5/README.md
+-rw-rw-rw-   0        0        0     1679 2024-05-20 14:16:10.000000 g3tables-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 14:17:00.618146 g3tables-0.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 14:17:00.502219 g3tables-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-20 14:17:00.529431 g3tables-0.2.5/src/g3tables/
+-rw-rw-rw-   0        0        0      550 2024-04-29 08:48:33.000000 g3tables-0.2.5/src/g3tables/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:17:00.560715 g3tables-0.2.5/src/g3tables/plc_composition_io_table/
+-rw-rw-rw-   0        0        0      361 2024-04-29 08:48:33.000000 g3tables-0.2.5/src/g3tables/plc_composition_io_table/__init__.py
+-rw-rw-rw-   0        0        0    14539 2024-04-29 08:48:33.000000 g3tables-0.2.5/src/g3tables/plc_composition_io_table/_extend_table.py
+-rw-rw-rw-   0        0        0    21360 2024-04-30 11:02:43.000000 g3tables-0.2.5/src/g3tables/plc_composition_io_table/_table.py
+-rw-rw-rw-   0        0        0     5780 2024-04-29 08:48:33.000000 g3tables-0.2.5/src/g3tables/plc_composition_io_table/io_signals.json
+-rw-rw-rw-   0        0        0        0 2024-04-29 08:48:33.000000 g3tables-0.2.5/src/g3tables/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-20 14:17:00.571224 g3tables-0.2.5/src/g3tables/sw_definition_table/
+-rw-rw-rw-   0        0        0      182 2024-04-29 08:48:33.000000 g3tables-0.2.5/src/g3tables/sw_definition_table/__init__.py
+-rw-rw-rw-   0        0        0    54470 2024-05-16 21:09:28.000000 g3tables-0.2.5/src/g3tables/sw_definition_table/_table.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:17:00.586874 g3tables-0.2.5/src/g3tables/system_config/
+-rw-rw-rw-   0        0        0      225 2024-04-29 08:48:33.000000 g3tables-0.2.5/src/g3tables/system_config/__init__.py
+-rw-rw-rw-   0        0        0    15259 2024-05-13 09:37:18.000000 g3tables-0.2.5/src/g3tables/system_config/_cli.py
+-rw-rw-rw-   0        0        0    22338 2024-04-30 11:02:43.000000 g3tables-0.2.5/src/g3tables/system_config/_g3core_updater.py
+-rw-rw-rw-   0        0        0      972 2024-04-30 11:02:43.000000 g3tables-0.2.5/src/g3tables/system_config/_hw_connections.py
+-rw-rw-rw-   0        0        0    12561 2024-05-20 13:50:33.000000 g3tables-0.2.5/src/g3tables/system_config/_iomap_updater.py
+-rw-rw-rw-   0        0        0       74 2024-04-29 08:48:33.000000 g3tables-0.2.5/src/g3tables/system_config/_logger.py
+-rw-rw-rw-   0        0        0     7323 2024-05-16 16:24:24.000000 g3tables-0.2.5/src/g3tables/system_config/_sw_system_dict_wrapper.py
+-rw-rw-rw-   0        0        0     4132 2024-04-29 08:48:33.000000 g3tables-0.2.5/src/g3tables/system_config/_system_config_processor.py
+-rw-rw-rw-   0        0        0     1192 2024-04-29 08:48:33.000000 g3tables-0.2.5/src/g3tables/system_config/type_hinting.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:17:00.602515 g3tables-0.2.5/src/g3tables/utils/
+-rw-rw-rw-   0        0        0      146 2024-04-29 08:48:33.000000 g3tables-0.2.5/src/g3tables/utils/__init__.py
+-rw-rw-rw-   0        0        0     1552 2024-04-29 08:48:33.000000 g3tables-0.2.5/src/g3tables/utils/_d2nd.py
+-rw-rw-rw-   0        0        0     3706 2024-04-29 08:48:33.000000 g3tables-0.2.5/src/g3tables/utils/_interval.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:17:00.602515 g3tables-0.2.5/src/g3tables/utils/gdrive/
+-rw-rw-rw-   0        0        0      365 2024-04-29 08:48:33.000000 g3tables-0.2.5/src/g3tables/utils/gdrive/__init__.py
+-rw-rw-rw-   0        0        0     5172 2024-04-29 08:48:33.000000 g3tables-0.2.5/src/g3tables/utils/gdrive/_gdrive.py
+-rw-rw-rw-   0        0        0     1263 2024-04-29 08:48:33.000000 g3tables-0.2.5/src/g3tables/utils/gdrive/_update_creds.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:17:00.602515 g3tables-0.2.5/src/g3tables/visualization_table/
+-rw-rw-rw-   0        0        0      207 2024-04-29 08:48:33.000000 g3tables-0.2.5/src/g3tables/visualization_table/__init__.py
+-rw-rw-rw-   0        0        0    14812 2024-05-16 16:24:45.000000 g3tables-0.2.5/src/g3tables/visualization_table/_table.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:17:00.602515 g3tables-0.2.5/src/g3tables.egg-info/
+-rw-rw-rw-   0        0        0     1325 2024-05-20 14:17:00.000000 g3tables-0.2.5/src/g3tables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1290 2024-05-20 14:17:00.000000 g3tables-0.2.5/src/g3tables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 14:17:00.000000 g3tables-0.2.5/src/g3tables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      207 2024-05-20 14:17:00.000000 g3tables-0.2.5/src/g3tables.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2024-05-20 14:17:00.000000 g3tables-0.2.5/src/g3tables.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-20 14:17:00.000000 g3tables-0.2.5/src/g3tables.egg-info/top_level.txt
```

### Comparing `g3tables-0.2.4/LICENCE` & `g3tables-0.2.5/LICENCE`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.4/PKG-INFO` & `g3tables-0.2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3tables
-Version: 0.2.4
+Version: 0.2.5
 Summary: G3 SW Definition, HW and PLC components, and Visualisation tables parser
 Author: Elektroline a.s.
 Project-URL: Homepage, https://gitlab.elektroline.cz/plc/systemg3-py/SystemG3Tables
 Keywords: Elektroline,Google Drive,Project table
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
```

### Comparing `g3tables-0.2.4/pyproject.toml` & `g3tables-0.2.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "g3tables"
-version = "0.2.4"
+version = "0.2.5"
 description = "G3 SW Definition, HW and PLC components, and Visualisation tables parser"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
   { name="Elektroline a.s." },
 ]
 classifiers = [
```

### Comparing `g3tables-0.2.4/src/g3tables/__init__.py` & `g3tables-0.2.5/src/g3tables/__init__.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.4/src/g3tables/plc_composition_io_table/_extend_table.py` & `g3tables-0.2.5/src/g3tables/plc_composition_io_table/_extend_table.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.4/src/g3tables/plc_composition_io_table/_table.py` & `g3tables-0.2.5/src/g3tables/plc_composition_io_table/_table.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.4/src/g3tables/plc_composition_io_table/io_signals.json` & `g3tables-0.2.5/src/g3tables/plc_composition_io_table/io_signals.json`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.4/src/g3tables/sw_definition_table/_table.py` & `g3tables-0.2.5/src/g3tables/sw_definition_table/_table.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.4/src/g3tables/system_config/_cli.py` & `g3tables-0.2.5/src/g3tables/system_config/_cli.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.4/src/g3tables/system_config/_g3core_updater.py` & `g3tables-0.2.5/src/g3tables/system_config/_g3core_updater.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.4/src/g3tables/system_config/_hw_connections.py` & `g3tables-0.2.5/src/g3tables/system_config/_hw_connections.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.4/src/g3tables/system_config/_iomap_updater.py` & `g3tables-0.2.5/src/g3tables/system_config/_iomap_updater.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     SWSystemDict
 )
 from ._sw_system_dict_wrapper import SWSystemDictWrapper
 from ._logger import logger
 
 
 class SWSystemDictControlIOMapUpdater:
-    EXCLUDED_FOR_SAFETY_IOMAP = ['Zone', 'Gate', 'Route']
+    EXCLUDED_FOR_SAFETY_IOMAP = []
 
     def __init__(
         self,
         system: SWSystemDict,
         iomap: dict[str, dict[str, str]] | None,
         sl8101_name: str | None,
         g3core: G3Core | None
```

### Comparing `g3tables-0.2.4/src/g3tables/system_config/_sw_system_dict_wrapper.py` & `g3tables-0.2.5/src/g3tables/system_config/_sw_system_dict_wrapper.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.4/src/g3tables/system_config/_system_config_processor.py` & `g3tables-0.2.5/src/g3tables/system_config/_system_config_processor.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.4/src/g3tables/system_config/type_hinting.py` & `g3tables-0.2.5/src/g3tables/system_config/type_hinting.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.4/src/g3tables/utils/_d2nd.py` & `g3tables-0.2.5/src/g3tables/utils/_d2nd.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.4/src/g3tables/utils/_interval.py` & `g3tables-0.2.5/src/g3tables/utils/_interval.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.4/src/g3tables/utils/gdrive/_gdrive.py` & `g3tables-0.2.5/src/g3tables/utils/gdrive/_gdrive.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.4/src/g3tables/utils/gdrive/_update_creds.py` & `g3tables-0.2.5/src/g3tables/utils/gdrive/_update_creds.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.4/src/g3tables/visualization_table/_table.py` & `g3tables-0.2.5/src/g3tables/visualization_table/_table.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.4/src/g3tables.egg-info/PKG-INFO` & `g3tables-0.2.5/src/g3tables.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3tables
-Version: 0.2.4
+Version: 0.2.5
 Summary: G3 SW Definition, HW and PLC components, and Visualisation tables parser
 Author: Elektroline a.s.
 Project-URL: Homepage, https://gitlab.elektroline.cz/plc/systemg3-py/SystemG3Tables
 Keywords: Elektroline,Google Drive,Project table
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
```

### Comparing `g3tables-0.2.4/src/g3tables.egg-info/SOURCES.txt` & `g3tables-0.2.5/src/g3tables.egg-info/SOURCES.txt`

 * *Files identical despite different names*


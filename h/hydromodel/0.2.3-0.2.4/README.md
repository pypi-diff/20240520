# Comparing `tmp/hydromodel-0.2.3.tar.gz` & `tmp/hydromodel-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydromodel-0.2.3.tar", last modified: Sun May 19 05:51:41 2024, max compression
+gzip compressed data, was "hydromodel-0.2.4.tar", last modified: Mon May 20 13:16:59 2024, max compression
```

## Comparing `hydromodel-0.2.3.tar` & `hydromodel-0.2.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:51:41.673990 hydromodel-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-19 05:51:33.000000 hydromodel-0.2.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 05:51:33.000000 hydromodel-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-19 05:51:33.000000 hydromodel-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-05-19 05:51:41.673990 hydromodel-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13005 2024-05-19 05:51:33.000000 hydromodel-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:51:41.669990 hydromodel-0.2.3/hydromodel/
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:51:41.673990 hydromodel-0.2.3/hydromodel/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17450 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/datasets/data_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/datasets/data_visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:51:41.673990 hydromodel-0.2.3/hydromodel/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/models/gr4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/models/hymod.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/models/model_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/models/model_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    32143 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/models/xaj.py
--rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/models/xaj_bmi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:51:41.673990 hydromodel-0.2.3/hydromodel/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/trainers/calibrate_ga.py
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/trainers/calibrate_sceua.py
--rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-05-19 05:51:33.000000 hydromodel-0.2.3/hydromodel/trainers/evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:51:41.669990 hydromodel-0.2.3/hydromodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-05-19 05:51:41.000000 hydromodel-0.2.3/hydromodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-19 05:51:41.000000 hydromodel-0.2.3/hydromodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-19 05:51:41.000000 hydromodel-0.2.3/hydromodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-19 05:51:41.000000 hydromodel-0.2.3/hydromodel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 05:51:41.000000 hydromodel-0.2.3/hydromodel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-19 05:51:41.000000 hydromodel-0.2.3/hydromodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 05:51:41.000000 hydromodel-0.2.3/hydromodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-19 05:51:33.000000 hydromodel-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-19 05:51:41.673990 hydromodel-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-19 05:51:33.000000 hydromodel-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:51:41.673990 hydromodel-0.2.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-19 05:51:33.000000 hydromodel-0.2.3/test/test_calibrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-05-19 05:51:33.000000 hydromodel-0.2.3/test/test_data_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-19 05:51:33.000000 hydromodel-0.2.3/test/test_data_visualize.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-19 05:51:33.000000 hydromodel-0.2.3/test/test_gr4j.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-19 05:51:33.000000 hydromodel-0.2.3/test/test_hymod.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-19 05:51:33.000000 hydromodel-0.2.3/test/test_show_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-19 05:51:33.000000 hydromodel-0.2.3/test/test_xaj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:16:59.293807 hydromodel-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-20 13:16:40.000000 hydromodel-0.2.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 13:16:40.000000 hydromodel-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-20 13:16:40.000000 hydromodel-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-05-20 13:16:59.293807 hydromodel-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13005 2024-05-20 13:16:40.000000 hydromodel-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:16:59.289807 hydromodel-0.2.4/hydromodel/
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-20 13:16:40.000000 hydromodel-0.2.4/hydromodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:16:59.289807 hydromodel-0.2.4/hydromodel/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-20 13:16:40.000000 hydromodel-0.2.4/hydromodel/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18008 2024-05-20 13:16:40.000000 hydromodel-0.2.4/hydromodel/datasets/data_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-05-20 13:16:40.000000 hydromodel-0.2.4/hydromodel/datasets/data_visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:16:59.289807 hydromodel-0.2.4/hydromodel/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:16:40.000000 hydromodel-0.2.4/hydromodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-05-20 13:16:40.000000 hydromodel-0.2.4/hydromodel/models/gr4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-20 13:16:40.000000 hydromodel-0.2.4/hydromodel/models/hymod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-20 13:16:40.000000 hydromodel-0.2.4/hydromodel/models/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-20 13:16:40.000000 hydromodel-0.2.4/hydromodel/models/model_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32143 2024-05-20 13:16:40.000000 hydromodel-0.2.4/hydromodel/models/xaj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-20 13:16:40.000000 hydromodel-0.2.4/hydromodel/models/xaj_bmi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:16:59.289807 hydromodel-0.2.4/hydromodel/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:16:40.000000 hydromodel-0.2.4/hydromodel/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-05-20 13:16:40.000000 hydromodel-0.2.4/hydromodel/trainers/calibrate_ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-05-20 13:16:40.000000 hydromodel-0.2.4/hydromodel/trainers/calibrate_sceua.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-05-20 13:16:40.000000 hydromodel-0.2.4/hydromodel/trainers/evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:16:59.289807 hydromodel-0.2.4/hydromodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-05-20 13:16:59.000000 hydromodel-0.2.4/hydromodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-20 13:16:59.000000 hydromodel-0.2.4/hydromodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-20 13:16:59.000000 hydromodel-0.2.4/hydromodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-20 13:16:59.000000 hydromodel-0.2.4/hydromodel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:16:59.000000 hydromodel-0.2.4/hydromodel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-20 13:16:59.000000 hydromodel-0.2.4/hydromodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 13:16:59.000000 hydromodel-0.2.4/hydromodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-20 13:16:40.000000 hydromodel-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-20 13:16:59.293807 hydromodel-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-20 13:16:40.000000 hydromodel-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:16:59.293807 hydromodel-0.2.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-20 13:16:40.000000 hydromodel-0.2.4/test/test_calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-05-20 13:16:40.000000 hydromodel-0.2.4/test/test_data_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-20 13:16:40.000000 hydromodel-0.2.4/test/test_data_visualize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-20 13:16:40.000000 hydromodel-0.2.4/test/test_gr4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-20 13:16:40.000000 hydromodel-0.2.4/test/test_hymod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-20 13:16:40.000000 hydromodel-0.2.4/test/test_show_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-20 13:16:40.000000 hydromodel-0.2.4/test/test_xaj.py
```

### Comparing `hydromodel-0.2.3/LICENSE` & `hydromodel-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hydromodel-0.2.3/PKG-INFO` & `hydromodel-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydromodel
-Version: 0.2.3
+Version: 0.2.4
 Summary: hydrological models starting from XinAnJiang
 Home-page: https://github.com/OuyangWenyu/hydromodel
 Author: Wenyu Ouyang
 Author-email: wenyuouyang@outlook.com
 License: GNU General Public License v3
 Keywords: hydromodel
 Classifier: Intended Audience :: Developers
```

### Comparing `hydromodel-0.2.3/README.md` & `hydromodel-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `hydromodel-0.2.3/hydromodel/__init__.py` & `hydromodel-0.2.4/hydromodel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import os
 from pathlib import Path
 from hydroutils import hydro_file
 import yaml
 
 __author__ = """Wenyu Ouyang"""
 __email__ = 'wenyuouyang@outlook.com'
-__version__ = '0.2.3'
+__version__ = '0.2.4'
 
 
 CACHE_DIR = hydro_file.get_cache_dir()
 SETTING_FILE = os.path.join(Path.home(), "hydro_setting.yml")
 
 
 def read_setting(setting_path):
```

### Comparing `hydromodel-0.2.3/hydromodel/datasets/__init__.py` & `hydromodel-0.2.4/hydromodel/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hydromodel-0.2.3/hydromodel/datasets/data_preprocess.py` & `hydromodel-0.2.4/hydromodel/datasets/data_preprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Author: Wenyu Ouyang
 Date: 2022-10-25 21:16:22
-LastEditTime: 2024-03-27 18:17:14
+LastEditTime: 2024-05-20 20:08:10
 LastEditors: Wenyu Ouyang
 Description: preprocess data for models in hydro-model-xaj
-FilePath: \hydro-model-xaj\hydromodel\datasets\data_preprocess.py
+FilePath: \hydromodel\hydromodel\datasets\data_preprocess.py
 Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
 """
 
 import os
 import re
 import numpy as np
 import pandas as pd
@@ -456,15 +456,15 @@
         camels_data_dir = os.path.join(
             SETTING["local_data_path"]["datasets-origin"], "camels", data_dir
         )
         camels = Camels(camels_data_dir)
         ts_data = camels.read_ts_xrdataset(
             basin_ids, periods, ["prcp", "PET", "streamflow"]
         )
-        # trans unit to mm/day
+        # trans unit to mm/time_interval
         qobs_ = ts_data[["streamflow"]]
         target_unit = ts_data["prcp"].attrs.get("units", "unknown")
         r_mmd = streamflow_unit_conv(qobs_, basin_area, target_unit=target_unit)
         ts_data[flow_name] = r_mmd["streamflow"]
         ts_data[flow_name].attrs["units"] = target_unit
         ts_data = ts_data.rename({"PET": pet_name})
         # ts_data = ts_data.drop_vars('streamflow')
@@ -522,23 +522,40 @@
         # cross validation
         train_and_test_data = cross_valid_data(ts_data, periods, warmup, cv_fold)
     return train_and_test_data
 
 
 def get_rr_events(rain, flow, basin_area):
     ureg = UnitRegistry()
-    # trans unit to mm/day
+    # trans unit to mm/time_interval
     flow_threshold = streamflow_unit_conv(
         np.array([100]) * ureg.m**3 / ureg.s,
         basin_area.isel(basin=0).to_array().to_numpy() * ureg.km**2,
-        target_unit="mm/h",
+        target_unit=flow.units,
     )
+    # 正则表达式匹配 mm/xh 和 mm/xd 格式
+    match = re.match(r"mm/(\d+)(h|d)", flow.units)
+
+    if match:
+        num, unit = match.groups()
+        num = int(num)
+        if unit == "h":
+            multiple = num
+        elif unit == "d":
+            multiple = num * 24
+        else:
+            raise ValueError(f"Unsupported unit: {unit}")
+    else:
+        raise ValueError(f"Invalid unit format: {flow.units}")
+
+    print(f"flow.units = { flow.units}, multiple = {multiple}")
     rr_events = {}
     for basin in basin_area.basin.values:
         rr_event = rainfall_runoff_event_identify(
             rain.sel(basin=basin).to_series(),
             flow.sel(basin=basin).to_series(),
-            multiple=1,
+            multiple=multiple,
             flow_threshold=flow_threshold[0],
+            rain_min=0.02 * multiple,
         )
         rr_events[basin] = rr_event
     return rr_events
```

### Comparing `hydromodel-0.2.3/hydromodel/datasets/data_visualize.py` & `hydromodel-0.2.4/hydromodel/datasets/data_visualize.py`

 * *Files identical despite different names*

### Comparing `hydromodel-0.2.3/hydromodel/models/gr4j.py` & `hydromodel-0.2.4/hydromodel/models/gr4j.py`

 * *Files identical despite different names*

### Comparing `hydromodel-0.2.3/hydromodel/models/hymod.py` & `hydromodel-0.2.4/hydromodel/models/hymod.py`

 * *Files identical despite different names*

### Comparing `hydromodel-0.2.3/hydromodel/models/model_config.py` & `hydromodel-0.2.4/hydromodel/models/model_config.py`

 * *Files identical despite different names*

### Comparing `hydromodel-0.2.3/hydromodel/models/model_dict.py` & `hydromodel-0.2.4/hydromodel/models/model_dict.py`

 * *Files identical despite different names*

### Comparing `hydromodel-0.2.3/hydromodel/models/xaj.py` & `hydromodel-0.2.4/hydromodel/models/xaj.py`

 * *Files identical despite different names*

### Comparing `hydromodel-0.2.3/hydromodel/models/xaj_bmi.py` & `hydromodel-0.2.4/hydromodel/models/xaj_bmi.py`

 * *Files identical despite different names*

### Comparing `hydromodel-0.2.3/hydromodel/trainers/calibrate_ga.py` & `hydromodel-0.2.4/hydromodel/trainers/calibrate_ga.py`

 * *Files identical despite different names*

### Comparing `hydromodel-0.2.3/hydromodel/trainers/calibrate_sceua.py` & `hydromodel-0.2.4/hydromodel/trainers/calibrate_sceua.py`

 * *Files identical despite different names*

### Comparing `hydromodel-0.2.3/hydromodel/trainers/evaluate.py` & `hydromodel-0.2.4/hydromodel/trainers/evaluate.py`

 * *Files identical despite different names*

### Comparing `hydromodel-0.2.3/hydromodel.egg-info/PKG-INFO` & `hydromodel-0.2.4/hydromodel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydromodel
-Version: 0.2.3
+Version: 0.2.4
 Summary: hydrological models starting from XinAnJiang
 Home-page: https://github.com/OuyangWenyu/hydromodel
 Author: Wenyu Ouyang
 Author-email: wenyuouyang@outlook.com
 License: GNU General Public License v3
 Keywords: hydromodel
 Classifier: Intended Audience :: Developers
```

### Comparing `hydromodel-0.2.3/hydromodel.egg-info/SOURCES.txt` & `hydromodel-0.2.4/hydromodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydromodel-0.2.3/setup.py` & `hydromodel-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,10 +60,10 @@
     keywords="hydromodel",
     name="hydromodel",
     packages=find_packages(include=["hydromodel", "hydromodel.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/OuyangWenyu/hydromodel",
-    version='0.2.3',
+    version='0.2.4',
     zip_safe=False,
 )
```

### Comparing `hydromodel-0.2.3/test/test_calibrate.py` & `hydromodel-0.2.4/test/test_calibrate.py`

 * *Files identical despite different names*

### Comparing `hydromodel-0.2.3/test/test_data_preprocess.py` & `hydromodel-0.2.4/test/test_data_preprocess.py`

 * *Files identical despite different names*

### Comparing `hydromodel-0.2.3/test/test_data_visualize.py` & `hydromodel-0.2.4/test/test_data_visualize.py`

 * *Files identical despite different names*

### Comparing `hydromodel-0.2.3/test/test_gr4j.py` & `hydromodel-0.2.4/test/test_gr4j.py`

 * *Files identical despite different names*

### Comparing `hydromodel-0.2.3/test/test_hymod.py` & `hydromodel-0.2.4/test/test_hymod.py`

 * *Files identical despite different names*

### Comparing `hydromodel-0.2.3/test/test_xaj.py` & `hydromodel-0.2.4/test/test_xaj.py`

 * *Files identical despite different names*


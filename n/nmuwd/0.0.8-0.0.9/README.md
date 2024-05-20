# Comparing `tmp/nmuwd-0.0.8.tar.gz` & `tmp/nmuwd-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmuwd-0.0.8.tar", last modified: Fri May 17 22:02:16 2024, max compression
+gzip compressed data, was "nmuwd-0.0.9.tar", last modified: Fri May 17 22:22:22 2024, max compression
```

## Comparing `nmuwd-0.0.8.tar` & `nmuwd-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:02:16.059163 nmuwd-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 22:02:12.000000 nmuwd-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-17 22:02:16.059163 nmuwd-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-17 22:02:12.000000 nmuwd-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:02:16.055163 nmuwd-0.0.8/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:02:12.000000 nmuwd-0.0.8/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-17 22:02:12.000000 nmuwd-0.0.8/backend/bounding_polygons.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-17 22:02:12.000000 nmuwd-0.0.8/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-17 22:02:12.000000 nmuwd-0.0.8/backend/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-17 22:02:12.000000 nmuwd-0.0.8/backend/geo_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-17 22:02:12.000000 nmuwd-0.0.8/backend/persister.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-17 22:02:12.000000 nmuwd-0.0.8/backend/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-05-17 22:02:12.000000 nmuwd-0.0.8/backend/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     8588 2024-05-17 22:02:12.000000 nmuwd-0.0.8/backend/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:02:16.055163 nmuwd-0.0.8/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:02:12.000000 nmuwd-0.0.8/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-17 22:02:12.000000 nmuwd-0.0.8/frontend/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-17 22:02:12.000000 nmuwd-0.0.8/frontend/unifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:02:16.059163 nmuwd-0.0.8/nmuwd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-17 22:02:16.000000 nmuwd-0.0.8/nmuwd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-17 22:02:16.000000 nmuwd-0.0.8/nmuwd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:02:16.000000 nmuwd-0.0.8/nmuwd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 22:02:16.000000 nmuwd-0.0.8/nmuwd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-17 22:02:16.000000 nmuwd-0.0.8/nmuwd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 22:02:16.000000 nmuwd-0.0.8/nmuwd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 22:02:16.059163 nmuwd-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-17 22:02:12.000000 nmuwd-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:22.642762 nmuwd-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 22:22:19.000000 nmuwd-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-17 22:22:22.642762 nmuwd-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-17 22:22:19.000000 nmuwd-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:22.634762 nmuwd-0.0.9/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:22.634762 nmuwd-0.0.9/backend/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:22.634762 nmuwd-0.0.9/backend/connectors/ampapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/ampapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/ampapi/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/ampapi/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:22.638762 nmuwd-0.0.9/backend/connectors/bor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/bor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/bor/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/bor/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:22.638762 nmuwd-0.0.9/backend/connectors/ckan/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/ckan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/ckan/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/ckan/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:22.638762 nmuwd-0.0.9/backend/connectors/isc_seven_rivers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/isc_seven_rivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/isc_seven_rivers/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/isc_seven_rivers/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:22.638762 nmuwd-0.0.9/backend/connectors/st2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/st2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/st2/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/st2/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:22.638762 nmuwd-0.0.9/backend/connectors/usgs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/usgs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/usgs/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/usgs/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:22.638762 nmuwd-0.0.9/backend/connectors/wqp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/wqp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/wqp/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-17 22:22:19.000000 nmuwd-0.0.9/backend/connectors/wqp/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:22.638762 nmuwd-0.0.9/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:19.000000 nmuwd-0.0.9/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-17 22:22:19.000000 nmuwd-0.0.9/frontend/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-17 22:22:19.000000 nmuwd-0.0.9/frontend/unifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:22:22.642762 nmuwd-0.0.9/nmuwd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-17 22:22:22.000000 nmuwd-0.0.9/nmuwd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-17 22:22:22.000000 nmuwd-0.0.9/nmuwd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:22:22.000000 nmuwd-0.0.9/nmuwd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 22:22:22.000000 nmuwd-0.0.9/nmuwd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-17 22:22:22.000000 nmuwd-0.0.9/nmuwd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 22:22:22.000000 nmuwd-0.0.9/nmuwd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 22:22:22.642762 nmuwd-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-17 22:22:19.000000 nmuwd-0.0.9/setup.py
```

### Comparing `nmuwd-0.0.8/LICENSE` & `nmuwd-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.8/PKG-INFO` & `nmuwd-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: nmuwd
-Version: 0.0.8
+Version: 0.0.9
 Summary: New Mexico Water Data Integration Engine
 Home-page: https://github.com/DataIntegrationGroup/PyWeaver
 Author: Jake Ross
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: httpx
 Requires-Dist: geopandas
 Requires-Dist: frost_sta_client
 
 # New Mexico Unified Water Data: Data Integration Engine
+[![Format code](https://github.com/DataIntegrationGroup/PyWeaver/actions/workflows/format_code.yml/badge.svg?branch=main)](https://github.com/DataIntegrationGroup/PyWeaver/actions/workflows/format_code.yml)
+[![Publish Python 🐍 distributions 📦 to PyPI and TestPyPI](https://github.com/DataIntegrationGroup/PyWeaver/actions/workflows/publish-to-pypi.yml/badge.svg)](https://github.com/DataIntegrationGroup/PyWeaver/actions/workflows/publish-to-pypi.yml)
 
-This package provides a command line interface to New Mexico Water Data Initiaive's data integration engine.
-Data Integration Engine. This tool is used to integrate the water data from multiple sources.
+This package provides a command line interface to New Mexico Water Data Initiaive's Data Integration Engine. This tool is used to integrate the water data from multiple sources.
 
 
 ## Sources
  - Bureau of Reclamation
  - USGS (NWIS)
  - ST2 (NMWDI)
    - Pecos Valley Artesian Conservancy District
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nmuwd-0.0.8/frontend/cli.py` & `nmuwd-0.0.9/frontend/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,15 +77,16 @@
         default="",
         help="Bounding box in the form 'x1 y1, x2 y2'",
     ),
     click.option(
         "--county",
         default="",
         help="New Mexico county name",
-    )]
+    ),
+]
 
 
 def add_options(options):
     def _add_options(func):
         for option in reversed(options):
             func = option(func)
         return func
@@ -110,34 +111,45 @@
     "--summarize/--no-summarize",
     is_flag=True,
     default=True,
     show_default=True,
     help="Summarize water levels",
 )
 @add_options(SOURCE_OPTIONS)
-def waterlevels(bbox, county, summarize, no_amp, no_nwis, no_st2, no_isc_seven_rivers, no_bor, no_wqp):
+def waterlevels(
+    bbox,
+    county,
+    summarize,
+    no_amp,
+    no_nwis,
+    no_st2,
+    no_isc_seven_rivers,
+    no_bor,
+    no_wqp,
+):
     config = setup_config("waterlevels", bbox, county)
     config.output_summary_waterlevel_stats = summarize
 
     config.use_source_ampapi = no_amp
     config.use_source_nwis = no_nwis
     config.use_source_st2 = no_st2
     config.use_source_isc_seven_rivers = no_isc_seven_rivers
     config.use_source_bor = no_bor
     config.use_source_wqp = no_wqp
 
     unify_waterlevels(config)
 
 
 @cli.command()
-@click.argument("analyte",
-                type=click.Choice(ANALYTE_CHOICES))
+@click.argument("analyte", type=click.Choice(ANALYTE_CHOICES))
 @add_options(SPATIAL_OPTIONS)
 @add_options(SOURCE_OPTIONS)
-def analytes(analyte, bbox, county, no_amp, no_nwis, no_st2, no_isc_seven_rivers, no_bor, no_wqp):
+def analytes(
+    analyte, bbox, county, no_amp, no_nwis, no_st2, no_isc_seven_rivers, no_bor, no_wqp
+):
     config = setup_config(f"analytes ({analyte})", bbox, county)
     config.analyte = analyte
 
     config.use_source_ampapi = no_amp
     config.use_source_nwis = no_nwis
     config.use_source_st2 = no_st2
     config.use_source_isc_seven_rivers = no_isc_seven_rivers
@@ -156,8 +168,9 @@
         click.echo(f"Getting {tag} for bounding box {bbox}")
 
         # bbox = -105.396826 36.219290, -106.024162 35.384307
         config.bbox = bbox
 
     return config
 
+
 # ============= EOF =============================================
```

### Comparing `nmuwd-0.0.8/frontend/unifier.py` & `nmuwd-0.0.9/frontend/unifier.py`

 * *Files identical despite different names*

### Comparing `nmuwd-0.0.8/nmuwd.egg-info/PKG-INFO` & `nmuwd-0.0.9/nmuwd.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: nmuwd
-Version: 0.0.8
+Version: 0.0.9
 Summary: New Mexico Water Data Integration Engine
 Home-page: https://github.com/DataIntegrationGroup/PyWeaver
 Author: Jake Ross
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: httpx
 Requires-Dist: geopandas
 Requires-Dist: frost_sta_client
 
 # New Mexico Unified Water Data: Data Integration Engine
+[![Format code](https://github.com/DataIntegrationGroup/PyWeaver/actions/workflows/format_code.yml/badge.svg?branch=main)](https://github.com/DataIntegrationGroup/PyWeaver/actions/workflows/format_code.yml)
+[![Publish Python 🐍 distributions 📦 to PyPI and TestPyPI](https://github.com/DataIntegrationGroup/PyWeaver/actions/workflows/publish-to-pypi.yml/badge.svg)](https://github.com/DataIntegrationGroup/PyWeaver/actions/workflows/publish-to-pypi.yml)
 
-This package provides a command line interface to New Mexico Water Data Initiaive's data integration engine.
-Data Integration Engine. This tool is used to integrate the water data from multiple sources.
+This package provides a command line interface to New Mexico Water Data Initiaive's Data Integration Engine. This tool is used to integrate the water data from multiple sources.
 
 
 ## Sources
  - Bureau of Reclamation
  - USGS (NWIS)
  - ST2 (NMWDI)
    - Pecos Valley Artesian Conservancy District
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nmuwd-0.0.8/setup.py` & `nmuwd-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="nmuwd",
-    version="0.0.8",
+    version="0.0.9",
     author="Jake Ross",
     description="New Mexico Water Data Integration Engine",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DataIntegrationGroup/PyWeaver",
     classifiers=[
         "Programming Language :: Python :: 3",
@@ -33,15 +33,15 @@
     ],
     install_requires=["click", "httpx", "geopandas", "frost_sta_client"],
     entry_points={
         "console_scripts": [
             "weave = frontend.cli:cli",
         ],
     },
-    packages=["frontend", "backend"],
+    packages=["frontend"] + [f'backend.{p}' for p in find_packages('backend')],
     python_requires=">=3.6",
     include_package_data=True,
     # package_data={
     # If any package contains *.txt or *.rst files, include them:
     #     "templates": [
     #         "*.template",
     #     ],
```


# Comparing `tmp/osm-rawdata-0.2.4.tar.gz` & `tmp/osm-rawdata-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osm-rawdata-0.2.4.tar", last modified: Sun Apr  7 19:14:37 2024, max compression
+gzip compressed data, was "osm-rawdata-0.3.0.tar", last modified: Mon May 20 15:04:43 2024, max compression
```

## Comparing `osm-rawdata-0.2.4.tar` & `osm-rawdata-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34102 2024-04-07 19:14:30.544991 osm-rawdata-0.2.4/LICENSE.md
--rw-r--r--   0        0        0     5563 2024-04-07 19:14:30.544991 osm-rawdata-0.2.4/README.md
--rw-r--r--   0        0        0       44 2024-04-07 19:14:30.548991 osm-rawdata-0.2.4/osm_rawdata/__version__.py
--rwxr-xr-x   0        0        0    13038 2024-04-07 19:14:30.548991 osm-rawdata-0.2.4/osm_rawdata/config.py
--rw-r--r--   0        0        0     3069 2024-04-07 19:14:30.548991 osm-rawdata-0.2.4/osm_rawdata/db_models.py
--rw-r--r--   0        0        0     1086 2024-04-07 19:14:30.548991 osm-rawdata-0.2.4/osm_rawdata/db_schemas.py
--rwxr-xr-x   0        0        0     3479 2024-04-07 19:14:30.548991 osm-rawdata-0.2.4/osm_rawdata/geofabrik.py
--rw-r--r--   0        0        0     2702 2024-04-07 19:14:30.548991 osm-rawdata-0.2.4/osm_rawdata/geofabrik.yaml
--rwxr-xr-x   0        0        0    13652 2024-04-07 19:14:30.548991 osm-rawdata-0.2.4/osm_rawdata/importer.py
--rw-r--r--   0        0        0     2317 2024-04-07 19:14:30.548991 osm-rawdata-0.2.4/osm_rawdata/models.py
--rw-r--r--   0        0        0     1141 2024-04-07 19:14:30.548991 osm-rawdata-0.2.4/osm_rawdata/nodes.sql
--rwxr-xr-x   0        0        0     6584 2024-04-07 19:14:30.548991 osm-rawdata-0.2.4/osm_rawdata/overture.py
--rwxr-xr-x   0        0        0    24439 2024-04-07 19:14:30.548991 osm-rawdata-0.2.4/osm_rawdata/pgasync.py
--rwxr-xr-x   0        0        0    31267 2024-04-07 19:14:30.548991 osm-rawdata-0.2.4/osm_rawdata/postgres.py
--rw-r--r--   0        0        0     6347 2024-04-07 19:14:30.548991 osm-rawdata-0.2.4/osm_rawdata/raw.lua
--rw-r--r--   0        0        0     6711 2024-04-07 19:14:30.548991 osm-rawdata-0.2.4/osm_rawdata/raw_with_ref.lua
--rw-r--r--   0        0        0     1170 2024-04-07 19:14:30.548991 osm-rawdata-0.2.4/osm_rawdata/ways_line.sql
--rw-r--r--   0        0        0     2893 2024-04-07 19:14:30.548991 osm-rawdata-0.2.4/osm_rawdata/ways_poly.sql
--rw-r--r--   0        0        0     2549 2024-04-07 19:14:30.548991 osm-rawdata-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     6290 1970-01-01 00:00:00.000000 osm-rawdata-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    34102 2024-05-20 15:04:34.327600 osm-rawdata-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     5563 2024-05-20 15:04:34.327600 osm-rawdata-0.3.0/README.md
+-rw-r--r--   0        0        0       44 2024-05-20 15:04:34.331600 osm-rawdata-0.3.0/osm_rawdata/__version__.py
+-rwxr-xr-x   0        0        0    13038 2024-05-20 15:04:34.331600 osm-rawdata-0.3.0/osm_rawdata/config.py
+-rw-r--r--   0        0        0     3069 2024-05-20 15:04:34.331600 osm-rawdata-0.3.0/osm_rawdata/db_models.py
+-rw-r--r--   0        0        0     1086 2024-05-20 15:04:34.331600 osm-rawdata-0.3.0/osm_rawdata/db_schemas.py
+-rwxr-xr-x   0        0        0     3479 2024-05-20 15:04:34.331600 osm-rawdata-0.3.0/osm_rawdata/geofabrik.py
+-rw-r--r--   0        0        0     2702 2024-05-20 15:04:34.331600 osm-rawdata-0.3.0/osm_rawdata/geofabrik.yaml
+-rwxr-xr-x   0        0        0    13652 2024-05-20 15:04:34.331600 osm-rawdata-0.3.0/osm_rawdata/importer.py
+-rw-r--r--   0        0        0     2317 2024-05-20 15:04:34.331600 osm-rawdata-0.3.0/osm_rawdata/models.py
+-rw-r--r--   0        0        0     1141 2024-05-20 15:04:34.331600 osm-rawdata-0.3.0/osm_rawdata/nodes.sql
+-rwxr-xr-x   0        0        0     6584 2024-05-20 15:04:34.331600 osm-rawdata-0.3.0/osm_rawdata/overture.py
+-rwxr-xr-x   0        0        0    24438 2024-05-20 15:04:34.331600 osm-rawdata-0.3.0/osm_rawdata/pgasync.py
+-rwxr-xr-x   0        0        0    31266 2024-05-20 15:04:34.331600 osm-rawdata-0.3.0/osm_rawdata/postgres.py
+-rw-r--r--   0        0        0     6347 2024-05-20 15:04:34.331600 osm-rawdata-0.3.0/osm_rawdata/raw.lua
+-rw-r--r--   0        0        0     6711 2024-05-20 15:04:34.331600 osm-rawdata-0.3.0/osm_rawdata/raw_with_ref.lua
+-rw-r--r--   0        0        0     1170 2024-05-20 15:04:34.331600 osm-rawdata-0.3.0/osm_rawdata/ways_line.sql
+-rw-r--r--   0        0        0     2893 2024-05-20 15:04:34.331600 osm-rawdata-0.3.0/osm_rawdata/ways_poly.sql
+-rw-r--r--   0        0        0     2549 2024-05-20 15:04:34.331600 osm-rawdata-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6290 1970-01-01 00:00:00.000000 osm-rawdata-0.3.0/PKG-INFO
```

### Comparing `osm-rawdata-0.2.4/LICENSE.md` & `osm-rawdata-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `osm-rawdata-0.2.4/README.md` & `osm-rawdata-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `osm-rawdata-0.2.4/osm_rawdata/config.py` & `osm-rawdata-0.3.0/osm_rawdata/config.py`

 * *Files identical despite different names*

### Comparing `osm-rawdata-0.2.4/osm_rawdata/db_models.py` & `osm-rawdata-0.3.0/osm_rawdata/db_models.py`

 * *Files identical despite different names*

### Comparing `osm-rawdata-0.2.4/osm_rawdata/db_schemas.py` & `osm-rawdata-0.3.0/osm_rawdata/db_schemas.py`

 * *Files identical despite different names*

### Comparing `osm-rawdata-0.2.4/osm_rawdata/geofabrik.py` & `osm-rawdata-0.3.0/osm_rawdata/geofabrik.py`

 * *Files identical despite different names*

### Comparing `osm-rawdata-0.2.4/osm_rawdata/geofabrik.yaml` & `osm-rawdata-0.3.0/osm_rawdata/geofabrik.yaml`

 * *Files identical despite different names*

### Comparing `osm-rawdata-0.2.4/osm_rawdata/importer.py` & `osm-rawdata-0.3.0/osm_rawdata/importer.py`

 * *Files identical despite different names*

### Comparing `osm-rawdata-0.2.4/osm_rawdata/models.py` & `osm-rawdata-0.3.0/osm_rawdata/models.py`

 * *Files identical despite different names*

### Comparing `osm-rawdata-0.2.4/osm_rawdata/nodes.sql` & `osm-rawdata-0.3.0/osm_rawdata/nodes.sql`

 * *Files identical despite different names*

### Comparing `osm-rawdata-0.2.4/osm_rawdata/overture.py` & `osm-rawdata-0.3.0/osm_rawdata/overture.py`

 * *Files identical despite different names*

### Comparing `osm-rawdata-0.2.4/osm_rawdata/pgasync.py` & `osm-rawdata-0.3.0/osm_rawdata/pgasync.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
         if self.dburi["dbname"] == "underpass":
             # Authentication data
             # self.auth = HTTPBasicAuth(self.user, self.passwd)
 
             # Use a persistant connect, better for multiple requests
             self.session = requests.Session()
-            self.url = os.getenv("UNDERPASS_API_URL", "https://raw-data-api0.hotosm.org/v1")
+            self.url = os.getenv("RAW_DATA_API_URL", "https://raw-data-api0.hotosm.org/v1")
             self.headers = {"accept": "application/json", "Content-Type": "application/json"}
         else:
             # log.debug(f"Connecting with: {connect}")
             try:
                 self.pg = await asyncpg.connect(connect)
                 if self.pg.is_closed():
                     log.error(f"Couldn't open cursor in {self.uri['dbname']}")
```

### Comparing `osm-rawdata-0.2.4/osm_rawdata/postgres.py` & `osm-rawdata-0.3.0/osm_rawdata/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         """
         self.dbshell = None
         self.dbcursor = None
         self.uri = uriParser(dburi)
         if self.uri["dbname"] == "underpass":
             # Use a persistant connect, better for multiple requests
             self.session = requests.Session()
-            self.url = os.getenv("UNDERPASS_API_URL", "https://api-prod.raw-data.hotosm.org/v1")
+            self.url = os.getenv("RAW_DATA_API_URL", "https://api-prod.raw-data.hotosm.org/v1")
             self.headers = {"accept": "application/json", "Content-Type": "application/json"}
         else:
             log.info(f"Opening database connection to: {self.uri['dbname']}")
             connect = "PG: dbname=" + self.uri["dbname"]
             if "dbname" in self.uri and self.uri["dbname"] is not None:
                 connect = f"dbname={self.uri['dbname']}"
             elif "dbhost" in self.uri and self.uri["dbhost"] == "localhost" and self.uri["dbhost"] is not None:
```

### Comparing `osm-rawdata-0.2.4/osm_rawdata/raw.lua` & `osm-rawdata-0.3.0/osm_rawdata/raw.lua`

 * *Files identical despite different names*

### Comparing `osm-rawdata-0.2.4/osm_rawdata/raw_with_ref.lua` & `osm-rawdata-0.3.0/osm_rawdata/raw_with_ref.lua`

 * *Files identical despite different names*

### Comparing `osm-rawdata-0.2.4/osm_rawdata/ways_line.sql` & `osm-rawdata-0.3.0/osm_rawdata/ways_line.sql`

 * *Files identical despite different names*

### Comparing `osm-rawdata-0.2.4/osm_rawdata/ways_poly.sql` & `osm-rawdata-0.3.0/osm_rawdata/ways_poly.sql`

 * *Files identical despite different names*

### Comparing `osm-rawdata-0.2.4/pyproject.toml` & `osm-rawdata-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 classifiers = [
     "Topic :: Utilities",
     "Topic :: Scientific/Engineering :: GIS",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "0.2.4"
+version = "0.3.0"
 
 [project.urls]
 homepage = "https://hotosm.github.io/osm-rawdata"
 documentation = "https://hotosm.github.io/osm-rawdata"
 repository = "https://github.com/hotosm/osm-rawdata"
 
 [project.scripts]
@@ -57,15 +57,15 @@
 ]
 pythonpath = "osm_rawdata"
 log_cli = true
 log_cli_level = "DEBUG"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.2.4"
+version = "0.3.0"
 version_files = [
     "pyproject.toml:version",
     "osm_rawdata/__version__.py",
     "Makefile:VERSION",
 ]
 update_changelog_on_bump = true
```

### Comparing `osm-rawdata-0.2.4/PKG-INFO` & `osm-rawdata-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm-rawdata
-Version: 0.2.4
+Version: 0.3.0
 Summary: Make data extracts from OSM data.
 License: AGPL-3.0-only
 Keywords: hot,osm,openstreetmap
 Author-email: Rob Savoye <rob.savoye@hotosm.org>,Sam Woodcock <sam.woodcock@hotosm.org>
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: osm-rawdata Version: 0.2.4 Summary: Make data
+Metadata-Version: 2.1 Name: osm-rawdata Version: 0.3.0 Summary: Make data
 extracts from OSM data. License: AGPL-3.0-only Keywords: hot,osm,openstreetmap
 Author-email: Rob Savoye
 hotosm.org>,Sam Woodcock
 hotosm.org> Requires-Python: >=3.10 Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Utilities Project-URL: documentation, https://
```


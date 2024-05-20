# Comparing `tmp/ftm_columnstore-0.3.0.tar.gz` & `tmp/ftm_columnstore-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftm_columnstore-0.3.0.tar", max compression
+gzip compressed data, was "ftm_columnstore-0.3.1.tar", max compression
```

## Comparing `ftm_columnstore-0.3.0.tar` & `ftm_columnstore-0.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2022-10-06 10:32:22.190067 ftm_columnstore-0.3.0/LICENSE
--rw-r--r--   0        0        0     1675 2023-10-20 05:57:45.228164 ftm_columnstore-0.3.0/README.md
--rw-r--r--   0        0        0      624 2024-05-19 01:38:51.140349 ftm_columnstore-0.3.0/ftm_columnstore/__init__.py
--rw-r--r--   0        0        0     1985 2023-10-20 05:44:54.544953 ftm_columnstore-0.3.0/ftm_columnstore/cli.py
--rw-r--r--   0        0        0    10556 2024-05-19 00:19:38.798693 ftm_columnstore-0.3.0/ftm_columnstore/engine.py
--rw-r--r--   0        0        0     2271 2023-10-20 05:44:54.544953 ftm_columnstore-0.3.0/ftm_columnstore/phonetic.py
--rw-r--r--   0        0        0      380 2024-05-19 01:38:51.140349 ftm_columnstore-0.3.0/ftm_columnstore/settings.py
--rw-r--r--   0        0        0     2461 2023-10-20 05:44:54.544953 ftm_columnstore-0.3.0/ftm_columnstore/statements.py
--rw-r--r--   0        0        0     2880 2023-10-20 05:44:54.544953 ftm_columnstore-0.3.0/ftm_columnstore/store.py
--rw-r--r--   0        0        0     1592 2024-05-19 01:38:51.140349 ftm_columnstore-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2968 1970-01-01 00:00:00.000000 ftm_columnstore-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-06 10:32:22.190067 ftm_columnstore-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1675 2023-10-20 05:57:45.228164 ftm_columnstore-0.3.1/README.md
+-rw-r--r--   0        0        0      624 2024-05-20 17:35:23.483653 ftm_columnstore-0.3.1/ftm_columnstore/__init__.py
+-rw-r--r--   0        0        0     2518 2024-05-20 16:56:37.993677 ftm_columnstore-0.3.1/ftm_columnstore/cli.py
+-rw-r--r--   0        0        0    11168 2024-05-20 12:37:28.378590 ftm_columnstore-0.3.1/ftm_columnstore/engine.py
+-rw-r--r--   0        0        0     2271 2023-10-20 05:44:54.544953 ftm_columnstore-0.3.1/ftm_columnstore/phonetic.py
+-rw-r--r--   0        0        0      380 2024-05-20 17:35:23.483653 ftm_columnstore-0.3.1/ftm_columnstore/settings.py
+-rw-r--r--   0        0        0     2461 2023-10-20 05:44:54.544953 ftm_columnstore-0.3.1/ftm_columnstore/statements.py
+-rw-r--r--   0        0        0     2880 2023-10-20 05:44:54.544953 ftm_columnstore-0.3.1/ftm_columnstore/store.py
+-rw-r--r--   0        0        0     1592 2024-05-20 17:35:23.483653 ftm_columnstore-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2968 1970-01-01 00:00:00.000000 ftm_columnstore-0.3.1/PKG-INFO
```

### Comparing `ftm_columnstore-0.3.0/LICENSE` & `ftm_columnstore-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ftm_columnstore-0.3.0/README.md` & `ftm_columnstore-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ftm_columnstore-0.3.0/ftm_columnstore/__init__.py` & `ftm_columnstore-0.3.1/ftm_columnstore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 logging.getLogger("numpy.core.fromnumeric").setLevel(logging.ERROR)
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 warnings.filterwarnings("ignore", category=np.VisibleDeprecationWarning)
 
 # FIXME sqlalchemy monkey patch not working
 nomenklatura.settings.DB_URL = "sqlite:///:memory:"
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 __all__ = ["get_engine", "get_store"]
```

### Comparing `ftm_columnstore-0.3.0/ftm_columnstore/cli.py` & `ftm_columnstore-0.3.1/ftm_columnstore/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from typing import Annotated, Optional
 
 import typer
-from ftmq.io import smart_read_proxies
+from ftmq.io import smart_read_proxies, smart_write_proxies
 from rich import print
 
 from ftm_columnstore import get_engine, get_store, settings
 
 log = logging.getLogger(__name__)
 
 cli = typer.Typer(no_args_is_help=True)
@@ -30,14 +30,30 @@
         ),
     ] = False
 ):
     engine = get_engine()
     engine.ensure(recreate=recreate, exists_ok=True)
 
 
+@cli.command("iterate", help="Read entities from the store.")
+def cli_iterate(
+    dataset: Annotated[
+        Optional[str], typer.Option("-d", help="Dataset to read from")
+    ] = None,
+    out_uri: Annotated[
+        str, typer.Option("-o", help="Entities uri (as interpreted by `ftmq`)")
+    ] = "-",
+):
+    """
+    Read entities from the store and write json to `-o` (default: stdout)
+    """
+    store = get_store(dataset=dataset)
+    smart_write_proxies(out_uri, store.iterate(dataset), serialize=True)
+
+
 @cli.command("write", help="Write entity fragments to the store.")
 def cli_write(
     in_uri: Annotated[
         str, typer.Option("-i", help="Entities uri (as read by `ftmq`)")
     ] = "-",
     dataset: Annotated[
         Optional[str], typer.Option("-d", help="Dataset to write to")
```

### Comparing `ftm_columnstore-0.3.0/ftm_columnstore/engine.py` & `ftm_columnstore-0.3.1/ftm_columnstore/engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,16 +146,16 @@
             INDEX cix (canonical_id) TYPE set(0) GRANULARITY 4,
             INDEX eix (entity_id) TYPE set(0) GRANULARITY 4,
             INDEX six (schema) TYPE set(0) GRANULARITY 1,
             INDEX dix (dataset) TYPE set(0) GRANULARITY 1,
             INDEX tix (prop_type) TYPE set(0) GRANULARITY 1,
             INDEX pix (prop) TYPE set(0) GRANULARITY 1
         ) ENGINE = ReplacingMergeTree(last_seen)
-        PRIMARY KEY (canonical_id, entity_id, id)
-        ORDER BY (canonical_id, entity_id, id)
+        PRIMARY KEY (canonical_id, entity_id, prop, value, id)
+        ORDER BY (canonical_id, entity_id, prop, value, id)
         """
 
         create_table_fpx = f"""
         CREATE TABLE {self.table_fpx}
         (
             `algorithm`     Enum('fingerprint', 'metaphone1', 'metaphone2', 'soundex'),
             `value`         String,
@@ -230,14 +230,22 @@
             length(value) AS len
         FROM {self.table_fpx}
         WHERE algorithm = 'fingerprint'
         GROUP BY value
         """
 
         projections = (
+            f"""ALTER TABLE {self.table} ADD PROJECTION {self.table}_dataset (
+                SELECT * ORDER BY dataset,canonical_id,prop)""",
+            f"""ALTER TABLE {self.table} ADD PROJECTION {self.table}_schema (
+                SELECT * ORDER BY schema,canonical_id,prop)""",
+            f"""ALTER TABLE {self.table} ADD PROJECTION {self.table}_dataset_schema (
+                SELECT * ORDER BY dataset,schema,canonical_id,prop)""",
+            f"""ALTER TABLE {self.table} ADD PROJECTION {self.table}_schema (
+                SELECT * ORDER BY schema,canonical_id,prop)""",
             f"""ALTER TABLE {self.table} ADD PROJECTION {self.table}_values (
                 SELECT * ORDER BY value,prop)""",
             f"""ALTER TABLE {self.table} ADD PROJECTION {self.table}_canonical_lookup (
                 SELECT * ORDER BY entity_id,canonical_id)""",
             f"""ALTER TABLE {self.table} ADD PROJECTION {self.table}_canonical_id (
                 SELECT * ORDER BY canonical_id,prop)""",
             f"""ALTER TABLE {self.table} ADD PROJECTION {self.table}_entity_id (
```

### Comparing `ftm_columnstore-0.3.0/ftm_columnstore/phonetic.py` & `ftm_columnstore-0.3.1/ftm_columnstore/phonetic.py`

 * *Files identical despite different names*

### Comparing `ftm_columnstore-0.3.0/ftm_columnstore/statements.py` & `ftm_columnstore-0.3.1/ftm_columnstore/statements.py`

 * *Files identical despite different names*

### Comparing `ftm_columnstore-0.3.0/ftm_columnstore/store.py` & `ftm_columnstore-0.3.1/ftm_columnstore/store.py`

 * *Files identical despite different names*

### Comparing `ftm_columnstore-0.3.0/pyproject.toml` & `ftm_columnstore-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftm-columnstore"
-version = "0.3.0"
+version = "0.3.1"
 description = "Column store implementation for ftm data based on clickhouse"
 authors = ["Simon Wörpel <simon@investigativedata.org>"]
 license = "GPL3"
 readme = "README.md"
 homepage = "https://github.com/investigativedata/ftm-columnstore"
 repository = "https://github.com/investigativedata/ftm-columnstore"
 documentation = "https://github.com/investigativedata/ftm-columnstore"
@@ -30,15 +30,15 @@
 clickhouse-driver = {extras = ["numpy"], version = "^0.2.7"}
 pyicu = "^2.13.1"
 libindic-soundex = "^1.0.2"
 libindic-utils = "^1.0.3"
 metaphone = "^0.6"
 pandas = "^2.2.2"
 rich = "^13.7.1"
-ftmq = "^0.6.4"
+ftmq = "^0.6.5"
 
 
 [tool.poetry.group.dev.dependencies]
 absolufy-imports = "^0.3.1"
 ipdb = "^0.13.13"
 black = "^23.11.0"
 isort = "^5.12.0"
```

### Comparing `ftm_columnstore-0.3.0/PKG-INFO` & `ftm_columnstore-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ftm-columnstore
-Version: 0.3.0
+Version: 0.3.1
 Summary: Column store implementation for ftm data based on clickhouse
 Home-page: https://github.com/investigativedata/ftm-columnstore
 License: GPL3
 Author: Simon Wörpel
 Author-email: simon@investigativedata.org
 Requires-Python: >=3.11,<3.12
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: banal (>=1.0.6,<2.0.0)
 Requires-Dist: clickhouse-driver[numpy] (>=0.2.7,<0.3.0)
-Requires-Dist: ftmq (>=0.6.4,<0.7.0)
+Requires-Dist: ftmq (>=0.6.5,<0.7.0)
 Requires-Dist: libindic-soundex (>=1.0.2,<2.0.0)
 Requires-Dist: libindic-utils (>=1.0.3,<2.0.0)
 Requires-Dist: metaphone (>=0.6,<0.7)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pyicu (>=2.13.1,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
```


# Comparing `tmp/pgmerge-1.9.0.tar.gz` & `tmp/pgmerge-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgmerge-1.9.0.tar", max compression
+gzip compressed data, was "pgmerge-1.9.1.tar", max compression
```

## Comparing `pgmerge-1.9.0.tar` & `pgmerge-1.9.1.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rwxr-xr-x   0        0        0    11358 2018-02-06 06:48:24.089373 pgmerge-1.9.0/LICENSE
--rwxr-xr-x   0        0        0      108 2021-09-26 16:06:26.949205 pgmerge-1.9.0/NOTICE
--rwxr-xr-x   0        0        0     4478 2021-09-26 19:26:29.983654 pgmerge-1.9.0/README.md
--rwxr-xr-x   0        0        0      144 2021-12-04 14:53:10.009974 pgmerge-1.9.0/pgmerge/__init__.py
--rwxr-xr-x   0        0        0     7544 2021-12-04 22:44:06.292323 pgmerge-1.9.0/pgmerge/db_config.py
--rwxr-xr-x   0        0        0    12325 2021-12-04 22:44:30.449150 pgmerge-1.9.0/pgmerge/db_export.py
--rwxr-xr-x   0        0        0     4894 2021-12-05 08:55:01.554240 pgmerge-1.9.0/pgmerge/db_graph.py
--rwxr-xr-x   0        0        0    18195 2021-12-05 08:55:01.558240 pgmerge-1.9.0/pgmerge/db_import.py
--rwxr-xr-x   0        0        0     7521 2021-12-04 22:26:04.441875 pgmerge-1.9.0/pgmerge/db_inspect.py
--rwxr-xr-x   0        0        0     3013 2021-12-04 20:56:00.604054 pgmerge-1.9.0/pgmerge/pg_pass.py
--rwxr-xr-x   0        0        0    26555 2021-12-04 22:37:18.793803 pgmerge-1.9.0/pgmerge/pgmerge.py
--rwxr-xr-x   0        0        0     1651 2019-07-27 12:20:33.108547 pgmerge-1.9.0/pgmerge/tables_config_schema.yml
--rwxr-xr-x   0        0        0        0 2021-12-04 15:14:43.192569 pgmerge-1.9.0/pgmerge/tests/__init__.py
--rwxr-xr-x   0        0        0    16391 2021-12-04 18:49:11.481334 pgmerge-1.9.0/pgmerge/tests/test_cli.py
--rwxr-xr-x   0        0        0     3318 2021-12-04 15:14:38.115717 pgmerge-1.9.0/pgmerge/tests/test_db.py
--rwxr-xr-x   0        0        0     2717 2021-12-04 20:51:20.467486 pgmerge-1.9.0/pgmerge/utils.py
--rwxr-xr-x   0        0        0     1271 2021-12-05 08:03:36.411446 pgmerge-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     5484 2021-12-05 08:55:14.604560 pgmerge-1.9.0/setup.py
--rw-r--r--   0        0        0     5752 2021-12-05 08:55:14.605065 pgmerge-1.9.0/PKG-INFO
+-rwxr-xr-x   0        0        0    11358 2018-02-06 06:48:24.089373 pgmerge-1.9.1/LICENSE
+-rwxr-xr-x   0        0        0      108 2021-09-26 16:06:26.949205 pgmerge-1.9.1/NOTICE
+-rwxr-xr-x   0        0        0     4478 2021-09-26 19:26:29.983654 pgmerge-1.9.1/README.md
+-rwxr-xr-x   0        0        0      144 2021-12-06 22:22:14.743585 pgmerge-1.9.1/pgmerge/__init__.py
+-rwxr-xr-x   0        0        0     7672 2021-12-06 19:43:50.520046 pgmerge-1.9.1/pgmerge/db_config.py
+-rwxr-xr-x   0        0        0    12325 2021-12-04 22:44:30.449150 pgmerge-1.9.1/pgmerge/db_export.py
+-rwxr-xr-x   0        0        0     4894 2021-12-11 14:53:50.424641 pgmerge-1.9.1/pgmerge/db_graph.py
+-rwxr-xr-x   0        0        0    18195 2021-12-11 14:53:50.446975 pgmerge-1.9.1/pgmerge/db_import.py
+-rwxr-xr-x   0        0        0     7590 2021-12-11 14:09:10.261102 pgmerge-1.9.1/pgmerge/db_inspect.py
+-rwxr-xr-x   0        0        0     3013 2021-12-06 18:51:49.030604 pgmerge-1.9.1/pgmerge/pg_pass.py
+-rwxr-xr-x   0        0        0    27057 2021-12-11 14:35:43.651634 pgmerge-1.9.1/pgmerge/pgmerge.py
+-rwxr-xr-x   0        0        0     1651 2019-07-27 12:20:33.108547 pgmerge-1.9.1/pgmerge/tables_config_schema.yml
+-rwxr-xr-x   0        0        0        0 2021-12-04 15:14:43.192569 pgmerge-1.9.1/pgmerge/tests/__init__.py
+-rwxr-xr-x   0        0        0     1894 2021-12-11 09:09:46.028653 pgmerge-1.9.1/pgmerge/tests/helpers.py
+-rwxr-xr-x   0        0        0    12095 2021-12-11 14:53:50.455317 pgmerge-1.9.1/pgmerge/tests/test_cli.py
+-rwxr-xr-x   0        0        0    10446 2021-12-11 14:53:50.462325 pgmerge-1.9.1/pgmerge/tests/test_config.py
+-rwxr-xr-x   0        0        0     3486 2021-12-07 21:43:25.963373 pgmerge-1.9.1/pgmerge/tests/test_db.py
+-rwxr-xr-x   0        0        0     1055 2021-12-11 14:52:27.579986 pgmerge-1.9.1/pgmerge/tests/test_utils.py
+-rwxr-xr-x   0        0        0     2717 2021-12-04 20:51:20.467486 pgmerge-1.9.1/pgmerge/utils.py
+-rwxr-xr-x   0        0        0     1367 2021-12-11 13:08:46.815085 pgmerge-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     5484 2021-12-11 14:54:15.032539 pgmerge-1.9.1/setup.py
+-rw-r--r--   0        0        0     5752 2021-12-11 14:54:15.033032 pgmerge-1.9.1/PKG-INFO
```

### Comparing `pgmerge-1.9.0/LICENSE` & `pgmerge-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pgmerge-1.9.0/README.md` & `pgmerge-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pgmerge-1.9.0/pgmerge/db_config.py` & `pgmerge-1.9.1/pgmerge/db_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 pgmerge - a PostgreSQL data import and merge utility.
 
 Copyright 2018-2021 Simon Muller (samullers@gmail.com)
 """
 import os
+import urllib
 import logging
 import getpass
 from typing import Any, Dict, List, Set, Optional, cast
 
 import yaml
 from rxjson import Rx
 from appdirs import user_config_dir
@@ -152,17 +153,19 @@
 def generate_url(uri: Optional[str], dbname: str, host: str, port: str, username: str, password: str,
                  type: str = "postgresql") -> str:
     """Generate connection string URL from various connection details."""
     if uri:
         uri = uri if uri[-1] != '/' else uri[:-1]
         return "{}/{}".format(uri, dbname)
 
-    config_db = {'type': type, 'host': host, 'port': port,
-                 'username': username, 'password': password,
-                 'dbname': dbname}
+    config_db = {'type': type, 'port': port,
+                 'host': urllib.parse.quote(host),
+                 'username': urllib.parse.quote(username),
+                 'password': urllib.parse.quote(password),
+                 'dbname': urllib.parse.quote(dbname)}
     url = "{type}://{username}:{password}@{host}:{port}/{dbname}".format(**config_db)
     return url
 
 
 class ConfigInvalidException(Exception):
     """Exception raised for invalid config file."""
```

### Comparing `pgmerge-1.9.0/pgmerge/db_export.py` & `pgmerge-1.9.1/pgmerge/db_export.py`

 * *Files identical despite different names*

### Comparing `pgmerge-1.9.0/pgmerge/db_graph.py` & `pgmerge-1.9.1/pgmerge/db_graph.py`

 * *Files identical despite different names*

### Comparing `pgmerge-1.9.0/pgmerge/db_import.py` & `pgmerge-1.9.1/pgmerge/db_import.py`

 * *Files identical despite different names*

### Comparing `pgmerge-1.9.0/pgmerge/db_inspect.py` & `pgmerge-1.9.1/pgmerge/db_inspect.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 _log = logging.getLogger(__name__)
 
 
 def print_missing_primary_keys(inspector: Any, schema: str) -> None:
     """Find and print tables in database that don't have primary keys."""
     no_pks = []
     for table in inspector.get_table_names(schema):
-        pks = inspector.get_primary_keys(table, schema)
+        pks = inspector.get_pk_constraint(table, schema)
         if len(pks) == 0:
             no_pks.append(table)
     if len(no_pks) > 0:
         print("\n%s tables have no primary key:" % (len(no_pks),))
         print(no_pks)
 
 
@@ -44,15 +44,15 @@
         print(cycle)
     except nx.exception.NetworkXNoCycle:
         pass
 
 
 def print_partition_info(table_graph: Any) -> None:
     """Traverse table/foreign-key dependency graph and look for disconnected sub-graphs."""
-    sub_graphs = [graph for graph in nx.weakly_connected_component_subgraphs(table_graph)]
+    sub_graphs = [table_graph.subgraph(c) for c in nx.connected_components(table_graph.to_undirected())]
     if len(sub_graphs) > 1:
         print("\nDependency graph can be partitioned into %s sub-graphs:" % (len(sub_graphs),))
         for graph in sub_graphs:
             print(graph.nodes())
 
 
 def print_insertion_order(table_graph: Any) -> None:
@@ -111,15 +111,15 @@
     natural_key_tables = []
     transformable = []
     pk_contains_fk = []
     tables = sorted(inspector.get_table_names(schema))
     for table in tables:
         columns = inspector.get_columns(table, schema)
         fks = inspector.get_foreign_keys(table, schema)
-        pks = inspector.get_primary_keys(table, schema)
+        pks = [col for pk in inspector.get_pk_constraint(table, schema) for col in pk['constrained_columns']]
         uniques = inspector.get_unique_constraints(table, schema)
 
         for fk in fks:
             if not set(fk['constrained_columns']).isdisjoint(set(pks)):
                 pk_contains_fk.append(table)
 
         auto_id = False
```

### Comparing `pgmerge-1.9.0/pgmerge/pg_pass.py` & `pgmerge-1.9.1/pgmerge/pg_pass.py`

 * *Files identical despite different names*

### Comparing `pgmerge-1.9.0/pgmerge/pgmerge.py` & `pgmerge-1.9.1/pgmerge/pgmerge.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,20 @@
     retrieve_password, generate_url, \
     ConfigInvalidException
 from . import db_graph, db_import, db_export, db_inspect, __version__
 
 APP_NAME = "pgmerge"
 LOG_FILE = os.path.join(user_log_dir(APP_NAME, appauthor=False), "out.log")
 
+EXIT_CODE_ARGS = 2
+# Use exit code 3 for exceptions since click already returns 1 and 2
+# (1 for aborts and 2 invalid arguments)
+EXIT_CODE_EXC = 3
+EXIT_CODE_INVALID_DATA = 4
+
 log = logging.getLogger()
 
 
 app = typer.Typer(
     help="Merge data in CSV files into a Postgresql database.",
     context_settings=dict(max_content_width=120),
     add_completion=False,
@@ -96,16 +102,17 @@
         print_message("Self-referencing tables found that could prevent import: {}"
                       .format(', '.join(sorted(relevant_tables))))
         return True
 
     return False
 
 
+# Excluded from code coverage because all the CLI pre-checks prevent this check from ever picking anything up
 def get_and_warn_about_any_unknown_tables(import_files: List[str], dest_tables: List[str], schema_tables: List[str]
-                                          ) -> Set[str]:
+                                          ) -> Set[str]:  # pragma: no cover
     """Compare tables expected for import with actual in schema and warn about inconsistencies."""
     unknown_tables = set(dest_tables).difference(set(schema_tables))
     if len(unknown_tables) > 0:
         print("Skipping files for unknown tables:")
         for table in unknown_tables:
             idx = dest_tables.index(table)
             print("\t%s: %s" % (table, import_files[idx]))
@@ -245,15 +252,15 @@
     # Check that all expected files exist
     expected_table_files = ["%s.csv" % (table,) for table in dest_tables]
     unknown_files = set(expected_table_files).difference(set(all_files))
     if len(unknown_files) > 0:
         print("No files found for the following tables:")
         for file in unknown_files:
             print("\t", file)
-        sys.exit()
+        sys.exit(EXIT_CODE_INVALID_DATA)
 
     # Convert filenames to full paths
     import_files = [os.path.join(directory, f) for f in import_files]
     return import_files, dest_tables
 
 
 def convert_to_config_per_subset(config_per_table: Dict[str, Any]) -> Dict[str, Any]:
@@ -279,28 +286,28 @@
 
 def validate_schema(inspector: Any, schema: str) -> str:
     """Check that the database schema specified exists and is valid."""
     if schema is None:
         schema = inspector.default_schema_name
     if schema not in inspector.get_schema_names():
         print("Schema not found: '{}'".format(schema))
-        sys.exit()
+        sys.exit(EXIT_CODE_ARGS)
     return schema
 
 
 def validate_tables(inspector: Any, schema: str, tables: Optional[List[str]]) -> Optional[List[str]]:
     """Check that the tables specified exists in the database."""
     if tables is None or len(tables) == 0:
         return None
     all_tables = set(inspector.get_table_names(schema))
     unknown_tables = set(tables) - all_tables
     if len(unknown_tables) > 0:
         print("Tables not found in database:")
         print("\t" + "\n\t".join(unknown_tables))
-        sys.exit()
+        sys.exit(EXIT_CODE_ARGS)
     return tables
 
 
 def check_table_params(ctx: click.Context, param: Union[click.Option, click.Parameter], value: List[str]) -> List[str]:
     """Check that 'tables' have been specified if 'include-dependent-tables' CLI is provided."""
     assert param.name == 'tables'
     other_flag = 'include_dependent_tables'
@@ -317,15 +324,15 @@
     config_per_table = None
     if config_file_name is not None:
         try:
             config_per_table = load_config_for_tables(config_file_name)
             validate_table_configs_with_schema(inspector, schema, config_per_table)
         except ConfigInvalidException as exc:
             print(exc)
-            sys.exit()
+            sys.exit(EXIT_CODE_EXC)
     return config_per_table
 
 
 def generate_single_table_config(directory: str, tables: List[str],
                                  config_per_table: Optional[Dict[str, Any]]
                                  ) -> Tuple[List[str], List[str], Dict[str, Any]]:
     """Create a fake config such that all files found in the directory are subsets for the given table."""
@@ -434,14 +441,15 @@
         def export_tables(conn: Any) -> Tuple[int, int]:
             return db_export.export_tables_per_config(conn, inspector, schema, directory, cast(List[str], tables),
                                                       config_per_table=config_per_table)
         table_count, file_count = run_in_session(engine, export_tables)
         print("Exported {} tables to {} files".format(table_count, file_count))
     except Exception as exc:
         logging.exception(exc)
+        sys.exit(EXIT_CODE_EXC)
     finally:
         if engine is not None:
             engine.dispose()
 
 
 @click.command(name="import")
 @decorate(DB_CONNECT_OPTIONS)
@@ -479,33 +487,34 @@
         table_graph = db_graph.build_fk_dependency_graph(inspector, schema, tables=None)
         tables = validate_tables(inspector, schema, tables)
         if include_dependent_tables and tables:
             tables = list(db_graph.get_all_dependent_tables(table_graph, tables))
 
         if single_table and (tables is None or len(tables) == 0):
             print("One table has to be specified when using the --single-table option")
-            sys.exit()
+            sys.exit(EXIT_CODE_ARGS)
         tables = cast(List[str], tables)
         if single_table and len(tables) > 1:
             print("Only one table can be specified when using the --single-table option")
-            sys.exit()
+            sys.exit(EXIT_CODE_ARGS)
 
         config_per_table = load_table_config_or_exit(inspector, schema, config)
         if single_table:
             import_files, dest_tables, config_per_table = generate_single_table_config(directory, tables,
                                                                                        config_per_table)
         else:
             import_files, dest_tables = get_import_files_and_tables(directory, tables, config_per_table)
         run_in_session(engine, lambda conn:
                        import_all_new(conn, inspector, schema, import_files, dest_tables,
                                       config_per_table=config_per_table,
                                       suspend_foreign_keys=disable_foreign_keys,
                                       fail_on_warning=not ignore_cycles))
     except Exception as exc:
         logging.exception(exc)
+        sys.exit(EXIT_CODE_EXC)
     finally:
         if engine is not None:
             engine.dispose()
 
 
 @click.command(context_settings=dict(max_content_width=120))
 @click.option('--engine', '-e', help="Type of database engine.", default='postgresql', show_default=True)
@@ -543,14 +552,15 @@
         db_url = generate_url(uri, dbname, host, port, username, password, type=engine)
         _engine = sqlalchemy.create_engine(db_url)
         db_inspect.main(_engine, schema,
                         warnings, list_tables, table_details, partition,
                         cycles, insert_order, export_graph, transferable)
     except Exception as exc:
         logging.exception(exc)
+        sys.exit(EXIT_CODE_EXC)
     finally:
         if _engine is not None:
             _engine.dispose()
 
 
 # Typer/Click combination object
 # cast() needed because Type is incorrectly defined in library?
```

### Comparing `pgmerge-1.9.0/pgmerge/tables_config_schema.yml` & `pgmerge-1.9.1/pgmerge/tables_config_schema.yml`

 * *Files identical despite different names*

### Comparing `pgmerge-1.9.0/pgmerge/tests/test_db.py` & `pgmerge-1.9.1/pgmerge/tests/test_db.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,102 +1,110 @@
-"""
-pgmerge - a PostgreSQL data import and merge utility
-
-Copyright 2018-2021 Simon Muller (samullers@gmail.com)
-"""
-import os
-import unittest
-from contextlib import contextmanager
-
-import sqlalchemy
-import psycopg2.extensions as psyext
-
-
-@contextmanager
-def create_table(engine, table):
-    table.create(engine, checkfirst=True)
-    try:
-        yield
-    finally:
-        table.drop(engine, checkfirst=False)
-
-
-def find_open_connections(connection):
-    return connection.execute("SELECT * FROM pg_stat_activity").fetchall()
-
-
-class TestDB(unittest.TestCase):
-    """
-    Class for setting up a test database and handling connections to it.
-
-    Requires environment variable with connection details/URL to database, e.g.:
-        DB_TEST_URL=postgres://postgres:password@localhost:5432/
-    User has to have create database permissions.
-    """
-
-    env_var = "DB_TEST_URL"
-    url = ''
-    db_name = 'testdb'
-    initial_db = 'template1'
-
-    @classmethod
-    def setUpClass(cls):
-        # Create class variables to be re-used between tests
-        cls.create_db_engine = None
-        cls.engine = None
-        cls.url = os.getenv(cls.env_var)
-        if not cls.url:
-            assert False, "No database URL set in '{}'".format(cls.env_var)
-        try:
-            cls.create_db(cls.db_name)
-        except Exception as err:
-            cls.drop_db(cls.db_name)
-            raise err
-
-    @classmethod
-    def tearDownClass(cls):
-        cls.drop_db(cls.db_name)
-
-    @classmethod
-    def create_db(cls, db_name):
-        # Open connection to template database (could build url with sqlalchemy.engine.url.URL)
-        cls.create_db_engine = sqlalchemy.create_engine(cls.url + cls.initial_db)
-        with cls.create_db_engine.connect() as conn:
-            conn.connection.set_isolation_level(psyext.ISOLATION_LEVEL_AUTOCOMMIT)
-            conn.execute("DROP DATABASE IF EXISTS " + db_name)
-            conn.execute("CREATE DATABASE " + db_name)
-            # conn.connection.set_isolation_level(psyext.ISOLATION_LEVEL_DEFAULT)
-        # self.connection.close()
-        cls.create_db_engine.dispose()
-        cls.create_db_engine = None
-
-        cls.engine = sqlalchemy.create_engine(cls.url + db_name)
-
-    @classmethod
-    def drop_db(cls, db_name):
-        if cls.engine is not None:
-            cls.engine.dispose()
-            cls.engine = None
-
-        cls.create_db_engine = sqlalchemy.create_engine(cls.url + cls.initial_db)
-        with cls.create_db_engine.connect() as conn:
-            conn.connection.set_isolation_level(psyext.ISOLATION_LEVEL_AUTOCOMMIT)
-            # print(find_open_connections(conn))
-            conn.execute("DROP DATABASE IF EXISTS " + db_name)
-            # self.connection.connection.set_isolation_level(psyext.ISOLATION_LEVEL_DEFAULT)
-        # self.connection.close()
-        cls.create_db_engine.dispose()
-
-    def setUp(self):
-        # Open connection before each test
-        self.open_db_conn()
-
-    def tearDown(self):
-        # Close connection after each test
-        self.close_db_conn()
-
-    def open_db_conn(self):
-        self.connection = self.engine.connect()
-
-    def close_db_conn(self):
-        self.connection.close()
-        self.connection = None
+"""
+pgmerge - a PostgreSQL data import and merge utility
+
+Copyright 2018-2021 Simon Muller (samullers@gmail.com)
+"""
+import os
+import unittest
+from contextlib import contextmanager
+
+from sqlalchemy import create_engine, text
+import psycopg2.extensions as psyext
+
+
+@contextmanager
+def create_table(engine, table):
+    table.create(engine, checkfirst=True)
+    try:
+        yield
+    finally:
+        table.drop(engine, checkfirst=False)
+
+
+def find_open_connections(connection):
+    return connection.execute(text("SELECT * FROM pg_stat_activity")).fetchall()
+
+
+class TestDB(unittest.TestCase):
+    """
+    Class for setting up a test database and handling connections to it.
+
+    Requires environment variable with connection details/URL to database, e.g.:
+        DB_TEST_URL=postgres://postgres:password@localhost:5432/
+    User has to have create database permissions.
+    """
+
+    env_var = "DB_TEST_URL"
+    url = ''
+    db_name = 'testdb'
+    initial_db = 'template1'
+
+    @classmethod
+    def setUpClass(cls):
+        # Create class variables to be re-used between tests
+        cls.create_db_engine = None
+        cls.engine = None
+        cls.url = os.getenv(cls.env_var)
+        if not cls.url:
+            assert False, "No database URL set in '{}'".format(cls.env_var)
+        try:
+            cls.create_db(cls.db_name)
+        except Exception as err:
+            cls.drop_db(cls.db_name)
+            raise err
+
+    @classmethod
+    def tearDownClass(cls):
+        cls.drop_db(cls.db_name)
+
+    @classmethod
+    def create_db(cls, db_name):
+        # Open connection to template database (could build url with sqlalchemy.engine.url.URL)
+        cls.create_db_engine = create_engine(cls.url + cls.initial_db)
+        with cls.create_db_engine.begin() as conn:
+            conn.connection.set_isolation_level(psyext.ISOLATION_LEVEL_AUTOCOMMIT)
+            conn.execute(text("DROP DATABASE IF EXISTS " + db_name))
+            conn.execute(text("CREATE DATABASE " + db_name))
+            # conn.connection.set_isolation_level(psyext.ISOLATION_LEVEL_DEFAULT)
+        # self.connection.close()
+        cls.create_db_engine.dispose()
+        cls.create_db_engine = None
+
+        cls.engine = create_engine(cls.url + db_name)
+
+    @classmethod
+    def drop_db(cls, db_name):
+        if cls.engine is not None:
+            cls.engine.dispose()
+            cls.engine = None
+
+        cls.create_db_engine = create_engine(cls.url + cls.initial_db)
+        with cls.create_db_engine.connect() as conn:
+            conn.connection.set_isolation_level(psyext.ISOLATION_LEVEL_AUTOCOMMIT)
+            # print(find_open_connections(conn))
+            with conn.begin():
+                conn.execute(text("DROP DATABASE IF EXISTS " + db_name))
+            # self.connection.connection.set_isolation_level(psyext.ISOLATION_LEVEL_DEFAULT)
+        # self.connection.close()
+        cls.create_db_engine.dispose()
+
+    def setUp(self):
+        # Open connection before each test
+        self.open_db_conn()
+
+    def tearDown(self):
+        # Close connection after each test
+        self.close_db_conn()
+
+    def open_db_conn(self):
+        self.connection = self.engine.connect()
+
+    def close_db_conn(self):
+        self.connection.close()
+        self.connection = None
+
+    def run_query(self, sql_stmt):
+        """Helper function to execute raw SQL statements"""
+        result = self.connection.execute(sql_stmt)
+        all = result.fetchall()
+        result.close()
+        return all
```

### Comparing `pgmerge-1.9.0/pgmerge/utils.py` & `pgmerge-1.9.1/pgmerge/utils.py`

 * *Files identical despite different names*

### Comparing `pgmerge-1.9.0/pyproject.toml` & `pgmerge-1.9.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pgmerge"
-version = "1.9.0"
+version = "1.9.1"
 description = "PostgreSQL data import/export utility"
 authors = ["Simon Muller <samullers@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/samuller/pgmerge"
 repository = "https://github.com/samuller/pgmerge"
 keywords = ["postgresql", "csv", "import", "export"]
 classifiers = [
@@ -40,11 +40,14 @@
 flake8-docstrings = "^1.6.0"
 mypy = "^0.910"
 
 [tool.pytest.ini_options]
 testpaths = [
     "pgmerge/tests"
 ]
+# Capture logging and print to stdout while running tests
+log_cli = true
+log_cli_level = "INFO"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pgmerge-1.9.0/setup.py` & `pgmerge-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'typer>=0.4.0,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['pgmerge = pgmerge.pgmerge:cli_app']}
 
 setup_kwargs = {
     'name': 'pgmerge',
-    'version': '1.9.0',
+    'version': '1.9.1',
     'description': 'PostgreSQL data import/export utility',
     'long_description': "# pgmerge - a PostgreSQL data import and merge utility\n\n[![Build Status](https://github.com/samuller/pgmerge/workflows/tests/badge.svg)](https://github.com/samuller/pgmerge/actions)\n[![PyPI Version](https://badge.fury.io/py/pgmerge.svg)](https://badge.fury.io/py/pgmerge)\n[![Code Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/samuller/3c84321138784d39b31a02d7fe93b31d/raw/badge-coverage.json)](https://github.com/samuller/pgmerge/actions)\n\nThis utility's main purpose is to manage a set of CSV files that correspond with tables in a PostgreSQL database. Each of these CSV files can then be *merged* into their table, meaning that the following process will occur (also called an *upsert* operation):\n\n* Rows whose primary key don't yet exist in the table will be imported.\n* When the primary key already exists, row values will be updated.\n* Rows that are missing or unchanged will be ignored.\n\npgmerge can then also export data in the *same format* expected for import.\n\nThese features allow you to move data between databases with the same schema to keep them up to date and in sync, although it does not cover handling deleted data.\n\n    $ pgmerge --help\n    Usage: pgmerge [OPTIONS] COMMAND [ARGS]...\n\n    Merges data in CSV files into a Postgresql database.\n\n    Options:\n    --version  Show the version and exit.\n    --help     Show this message and exit.\n\n    Commands:\n    export  Export each table to a CSV file.\n    import  Import/merge each CSV file into a table.\n    inspect  Inspect database schema in various ways.\n\n### Import\n\n    $ pgmerge import --help\n    Usage: pgmerge import [OPTIONS] DIRECTORY [TABLES]...\n\n    Import/merge each CSV file into a table.\n\n    All CSV files need the same name as their matching table and have to be located\n    in the given directory. If one or more tables are specified then only they will\n    be used, otherwise all tables found will be selected.\n\n    Options:\n    -d, --dbname TEXT               Database name to connect to.  [required]\n    -h, --host TEXT                 Database server host or socket directory.\n                                    [default: localhost]\n    -p, --port TEXT                 Database server port.  [default: 5432]\n    -U, --username TEXT             Database user name.  [default: postgres]\n    -s, --schema TEXT               Database schema to use.  [default: public]\n    -w, --no-password               Never prompt for password (e.g. peer\n                                    authentication).\n    -W, --password TEXT             Database password (default is to prompt for\n                                    password or read config).\n    -L, --uri TEXT                  Connection URI can be used instead of specifying\n                                    parameters separately (also sets --no-password).\n    -f, --ignore-cycles             Don't stop import when cycles are detected in\n                                    schema (will still fail if there are cycles in\n                                    data)\n    -F, --disable-foreign-keys      Disable foreign key constraint checking during\n                                    import (necessary if you have cycles, but requires\n                                    superuser rights).\n    -c, --config PATH               Config file for customizing how tables are\n                                    imported/exported.\n    -i, --include-dependent-tables  When selecting specific tables, also include all\n                                    tables on which they depend due to foreign key\n                                    constraints.\n    --help                          Show this message and exit.\n\n## Installation\n\n> WARNING: the reliability of this utility is not guaranteed and loss or corruption of data is always a possibility.\n\n### Install from PyPI\n\nWith `Python 3` installed on your system, you can run:\n\n    pip install pgmerge\n\n(your `pip --version` has to be 9.0 or greater). To test that installation worked, run:\n\n    pgmerge --help\n\nand you can uninstall at any time with:\n\n    pip uninstall pgmerge\n\n### Install from Github\n\nTo install the newest code directly from Github:\n\n    pip install git+https://github.com/samuller/pgmerge\n\n### Issues\n\nIf you have trouble installing and you're running a Debian-based Linux that uses `Python 2` as its system default, then you might need to run:\n\n    sudo apt install libpq-dev python3-pip python3-setuptools\n    sudo -H pip3 install pgmerge\n",
     'author': 'Simon Muller',
     'author_email': 'samullers@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/samuller/pgmerge',
```

### Comparing `pgmerge-1.9.0/PKG-INFO` & `pgmerge-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgmerge
-Version: 1.9.0
+Version: 1.9.1
 Summary: PostgreSQL data import/export utility
 Home-page: https://github.com/samuller/pgmerge
 Keywords: postgresql,csv,import,export
 Author: Simon Muller
 Author-email: samullers@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```


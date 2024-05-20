# Comparing `tmp/subsetter-0.3.0.tar.gz` & `tmp/subsetter-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subsetter-0.3.0.tar", last modified: Wed May  1 07:01:45 2024, max compression
+gzip compressed data, was "subsetter-0.3.1.tar", last modified: Mon May 20 01:31:55 2024, max compression
```

## Comparing `subsetter-0.3.0.tar` & `subsetter-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-05-01 07:01:45.003337 subsetter-0.3.0/
--rw-rw-r--   0 msg       (1000) msg       (1000)     1493 2023-08-14 00:07:05.000000 subsetter-0.3.0/LICENSE
--rw-r--r--   0 msg       (1000) msg       (1000)     5260 2024-05-01 07:01:45.003337 subsetter-0.3.0/PKG-INFO
--rw-rw-r--   0 msg       (1000) msg       (1000)     4234 2024-04-26 07:16:28.000000 subsetter-0.3.0/README.md
--rw-rw-r--   0 msg       (1000) msg       (1000)     1406 2024-03-25 08:03:09.000000 subsetter-0.3.0/pyproject.toml
--rw-rw-r--   0 msg       (1000) msg       (1000)     1108 2024-05-01 07:01:45.003337 subsetter-0.3.0/setup.cfg
-drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-05-01 07:01:44.999337 subsetter-0.3.0/subsetter/
--rw-rw-r--   0 msg       (1000) msg       (1000)        0 2023-08-14 00:07:05.000000 subsetter-0.3.0/subsetter/__init__.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     9844 2024-04-22 04:48:05.000000 subsetter-0.3.0/subsetter/__main__.py
--rw-rw-r--   0 msg       (1000) msg       (1000)       22 2024-04-23 01:12:27.000000 subsetter-0.3.0/subsetter/_version.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     3543 2024-04-15 04:56:03.000000 subsetter-0.3.0/subsetter/common.py
--rw-rw-r--   0 msg       (1000) msg       (1000)    20926 2024-03-25 08:26:43.000000 subsetter-0.3.0/subsetter/filters.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     9676 2024-04-24 08:31:13.000000 subsetter-0.3.0/subsetter/metadata.py
--rw-rw-r--   0 msg       (1000) msg       (1000)    11194 2024-04-22 04:48:05.000000 subsetter-0.3.0/subsetter/plan_model.py
--rw-rw-r--   0 msg       (1000) msg       (1000)    13820 2024-04-30 04:49:33.000000 subsetter-0.3.0/subsetter/planner.py
--rw-rw-r--   0 msg       (1000) msg       (1000)    21639 2024-04-30 04:49:47.000000 subsetter-0.3.0/subsetter/sampler.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     4859 2024-05-01 06:44:40.000000 subsetter-0.3.0/subsetter/solver.py
-drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-05-01 07:01:45.003337 subsetter-0.3.0/subsetter.egg-info/
--rw-r--r--   0 msg       (1000) msg       (1000)     5260 2024-05-01 07:01:44.000000 subsetter-0.3.0/subsetter.egg-info/PKG-INFO
--rw-rw-r--   0 msg       (1000) msg       (1000)      519 2024-05-01 07:01:44.000000 subsetter-0.3.0/subsetter.egg-info/SOURCES.txt
--rw-rw-r--   0 msg       (1000) msg       (1000)        1 2024-05-01 07:01:44.000000 subsetter-0.3.0/subsetter.egg-info/dependency_links.txt
--rw-rw-r--   0 msg       (1000) msg       (1000)       54 2024-05-01 07:01:44.000000 subsetter-0.3.0/subsetter.egg-info/entry_points.txt
--rw-rw-r--   0 msg       (1000) msg       (1000)      133 2024-05-01 07:01:44.000000 subsetter-0.3.0/subsetter.egg-info/requires.txt
--rw-rw-r--   0 msg       (1000) msg       (1000)       10 2024-05-01 07:01:44.000000 subsetter-0.3.0/subsetter.egg-info/top_level.txt
-drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-05-01 07:01:45.003337 subsetter-0.3.0/tests/
--rw-rw-r--   0 msg       (1000) msg       (1000)     7317 2024-03-25 07:55:35.000000 subsetter-0.3.0/tests/test_filters.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     1686 2024-04-22 04:48:05.000000 subsetter-0.3.0/tests/test_live.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     5203 2024-05-01 06:38:45.000000 subsetter-0.3.0/tests/test_solver.py
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-05-20 01:31:55.968190 subsetter-0.3.1/
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1493 2023-08-14 00:07:05.000000 subsetter-0.3.1/LICENSE
+-rw-r--r--   0 msg       (1000) msg       (1000)     7407 2024-05-20 01:31:55.968190 subsetter-0.3.1/PKG-INFO
+-rw-rw-r--   0 msg       (1000) msg       (1000)     6134 2024-05-05 19:57:59.000000 subsetter-0.3.1/README.md
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1406 2024-03-25 08:03:09.000000 subsetter-0.3.1/pyproject.toml
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1239 2024-05-20 01:31:55.968190 subsetter-0.3.1/setup.cfg
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-05-20 01:31:55.964190 subsetter-0.3.1/subsetter/
+-rw-rw-r--   0 msg       (1000) msg       (1000)        0 2023-08-14 00:07:05.000000 subsetter-0.3.1/subsetter/__init__.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    10187 2024-05-06 06:16:14.000000 subsetter-0.3.1/subsetter/__main__.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)       22 2024-05-20 01:25:53.000000 subsetter-0.3.1/subsetter/_version.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     4319 2024-05-13 06:21:18.000000 subsetter-0.3.1/subsetter/common.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    20926 2024-03-25 08:26:43.000000 subsetter-0.3.1/subsetter/filters.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     8125 2024-05-13 06:21:18.000000 subsetter-0.3.1/subsetter/metadata.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    11194 2024-04-22 04:48:05.000000 subsetter-0.3.1/subsetter/plan_model.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    15446 2024-05-13 06:21:18.000000 subsetter-0.3.1/subsetter/planner.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    25832 2024-05-20 01:12:33.000000 subsetter-0.3.1/subsetter/sampler.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     4859 2024-05-05 21:33:29.000000 subsetter-0.3.1/subsetter/solver.py
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-05-20 01:31:55.964190 subsetter-0.3.1/subsetter.egg-info/
+-rw-r--r--   0 msg       (1000) msg       (1000)     7407 2024-05-20 01:31:55.000000 subsetter-0.3.1/subsetter.egg-info/PKG-INFO
+-rw-rw-r--   0 msg       (1000) msg       (1000)      519 2024-05-20 01:31:55.000000 subsetter-0.3.1/subsetter.egg-info/SOURCES.txt
+-rw-rw-r--   0 msg       (1000) msg       (1000)        1 2024-05-20 01:31:55.000000 subsetter-0.3.1/subsetter.egg-info/dependency_links.txt
+-rw-rw-r--   0 msg       (1000) msg       (1000)       54 2024-05-20 01:31:55.000000 subsetter-0.3.1/subsetter.egg-info/entry_points.txt
+-rw-rw-r--   0 msg       (1000) msg       (1000)      266 2024-05-20 01:31:55.000000 subsetter-0.3.1/subsetter.egg-info/requires.txt
+-rw-rw-r--   0 msg       (1000) msg       (1000)       10 2024-05-20 01:31:55.000000 subsetter-0.3.1/subsetter.egg-info/top_level.txt
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-05-20 01:31:55.964190 subsetter-0.3.1/tests/
+-rw-rw-r--   0 msg       (1000) msg       (1000)     7317 2024-03-25 07:55:35.000000 subsetter-0.3.1/tests/test_filters.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     2333 2024-05-13 06:21:18.000000 subsetter-0.3.1/tests/test_live.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     5203 2024-05-01 06:38:45.000000 subsetter-0.3.1/tests/test_solver.py
```

### Comparing `subsetter-0.3.0/LICENSE` & `subsetter-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `subsetter-0.3.0/PKG-INFO` & `subsetter-0.3.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subsetter
-Version: 0.3.0
+Version: 0.3.1
 Summary: MySQL database subsetting CLI tool
 Home-page: http://github.com/msg555/subsetter/
 Author: Mark Gordon
 Author-email: msg555@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -18,18 +18,22 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sqlalchemy[mypy]~=2.0
 Requires-Dist: pydantic~=2.6
 Requires-Dist: pyyaml~=6.0
 Requires-Dist: faker~=19.3
 Requires-Dist: typing-extensions
-Provides-Extra: mysql
-Requires-Dist: pymysql~=1.0; extra == "mysql"
-Provides-Extra: postgres
-Requires-Dist: psycopg2-binary~=2.0; extra == "postgres"
+Provides-Extra: all
+Requires-Dist: sqlalchemy[postgresql_psycopg2binary,pymysql]; extra == "all"
+Provides-Extra: pymysql
+Requires-Dist: sqlalchemy[pymysql]; extra == "pymysql"
+Provides-Extra: postgresql
+Requires-Dist: sqlalchemy[postgresql]; extra == "postgresql"
+Provides-Extra: postgresql-psycopg2binary
+Requires-Dist: sqlalchemy[postgresql_psycopg2binary]; extra == "postgresql-psycopg2binary"
 
 # Subsetter
 
 Subsetter is a Python utility that can be used for subsetting portions of
 relational databases. _Subsetting_ is the action extracting a smaller set of rows
 from your database that still maintain expected foreign-key relationships
 between your data. This can be useful for testing against a small but
@@ -115,7 +119,44 @@
 create a semantically consistent large dataset from your existing data. The
 sampler has support for this by setting the multiplicity factor.
 
 Multiplicity works by creating multiple copies of your sampled dataset in your
 output database. To ensure these datasets do not collide it remaps all foreign
 keys into a new key-space. Note that this process assumes your foreign keys are
 opaque integers identifiers.
+
+# FAQ
+
+## How do multiple targets work
+
+When using multiple targets each target table will be sampled entirely
+independently unless another target table directly or indirectly depends on some
+rows from it through a series of foreign keys. In the later case the subsetter
+will sample a union of the rows from the independently sampling of the table and
+those rows that other targets depend on.
+
+## How does the subsetter use foreign keys?
+
+The subsetter uses the foreign keys present in the database schema to understand
+relationships between data and generate a sampling plan. Foreign key
+relationships can be followed in both directions if need be. For example,
+suppose there was a `users` and an `orders` table where `orders` had a foreign key
+to the `users` table.
+
+If `users` was sampled first the subsetter would sample `orders` from `users` by
+sampling all rows from `orders` such that their corresponding user row existed.
+This represents the _maximal_ set of rows that can be included without violating
+foreign key constraints.
+
+Otherwise if `orders` was sampled first the subsetter would sample `users` from
+`orders` by sampling all rows from `users` such that they had at least one
+`order`. This represents the _minimal_ set of rows that can be included without
+violating foreign key constraints.
+
+In general the subsetter will always sample tables in an order such that all
+foreign key relationships to previously sampled tables are going in the same
+direction. If they are followed in the forwards direction (as in our first case)
+the subsetter will select the _intersection_ of all rows that obey each foreign
+key relationship. Otherwise if they are followed in the backwards direction (as
+in our second case) the subsetter will select the _union_ of all rows that obey
+each foreign key relationship. This strategy ensures no foreign key
+relationships are violated in the sampled data.
```

### Comparing `subsetter-0.3.0/README.md` & `subsetter-0.3.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -86,7 +86,44 @@
 create a semantically consistent large dataset from your existing data. The
 sampler has support for this by setting the multiplicity factor.
 
 Multiplicity works by creating multiple copies of your sampled dataset in your
 output database. To ensure these datasets do not collide it remaps all foreign
 keys into a new key-space. Note that this process assumes your foreign keys are
 opaque integers identifiers.
+
+# FAQ
+
+## How do multiple targets work
+
+When using multiple targets each target table will be sampled entirely
+independently unless another target table directly or indirectly depends on some
+rows from it through a series of foreign keys. In the later case the subsetter
+will sample a union of the rows from the independently sampling of the table and
+those rows that other targets depend on.
+
+## How does the subsetter use foreign keys?
+
+The subsetter uses the foreign keys present in the database schema to understand
+relationships between data and generate a sampling plan. Foreign key
+relationships can be followed in both directions if need be. For example,
+suppose there was a `users` and an `orders` table where `orders` had a foreign key
+to the `users` table.
+
+If `users` was sampled first the subsetter would sample `orders` from `users` by
+sampling all rows from `orders` such that their corresponding user row existed.
+This represents the _maximal_ set of rows that can be included without violating
+foreign key constraints.
+
+Otherwise if `orders` was sampled first the subsetter would sample `users` from
+`orders` by sampling all rows from `users` such that they had at least one
+`order`. This represents the _minimal_ set of rows that can be included without
+violating foreign key constraints.
+
+In general the subsetter will always sample tables in an order such that all
+foreign key relationships to previously sampled tables are going in the same
+direction. If they are followed in the forwards direction (as in our first case)
+the subsetter will select the _intersection_ of all rows that obey each foreign
+key relationship. Otherwise if they are followed in the backwards direction (as
+in our second case) the subsetter will select the _union_ of all rows that obey
+each foreign key relationship. This strategy ensures no foreign key
+relationships are violated in the sampled data.
```

### Comparing `subsetter-0.3.0/pyproject.toml` & `subsetter-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `subsetter-0.3.0/setup.cfg` & `subsetter-0.3.1/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -27,18 +27,22 @@
 	sqlalchemy[mypy] ~= 2.0
 	pydantic ~= 2.6
 	pyyaml ~= 6.0
 	faker ~= 19.3
 	typing-extensions
 
 [options.extras_require]
-mysql = 
-	pymysql ~= 1.0
-postgres = 
-	psycopg2-binary ~= 2.0
+all = 
+	sqlalchemy[pymysql,postgresql_psycopg2binary]
+pymysql = 
+	sqlalchemy[pymysql]
+postgresql = 
+	sqlalchemy[postgresql]
+postgresql_psycopg2binary = 
+	sqlalchemy[postgresql_psycopg2binary]
 
 [options.package_data]
 subsetter = 
 	py.typed
 
 [options.entry_points]
 console_scripts =
```

### Comparing `subsetter-0.3.0/subsetter/__main__.py` & `subsetter-0.3.1/subsetter/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,21 @@
     parser.add_argument(
         "--truncate",
         action="store_const",
         const=True,
         default=False,
         help="Truncate existing output before sampling",
     )
+    parser.add_argument(
+        "--create",
+        action="store_const",
+        const=True,
+        default=False,
+        help="Create tables in destination from source if missing",
+    )
     output_parsers = parser.add_subparsers(
         dest="output",
         required=False,
         help="Configure sampling output destination",
     )
 
     mysql_parser = output_parsers.add_parser(
@@ -265,15 +272,19 @@
             "Could not open plan file %r: %s",
             args.plan,
             exc,
             exc_info=args.verbose > 1,
         )
         sys.exit(1)
 
-    Sampler(_get_sample_config(args)).sample(plan, truncate=args.truncate)
+    Sampler(_get_sample_config(args)).sample(
+        plan,
+        truncate=args.truncate,
+        create=args.create,
+    )
 
 
 def _main_subset(args):
     planner_config = _get_plan_config(args)
     planner_config.source = _get_source_database_config(
         args, overlay=planner_config.source
     )
@@ -281,17 +292,20 @@
     sampler_config.source = planner_config.source
     plan = Planner(planner_config).plan()
     Sampler(sampler_config).sample(plan, truncate=args.truncate)
 
 
 def main():
     args = _parse_args()
+    logging_format = "%(levelname)s\t%(message)s"
+    if args.verbose > 0:
+        logging_format = "%(asctime)s\t%(levelname)s\t%(message)s"
     logging.basicConfig(
         level=logging.DEBUG if args.verbose > 0 else logging.INFO,
-        format="%(asctime)s %(levelname)s %(message)s",
+        format=logging_format,
     )
     logging.getLogger("faker").setLevel(logging.INFO)
 
     with logging_redirect_tqdm():
         try:
             if args.action == "plan":
                 _main_plan(args)
@@ -299,15 +313,15 @@
                 _main_sample(args)
             elif args.action == "subset":
                 _main_subset(args)
             else:
                 raise RuntimeError("Unknown action")
         except Exception as exc:  # pylint: disable=broad-exception-caught
             LOGGER.error(
-                "Unexpected error %s: %s",
+                "%s: %s",
                 type(exc).__name__,
                 exc,
                 exc_info=args.verbose > 1,
             )
             sys.exit(1)
```

### Comparing `subsetter-0.3.0/subsetter/common.py` & `subsetter-0.3.1/subsetter/common.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import sqlalchemy as sa
 from pydantic import BaseModel
 
 DatabaseDialect = Literal[
     "mysql",
     "postgres",
+    "sqlite",
 ]
 
 LOGGER = logging.getLogger(__name__)
 DEFAULT_DIALECT: Literal["mysql"] = "mysql"
 
 # pylint: disable=unused-argument
 
@@ -33,17 +34,17 @@
     username: Optional[str] = None,
     password: Optional[str] = None,
 ) -> sa.engine.URL:
     if env_prefix is not None:
         dialect = dialect or os.getenv(f"{env_prefix}DIALECT", None)  # type: ignore
         host = host or os.getenv(f"{env_prefix}HOST", "localhost")
         port = port or int(os.getenv(f"{env_prefix}PORT", "0"))
-        database = database or os.getenv(f"{env_prefix}DATABASE", "")
-        username = username or os.environ[f"{env_prefix}USERNAME"]
-        password = os.environ[f"{env_prefix}PASSWORD"] if password is None else password
+        database = database or os.getenv(f"{env_prefix}DATABASE", None)
+        username = username or os.getenv(f"{env_prefix}USERNAME", None)
+        password = password or os.getenv(f"{env_prefix}PASSWORD", None)
 
     if dialect is None:
         dialect = DEFAULT_DIALECT
         LOGGER.warning("No database dialect selected, defaulting to '%s'", dialect)
 
     extra_kwargs: Dict[str, Any] = {}
     if dialect == "mysql":
@@ -53,21 +54,23 @@
         extra_kwargs["query"] = {"charset": "utf8mb4"}
     elif dialect == "postgres":
         drivername = "postgresql+psycopg2"
         if not port:
             port = 5432
         if database:
             extra_kwargs["database"] = database
+    elif dialect == "sqlite":
+        return sa.engine.URL.create(drivername="sqlite", database=database)
     else:
         raise ValueError(f"Unsupported SQL dialect {dialect!r}")
 
     return sa.engine.URL.create(
         drivername=drivername,
         host=host,
-        port=port or 3306,
+        port=port,
         username=username,
         password=password,
         **extra_kwargs,
     )
 
 
 IsolationLevel = Literal[
@@ -82,15 +85,16 @@
     dialect: Optional[DatabaseDialect] = None
     host: Optional[str] = None
     port: Optional[int] = None
     database: Optional[str] = None
     username: Optional[str] = None
     password: Optional[str] = None
     session_sqls: List[str] = []
-    isolation_level: IsolationLevel = "READ COMMITTED"
+    sqlite_databases: Optional[Dict[str, str]] = {}
+    isolation_level: Optional[IsolationLevel] = None
 
     def database_url(
         self,
         env_prefix: Optional[str] = None,
     ) -> sa.engine.URL:
         return database_url(
             env_prefix=env_prefix,
@@ -102,20 +106,36 @@
             password=self.password,
         )
 
     def database_engine(
         self,
         env_prefix: Optional[str] = None,
     ) -> sa.engine.Engine:
+        if self.isolation_level:
+            isolation_level = self.isolation_level
+        elif self.dialect == "sqlite":
+            isolation_level = "SERIALIZABLE"
+        else:
+            isolation_level = "READ COMMITTED"
         engine = sa.create_engine(
             self.database_url(env_prefix=env_prefix),
-            isolation_level=self.isolation_level,
+            isolation_level=isolation_level,
             pool_pre_ping=True,
         )
 
         @sa.event.listens_for(engine, "connect")
         def _set_session_sqls(dbapi_connection, _):
-            with dbapi_connection.cursor() as cursor:
+            cursor = dbapi_connection.cursor()
+            try:
+                if self.dialect == "sqlite":
+                    for db_alias, db_file in self.sqlite_databases.items():
+                        escaped_db_file = db_file.replace("'", "''")
+                        cursor.execute(
+                            f"ATTACH DATABASE '{escaped_db_file}' as {db_alias}"
+                        )
+
                 for session_sql in self.session_sqls:
                     cursor.execute(session_sql)
+            finally:
+                cursor.close()
 
         return engine
```

### Comparing `subsetter-0.3.0/subsetter/filters.py` & `subsetter-0.3.1/subsetter/filters.py`

 * *Files identical despite different names*

### Comparing `subsetter-0.3.0/subsetter/plan_model.py` & `subsetter-0.3.1/subsetter/plan_model.py`

 * *Files identical despite different names*

### Comparing `subsetter-0.3.0/subsetter/planner.py` & `subsetter-0.3.1/subsetter/planner.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     SQLWhereClauseIn,
     SQLWhereClauseOperator,
     SQLWhereClauseOr,
     SQLWhereClauseRandom,
     SQLWhereClauseSQL,
     SubsetPlan,
 )
-from subsetter.solver import order_graph
+from subsetter.solver import CycleException, order_graph
 
 LOGGER = logging.getLogger(__name__)
 
 
 class PlannerConfig(BaseModel):
     class TargetConfig(BaseModel):
         all_: bool = Field(False, alias="all")
@@ -55,18 +55,22 @@
     select: List[str]
     targets: Dict[str, TargetConfig]
     ignore: List[str] = []
     passthrough: List[str] = []
     ignore_fks: List[IgnoreFKConfig] = []
     extra_fks: List[ExtraFKConfig] = []
     infer_foreign_keys: bool = False
-    normalize_foreign_keys: bool = False
 
 
 class Planner:
+    """
+    Class responsible for taking in a plan configuration and a source database
+    schema and producing a subsetting strategy.
+    """
+
     def __init__(self, config: PlannerConfig) -> None:
         self.config = config
         self.engine = self.config.source.database_engine(env_prefix="SUBSET_SOURCE_")
         self.meta: DatabaseMetadata
         self.ignore_tables = {parse_table_name(table) for table in config.ignore}
         self.passthrough_tables = {
             parse_table_name(table) for table in config.passthrough
@@ -88,18 +92,19 @@
         for extra_table in extra_tables:
             LOGGER.info(
                 "Selected additional table %s.%s referenced by foreign keys",
                 extra_table[0],
                 extra_table[1],
             )
 
+        return self._plan_internal()
+
+    def _plan_internal(self) -> SubsetPlan:
         if self.config.infer_foreign_keys:
             self.meta.infer_missing_foreign_keys()
-        if self.config.normalize_foreign_keys:
-            self.meta.normalize_foreign_keys()
         self._remove_ignore_fks()
         self._add_extra_fks()
         self._check_ignore_tables()
         self._check_passthrough_tables()
 
         order = self._solve_order()
         self.meta.compute_reverse_keys()
@@ -134,15 +139,26 @@
         satisfies all constraints.
         """
         source = ""
         graph = self.meta.as_graph(
             ignore_tables=self.passthrough_tables | self.ignore_tables
         )
         graph[source] = set(self.config.targets)
-        order = order_graph(graph, source)[1:]
+
+        for target in self.config.targets:
+            if target not in graph:
+                raise ValueError(f"Cannot target unselected table {target}")
+
+        try:
+            order = order_graph(graph, source)[1:]
+        except CycleException as exc:
+            cycle_text = "->".join([*exc.cycle, exc.cycle[0]])  # type: ignore
+            raise ValueError(
+                f"Cannot create plan due to foreign key cycle {cycle_text}"
+            ) from exc
 
         order_st = set(order)
         for table in graph:
             if table and table not in order_st:
                 LOGGER.warning(
                     "warning: no relationship found to %s, ignoring table", table
                 )
@@ -257,18 +273,42 @@
             fk
             for fk in table.rev_foreign_keys
             if (fk.dst_schema, fk.dst_table) in processed
         )
 
         # Make sure the solver gave us something reasonable
         assert not foreign_keys or not rev_foreign_keys
+        assert target or foreign_keys or rev_foreign_keys
+
+        # If we're a target we can only have reverse foreign key constraints.
+        # If we're selecting all rows we can just ignore them.
         if target:
             assert not foreign_keys
             if target.all_:
                 rev_foreign_keys.clear()
+            if rev_foreign_keys:
+                LOGGER.debug(
+                    "Sampling %s as union of target parameters and references from %s",
+                    table,
+                    [f"{fk.dst_schema}.{fk.dst_table}" for fk in rev_foreign_keys],
+                )
+            else:
+                LOGGER.debug("Targetting %s", table)
+        elif foreign_keys:
+            LOGGER.debug(
+                "Sampling %s as intersection of references from %s",
+                table,
+                [f"{fk.dst_schema}.{fk.dst_table}" for fk in foreign_keys],
+            )
+        else:
+            LOGGER.debug(
+                "Sampling %s as union of references from %s",
+                table,
+                [f"{fk.dst_schema}.{fk.dst_table}" for fk in rev_foreign_keys],
+            )
 
         fk_constraints = [
             SQLWhereClauseIn(
                 type_="in",
                 columns=list(fk.columns),
                 values=SQLStatementSelect(
                     type_="select",
@@ -295,26 +335,35 @@
                 conditions=fk_constraints,
             )
 
         conf_constraints = self.config.table_constraints.get(
             f"{table.schema}.{table.name}", []
         )
         conf_constraints_sql: List[SQLWhereClause] = []
-        all_columns = {column.name for column in table.table_obj.columns}
+        if conf_constraints and rev_foreign_keys:
+            raise ValueError(
+                f"Cannot apply table constraints to {table} without violating "
+                "foreign key constraints of previously sampled tables",
+            )
+
         for conf_constraint in conf_constraints:
-            if conf_constraint.column in all_columns:
-                conf_constraints_sql.append(
-                    SQLWhereClauseOperator(
-                        type_="operator",
-                        operator=conf_constraint.operator,
-                        column=conf_constraint.column,
-                        value=conf_constraint.value,
-                    )
+            if conf_constraint.column not in table.table_obj.columns:
+                raise ValueError(
+                    "Table {table} has no column {conf_constraint.column!r} for table constraint",
                 )
 
+            conf_constraints_sql.append(
+                SQLWhereClauseOperator(
+                    type_="operator",
+                    operator=conf_constraint.operator,
+                    column=conf_constraint.column,
+                    value=conf_constraint.value,
+                )
+            )
+
         # Calculate initial foreign-key / config constraint statement
         statements: List[SQLStatementSelect] = [
             SQLStatementSelect(
                 type_="select",
                 from_=SQLTableIdentifier(
                     table_schema=table.schema,
                     table_name=table.name,
@@ -344,27 +393,22 @@
                     SQLWhereClauseSQL(
                         type_="sql",
                         sql=target.sql,
                     )
                 )
 
             for column, patterns in target.like.items():
-                target_constraints.append(
-                    SQLWhereClauseOr(
-                        type_="or",
-                        conditions=[
-                            SQLWhereClauseOperator(
-                                type_="operator",
-                                operator="like",
-                                column=column,
-                                value=pattern,
-                            )
-                            for pattern in patterns
-                        ],
+                target_constraints.extend(
+                    SQLWhereClauseOperator(
+                        type_="operator",
+                        operator="like",
+                        column=column,
+                        value=pattern,
                     )
+                    for pattern in patterns
                 )
 
             for column, in_list in target.in_.items():
                 target_constraints.append(
                     SQLWhereClauseIn(
                         type_="in",
                         columns=[column],
```

### Comparing `subsetter-0.3.0/subsetter/sampler.py` & `subsetter-0.3.1/subsetter/sampler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import abc
 import functools
 import json
 import logging
 import os
 import re
-from typing import Any, Dict, List, Literal, Optional, Set, Tuple, Union
+from typing import Any, Dict, Iterable, List, Literal, Optional, Set, Tuple, Union
 
 import sqlalchemy as sa
 from pydantic import BaseModel, Field
 from sqlalchemy.ext.compiler import compiles
 from sqlalchemy.sql.expression import ClauseElement, Executable
 from typing_extensions import Annotated
 
@@ -56,15 +56,15 @@
             name,
             sa.MetaData(),
             *(sa.Column(col.name, col.type) for col in self.select.selected_columns),
             schema=self.schema,
         )
         return f"CREATE TEMPORARY TABLE {schema_enc}.{name_enc} AS {select_stmt}"
 
-    def _temporary_table_compile_postgres(self, compiler, **_) -> str:
+    def _temporary_table_compile_no_schema(self, compiler, **_) -> str:
         """
         Postgres creates temporary tables in a special schema. We make the table
         name incorporate the schema name to compensate and avoid collisions.
         """
         name = self.schema + self.TEMP_ID + f"{self.index}_" + self.name
         name_enc = compiler.dialect.identifier_preparer.quote(name)
         select_stmt = compiler.process(self.select)
@@ -72,15 +72,17 @@
             name,
             sa.MetaData(),
             *(sa.Column(col.name, col.type) for col in self.select.selected_columns),
         )
         return f"CREATE TEMPORARY TABLE {name_enc} AS {select_stmt}"
 
 
-compiles(TemporaryTable, "postgresql")(TemporaryTable._temporary_table_compile_postgres)
+compiles(TemporaryTable, "postgresql", "sqlite")(
+    TemporaryTable._temporary_table_compile_no_schema
+)
 compiles(TemporaryTable)(TemporaryTable._temporary_table_compile_generic)
 
 
 def _multiply_column(
     value: Optional[int], multiplier: int, iteration: int
 ) -> Optional[int]:
     if value is None:
@@ -137,14 +139,17 @@
         column_multipliers: Optional[Set[str]] = None,
     ) -> None:
         pass
 
     def truncate(self) -> None:
         """Delete any existing data that could interfere with output destination"""
 
+    def create(self, source_meta: DatabaseMetadata) -> None:
+        """Create any missing tables in destination from the source schema"""
+
     @abc.abstractmethod
     def insert_order(self) -> List[str]:
         """Return the order to insert data that respects foreign key relationships"""
 
     @staticmethod
     def from_config(config: Any, tables: List[str]) -> "SamplerOutput":
         if isinstance(config, DirectoryOutputConfig):
@@ -211,14 +216,100 @@
 
         self.meta, self.additional_tables = DatabaseMetadata.from_engine(
             self.engine,
             list(self.table_remap),
             close_backward=True,
         )
 
+    def create(self, source_meta: DatabaseMetadata) -> None:
+        """Create any missing tables in destination from the source schema"""
+        metadata_obj = sa.MetaData()
+
+        table_obj_map = {}
+        tables_created = set()
+        for remapped_table, table in self.table_remap.items():
+            remap_schema, remap_table = parse_table_name(remapped_table)
+
+            if (remap_schema, remap_table) in self.meta.tables:
+                table_obj_map[table] = self.meta.tables[
+                    (remap_schema, remap_table)
+                ].table_obj
+                continue
+
+            table_obj = source_meta.tables[parse_table_name(table)].table_obj
+            table_obj_map[table] = sa.Table(
+                remap_table,
+                metadata_obj,
+                *(
+                    sa.Column(
+                        col.name,
+                        col.type,
+                        nullable=col.nullable,
+                        primary_key=col.primary_key,
+                    )
+                    for col in table_obj.columns
+                ),
+                schema=remap_schema,
+            )
+            tables_created.add(table_obj_map[table])
+
+        def _remap_cols(cols: Iterable[sa.Column]) -> List[sa.Column]:
+            return [
+                table_obj_map[f"{col.table.schema}.{col.table.name}"].columns[col.name]
+                for col in cols
+            ]
+
+        # Copy table constraints including foreign key constraints.
+        for table, remapped_table_obj in table_obj_map.items():
+            if remapped_table_obj not in tables_created:
+                continue
+
+            table_obj = source_meta.tables[parse_table_name(table)].table_obj
+            for constraint in table_obj.constraints:
+                if isinstance(constraint, sa.UniqueConstraint):
+                    remapped_table_obj.append_constraint(
+                        sa.UniqueConstraint(*_remap_cols(constraint.columns))
+                    )
+                if isinstance(constraint, sa.CheckConstraint):
+                    remapped_table_obj.append_constraint(
+                        sa.CheckConstraint(constraint.sqltext)
+                    )
+                if isinstance(constraint, sa.ForeignKeyConstraint):
+                    fk_cols = _remap_cols(elem.column for elem in constraint.elements)
+                    remapped_table_obj.append_constraint(
+                        sa.ForeignKeyConstraint(
+                            _remap_cols(constraint.columns),
+                            fk_cols,
+                            name=constraint.name,
+                            use_alter=True,
+                        )
+                    )
+
+            for index_idx, index in enumerate(table_obj.indexes):
+                sa.Index(
+                    f"idx_subsetter_{remapped_table_obj.name}_{index_idx}",
+                    *(
+                        (
+                            remapped_table_obj.columns[col.name]
+                            if isinstance(col, sa.Column)
+                            else col
+                        )
+                        for col in index.columns
+                    ),
+                    unique=index.unique,
+                    dialect_options=index.dialect_options,
+                    **index.dialect_kwargs,
+                )
+
+        if tables_created:
+            LOGGER.info("Creating %d tables in destination", len(tables_created))
+            metadata_obj.create_all(bind=self.engine)
+            for remapped_table_obj in tables_created:
+                self.meta.track_new_table(remapped_table_obj)
+
     def truncate(self) -> None:
         for schema, table_name in self.additional_tables:
             LOGGER.info(
                 "Found additional table %s.%s to truncate",
                 schema,
                 table_name,
             )
@@ -258,16 +349,24 @@
         filter_view: Optional[FilterView] = None,
         multiplier: int = 1,
         column_multipliers: Optional[Set[str]] = None,
     ) -> None:
         schema, table_name = self._remap_table(schema, table_name)
         table = self.meta.tables[(schema, table_name)]
 
-        # Automatically omit any included computed columns
         columns_out = filter_view.columns_out if filter_view else columns
+        missing_columns = {
+            col for col in columns_out if col not in table.table_obj.columns
+        }
+        if missing_columns:
+            raise ValueError(
+                f"Destination table {schema}.{table_name} is missing expected columns {missing_columns}"
+            )
+
+        # Automatically omit any included computed columns
         computed_columns = [
             col for col in columns_out if table.table_obj.columns[col].computed
         ]
         if computed_columns:
             omit_filter = FilterOmit(columns_out, computed_columns)
             columns_out = omit_filter.columns_out
             if filter_view:
@@ -313,25 +412,33 @@
 class Sampler:
     def __init__(self, config: SamplerConfig) -> None:
         self.config = config
         self.source_engine = self.config.source.database_engine(
             env_prefix="SUBSET_SOURCE_"
         )
 
-    def sample(self, plan: SubsetPlan, *, truncate: bool = False) -> None:
+    def sample(
+        self,
+        plan: SubsetPlan,
+        *,
+        truncate: bool = False,
+        create: bool = False,
+    ) -> None:
         meta, _ = DatabaseMetadata.from_engine(self.source_engine, list(plan.queries))
         if self.config.multiplicity.infer_foreign_keys:
             meta.infer_missing_foreign_keys()
         self._validate_filters(meta)
 
         table_column_multipliers = self._get_multiplied_columns(
             meta, list(plan.queries)
         )
 
         output = SamplerOutput.from_config(self.config.output, list(plan.queries))
+        if create:
+            output.create(meta)
         insert_order = output.insert_order()
         if truncate:
             output.truncate()
 
         with self.source_engine.execution_options().connect() as conn:
             self._materialize_tables(meta, conn, plan)
             self._copy_results(
```

### Comparing `subsetter-0.3.0/subsetter/solver.py` & `subsetter-0.3.1/subsetter/solver.py`

 * *Files identical despite different names*

### Comparing `subsetter-0.3.0/subsetter.egg-info/PKG-INFO` & `subsetter-0.3.1/subsetter.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subsetter
-Version: 0.3.0
+Version: 0.3.1
 Summary: MySQL database subsetting CLI tool
 Home-page: http://github.com/msg555/subsetter/
 Author: Mark Gordon
 Author-email: msg555@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -18,18 +18,22 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sqlalchemy[mypy]~=2.0
 Requires-Dist: pydantic~=2.6
 Requires-Dist: pyyaml~=6.0
 Requires-Dist: faker~=19.3
 Requires-Dist: typing-extensions
-Provides-Extra: mysql
-Requires-Dist: pymysql~=1.0; extra == "mysql"
-Provides-Extra: postgres
-Requires-Dist: psycopg2-binary~=2.0; extra == "postgres"
+Provides-Extra: all
+Requires-Dist: sqlalchemy[postgresql_psycopg2binary,pymysql]; extra == "all"
+Provides-Extra: pymysql
+Requires-Dist: sqlalchemy[pymysql]; extra == "pymysql"
+Provides-Extra: postgresql
+Requires-Dist: sqlalchemy[postgresql]; extra == "postgresql"
+Provides-Extra: postgresql-psycopg2binary
+Requires-Dist: sqlalchemy[postgresql_psycopg2binary]; extra == "postgresql-psycopg2binary"
 
 # Subsetter
 
 Subsetter is a Python utility that can be used for subsetting portions of
 relational databases. _Subsetting_ is the action extracting a smaller set of rows
 from your database that still maintain expected foreign-key relationships
 between your data. This can be useful for testing against a small but
@@ -115,7 +119,44 @@
 create a semantically consistent large dataset from your existing data. The
 sampler has support for this by setting the multiplicity factor.
 
 Multiplicity works by creating multiple copies of your sampled dataset in your
 output database. To ensure these datasets do not collide it remaps all foreign
 keys into a new key-space. Note that this process assumes your foreign keys are
 opaque integers identifiers.
+
+# FAQ
+
+## How do multiple targets work
+
+When using multiple targets each target table will be sampled entirely
+independently unless another target table directly or indirectly depends on some
+rows from it through a series of foreign keys. In the later case the subsetter
+will sample a union of the rows from the independently sampling of the table and
+those rows that other targets depend on.
+
+## How does the subsetter use foreign keys?
+
+The subsetter uses the foreign keys present in the database schema to understand
+relationships between data and generate a sampling plan. Foreign key
+relationships can be followed in both directions if need be. For example,
+suppose there was a `users` and an `orders` table where `orders` had a foreign key
+to the `users` table.
+
+If `users` was sampled first the subsetter would sample `orders` from `users` by
+sampling all rows from `orders` such that their corresponding user row existed.
+This represents the _maximal_ set of rows that can be included without violating
+foreign key constraints.
+
+Otherwise if `orders` was sampled first the subsetter would sample `users` from
+`orders` by sampling all rows from `users` such that they had at least one
+`order`. This represents the _minimal_ set of rows that can be included without
+violating foreign key constraints.
+
+In general the subsetter will always sample tables in an order such that all
+foreign key relationships to previously sampled tables are going in the same
+direction. If they are followed in the forwards direction (as in our first case)
+the subsetter will select the _intersection_ of all rows that obey each foreign
+key relationship. Otherwise if they are followed in the backwards direction (as
+in our second case) the subsetter will select the _union_ of all rows that obey
+each foreign key relationship. This strategy ensures no foreign key
+relationships are violated in the sampled data.
```

### Comparing `subsetter-0.3.0/subsetter.egg-info/SOURCES.txt` & `subsetter-0.3.1/subsetter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `subsetter-0.3.0/tests/test_filters.py` & `subsetter-0.3.1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `subsetter-0.3.0/tests/test_live.py` & `subsetter-0.3.1/tests/test_live.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import tempfile
 
 import pytest
 
 from subsetter.common import DatabaseConfig
 
 from .dataset_manager import do_dataset_test
 
@@ -27,14 +28,32 @@
         host=postgresql.host,
         port=postgresql.port,
         username=postgresql.user,
         password="",
     )
 
 
+@pytest.fixture
+def sqlite_init_db():
+    with tempfile.NamedTemporaryFile(suffix=".db") as tf1:
+        with tempfile.NamedTemporaryFile(suffix=".db") as tf2:
+            yield tf1.name, tf2.name
+
+
+def db_config_sqlite(request):
+    db1, db2 = request.getfixturevalue("sqlite_init_db")
+    return DatabaseConfig(
+        dialect="sqlite",
+        sqlite_databases={
+            "test": db1,
+            "test_out": db2,
+        },
+    )
+
+
 DATABASE_CONFIGURATIONS = [
     pytest.param(
         db_config_mysql,
         marks=[
             pytest.mark.usefixtures("mysql_proc"),
             pytest.mark.mysql_live,
         ],
@@ -44,14 +63,22 @@
         db_config_postgres,
         marks=[
             pytest.mark.usefixtures("postgresql_proc"),
             pytest.mark.postgres_live,
         ],
         id="postgres",
     ),
+    pytest.param(
+        db_config_sqlite,
+        marks=[
+            pytest.mark.usefixtures("sqlite_init_db"),
+            pytest.mark.sqlite_live,
+        ],
+        id="sqlite",
+    ),
 ]
 
 
 @pytest.fixture(name="db_config")
 def fixture_db_config(request):
     return request.param(request)
```

### Comparing `subsetter-0.3.0/tests/test_solver.py` & `subsetter-0.3.1/tests/test_solver.py`

 * *Files identical despite different names*


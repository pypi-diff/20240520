# Comparing `tmp/pypomes_db-0.8.5.tar.gz` & `tmp/pypomes_db-0.8.6.tar.gz`

## Comparing `pypomes_db-0.8.5.tar` & `pypomes_db-0.8.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    32487 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    18598 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    16025 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    15140 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    31452 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    18598 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    15146 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    13914 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/PKG-INFO
```

### Comparing `pypomes_db-0.8.5/src/pypomes_db/__init__.py` & `pypomes_db-0.8.6/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.5/src/pypomes_db/db_common.py` & `pypomes_db-0.8.6/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.5/src/pypomes_db/db_pomes.py` & `pypomes_db-0.8.6/src/pypomes_db/db_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,17 +108,16 @@
 
     # determine the database engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     proceed: bool = True
     if curr_engine == "oracle":
         from . import oracle_pomes
-        # noinspection PyProtectedMember
-        proceed = oracle_pomes._initialize(errors=op_errors,
-                                           logger=logger)
+        proceed = oracle_pomes.initialize(errors=op_errors,
+                                          logger=logger)
     if proceed:
         conn: Any = db_connect(errors=op_errors,
                                engine=curr_engine,
                                logger=logger)
         if conn:
             conn.close()
             result = True
@@ -151,27 +150,24 @@
     # determine the database engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        # noinspection PyProtectedMember
-        result = oracle_pomes._connect(errors=op_errors,
-                                       logger=logger)
+        result = oracle_pomes.connect(errors=op_errors,
+                                      logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        # noinspection PyProtectedMember
-        result = postgres_pomes._connect(errors=op_errors,
-                                         logger=logger)
+        result = postgres_pomes.connect(errors=op_errors,
+                                        logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        # noinspection PyProtectedMember
-        result = sqlserver_pomes._connect(errors=op_errors,
-                                          logger=logger)
+        result = sqlserver_pomes.connect(errors=op_errors,
+                                         logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -299,42 +295,39 @@
     # determine the database engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        # noinspection PyProtectedMember
-        result = oracle_pomes._select_all(errors=op_errors,
-                                          sel_stmt=sel_stmt,
-                                          where_vals=where_vals,
-                                          require_min=require_min,
-                                          require_max=require_max,
-                                          conn=conn,
-                                          logger=logger)
+        result = oracle_pomes.select_all(errors=op_errors,
+                                         sel_stmt=sel_stmt,
+                                         where_vals=where_vals,
+                                         require_min=require_min,
+                                         require_max=require_max,
+                                         conn=conn,
+                                         logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        # noinspection PyProtectedMember
-        result = postgres_pomes._select_all(errors=op_errors,
+        result = postgres_pomes.select_all(errors=op_errors,
+                                           sel_stmt=sel_stmt,
+                                           where_vals=where_vals,
+                                           require_min=require_min,
+                                           require_max=require_max,
+                                           conn=conn,
+                                           logger=logger)
+    elif curr_engine == "sqlserver":
+        from . import sqlserver_pomes
+        result = sqlserver_pomes.select_all(errors=op_errors,
                                             sel_stmt=sel_stmt,
                                             where_vals=where_vals,
                                             require_min=require_min,
                                             require_max=require_max,
                                             conn=conn,
                                             logger=logger)
-    elif curr_engine == "sqlserver":
-        from . import sqlserver_pomes
-        # noinspection PyProtectedMember
-        result = sqlserver_pomes._select_all(errors=op_errors,
-                                             sel_stmt=sel_stmt,
-                                             where_vals=where_vals,
-                                             require_min=require_min,
-                                             require_max=require_max,
-                                             conn=conn,
-                                             logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -483,36 +476,33 @@
     # determine the database engine
     curr_engine: str = _assert_engine(op_errors, engine)
     
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        # noinspection PyProtectedMember
-        result = oracle_pomes._bulk_insert(errors=op_errors,
-                                           insert_stmt=insert_stmt,
-                                           insert_vals=insert_vals,
-                                           conn=conn,
-                                           logger=logger)
+        result = oracle_pomes.bulk_insert(errors=op_errors,
+                                          insert_stmt=insert_stmt,
+                                          insert_vals=insert_vals,
+                                          conn=conn,
+                                          logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        # noinspection PyProtectedMember
-        result = postgres_pomes._bulk_insert(errors=op_errors,
+        result = postgres_pomes.bulk_insert(errors=op_errors,
+                                            insert_stmt=insert_stmt,
+                                            insert_vals=insert_vals,
+                                            conn=conn,
+                                            logger=logger)
+    elif curr_engine == "sqlserver":
+        from . import sqlserver_pomes
+        result = sqlserver_pomes.bulk_insert(errors=op_errors,
                                              insert_stmt=insert_stmt,
                                              insert_vals=insert_vals,
                                              conn=conn,
                                              logger=logger)
-    elif curr_engine == "sqlserver":
-        from . import sqlserver_pomes
-        # noinspection PyProtectedMember
-        result = sqlserver_pomes._bulk_insert(errors=op_errors,
-                                              insert_stmt=insert_stmt,
-                                              insert_vals=insert_vals,
-                                              conn=conn,
-                                              logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -547,48 +537,45 @@
     # determine the database engine
     curr_engine: str = _assert_engine(op_errors, engine)
     
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        # noinspection PyProtectedMember
-        oracle_pomes._update_lob(errors=op_errors,
-                                 lob_table=lob_table,
-                                 lob_column=lob_column,
-                                 pk_columns=pk_columns,
-                                 pk_vals=pk_vals,
-                                 lob_file=lob_file,
-                                 chunk_size=chunk_size,
-                                 conn=conn,
-                                 logger=logger)
+        oracle_pomes.update_lob(errors=op_errors,
+                                lob_table=lob_table,
+                                lob_column=lob_column,
+                                pk_columns=pk_columns,
+                                pk_vals=pk_vals,
+                                lob_file=lob_file,
+                                chunk_size=chunk_size,
+                                conn=conn,
+                                logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        # noinspection PyProtectedMember
-        postgres_pomes._update_lob(errors=op_errors,
+        postgres_pomes.update_lob(errors=op_errors,
+                                  lob_table=lob_table,
+                                  lob_column=lob_column,
+                                  pk_columns=pk_columns,
+                                  pk_vals=pk_vals,
+                                  lob_file=lob_file,
+                                  chunk_size=chunk_size,
+                                  conn=conn,
+                                  logger=logger)
+    elif curr_engine == "sqlserver":
+        from . import sqlserver_pomes
+        sqlserver_pomes.update_lob(errors=op_errors,
                                    lob_table=lob_table,
                                    lob_column=lob_column,
                                    pk_columns=pk_columns,
                                    pk_vals=pk_vals,
                                    lob_file=lob_file,
                                    chunk_size=chunk_size,
                                    conn=conn,
                                    logger=logger)
-    elif curr_engine == "sqlserver":
-        from . import sqlserver_pomes
-        # noinspection PyProtectedMember
-        sqlserver_pomes._update_lob(errors=op_errors,
-                                    lob_table=lob_table,
-                                    lob_column=lob_column,
-                                    pk_columns=pk_columns,
-                                    pk_vals=pk_vals,
-                                    lob_file=lob_file,
-                                    chunk_size=chunk_size,
-                                    conn=conn,
-                                    logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
 
 def db_execute(errors: list[str] | None,
                exc_stmt: str,
@@ -624,36 +611,33 @@
     # determine the database engine
     curr_engine: str = _assert_engine(op_errors, engine)
     
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        # noinspection PyProtectedMember
-        result = oracle_pomes._execute(errors=op_errors,
-                                       exc_stmt=exc_stmt,
-                                       bind_vals=bind_vals,
-                                       conn=conn,
-                                       logger=logger)
+        result = oracle_pomes.execute(errors=op_errors,
+                                      exc_stmt=exc_stmt,
+                                      bind_vals=bind_vals,
+                                      conn=conn,
+                                      logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        # noinspection PyProtectedMember
         result = postgres_pomes.db_execute(errors=op_errors,
                                            exc_stmt=exc_stmt,
                                            bind_vals=bind_vals,
                                            conn=conn,
                                            logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        # noinspection PyProtectedMember
-        result = sqlserver_pomes._execute(errors=op_errors,
-                                          exc_stmt=exc_stmt,
-                                          bind_vals=bind_vals,
-                                          conn=conn,
-                                          logger=logger)
+        result = sqlserver_pomes.execute(errors=op_errors,
+                                         exc_stmt=exc_stmt,
+                                         bind_vals=bind_vals,
+                                         conn=conn,
+                                         logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -685,36 +669,33 @@
     # determine the database engine
     curr_engine: str = _assert_engine(op_errors, engine)
     
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        # noinspection PyProtectedMember
-        result = oracle_pomes._call_function(errors=op_errors,
-                                             func_name=func_name,
-                                             func_vals=func_vals,
-                                             conn=conn,
-                                             logger=logger)
+        result = oracle_pomes.call_function(errors=op_errors,
+                                            func_name=func_name,
+                                            func_vals=func_vals,
+                                            conn=conn,
+                                            logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        # noinspection PyProtectedMember
-        result = postgres_pomes._call_procedure(errors=op_errors,
+        result = postgres_pomes.call_procedure(errors=op_errors,
+                                               proc_name=func_name,
+                                               proc_vals=func_vals,
+                                               conn=conn,
+                                               logger=logger)
+    elif curr_engine == "sqlserver":
+        from . import sqlserver_pomes
+        result = sqlserver_pomes.call_procedure(errors=op_errors,
                                                 proc_name=func_name,
                                                 proc_vals=func_vals,
                                                 conn=conn,
                                                 logger=logger)
-    elif curr_engine == "sqlserver":
-        from . import sqlserver_pomes
-        # noinspection PyProtectedMember
-        result = sqlserver_pomes._call_procedure(errors=op_errors,
-                                                 proc_name=func_name,
-                                                 proc_vals=func_vals,
-                                                 conn=conn,
-                                                 logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -746,34 +727,31 @@
     # determine the database engine
     curr_engine: str = _assert_engine(op_errors, engine)
     
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        # noinspection PyProtectedMember
-        result = oracle_pomes._call_procedure(errors=op_errors,
-                                              proc_name=proc_name,
-                                              proc_vals=proc_vals,
-                                              conn=conn,
-                                              logger=logger)
+        result = oracle_pomes.call_procedure(errors=op_errors,
+                                             proc_name=proc_name,
+                                             proc_vals=proc_vals,
+                                             conn=conn,
+                                             logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        # noinspection PyProtectedMember
-        result = postgres_pomes._call_procedure(errors=op_errors,
+        result = postgres_pomes.call_procedure(errors=op_errors,
+                                               proc_name=proc_name,
+                                               proc_vals=proc_vals,
+                                               conn=conn,
+                                               logger=logger)
+    elif curr_engine == "sqlserver":
+        from . import sqlserver_pomes
+        result = sqlserver_pomes.call_procedure(errors=op_errors,
                                                 proc_name=proc_name,
                                                 proc_vals=proc_vals,
                                                 conn=conn,
                                                 logger=logger)
-    elif curr_engine == "sqlserver":
-        from . import sqlserver_pomes
-        # noinspection PyProtectedMember
-        result = sqlserver_pomes._call_procedure(errors=op_errors,
-                                                 proc_name=proc_name,
-                                                 proc_vals=proc_vals,
-                                                 conn=conn,
-                                                 logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
```

### Comparing `pypomes_db-0.8.5/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.8.6/src/pypomes_db/migration_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.5/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.8.6/src/pypomes_db/oracle_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # noinspection DuplicatedCode
+import oracledb
 from logging import Logger
-from oracledb import Connection, connect, init_oracle_client
+from oracledb import Connection, init_oracle_client
 from pathlib import Path
 
 from .db_common import (
     _DB_CONN_DATA,
     _db_assert_query_quota, _db_get_params, _db_log, _db_except_msg
 )
 
 
-def _connect(errors: list[str],
-             logger: Logger) -> Connection:
+def connect(errors: list[str],
+            logger: Logger) -> Connection:
     """
     Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
     """
@@ -23,19 +24,19 @@
 
     # retrieve the connection parameters
     name, user, pwd, host, port = _db_get_params("oracle")
 
     # obtain a connection to the database
     err_msg: str | None = None
     try:
-        result = connect(service_name=name,
-                         host=host,
-                         port=port,
-                         user=user,
-                         password=pwd)
+        result = oracledb.connect(service_name=name,
+                                  host=host,
+                                  port=port,
+                                  user=user,
+                                  password=pwd)
         # make sure the connection is not in autocommit mode
         result.autocommit = False
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
 
     # log the results
@@ -44,21 +45,21 @@
             err_msg=err_msg,
             errors=errors,
             stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
-def _select_all(errors: list[str],
-                sel_stmt: str,
-                where_vals: tuple,
-                require_min: int,
-                require_max: int,
-                conn: Connection,
-                logger: Logger) -> list[tuple]:
+def select_all(errors: list[str],
+               sel_stmt: str,
+               where_vals: tuple,
+               require_min: int,
+               require_max: int,
+               conn: Connection,
+               logger: Logger) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
     If the search is empty, an empty list is returned.
@@ -72,16 +73,16 @@
     :param logger: optional logger
     :return: tuple containing the search result, [] if the search was empty, or None if there was an error
     """
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
-    curr_conn: Connection = conn or _connect(errors=errors,
-                                             logger=logger)
+    curr_conn: Connection = conn or connect(errors=errors,
+                                            logger=logger)
 
     if isinstance(require_max, int) and require_max > 0:
         sel_stmt: str = f"{sel_stmt} FETCH NEXT {require_max} ROWS ONLY"
 
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
@@ -123,19 +124,19 @@
                 errors=errors,
                 stmt=sel_stmt,
                 bind_vals=where_vals)
 
     return result
 
 
-def _bulk_insert(errors: list[str],
-                 insert_stmt: str,
-                 insert_vals: list[tuple],
-                 conn: Connection,
-                 logger: Logger) -> int:
+def bulk_insert(errors: list[str],
+                insert_stmt: str,
+                insert_vals: list[tuple],
+                conn: Connection,
+                logger: Logger) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     The binding must be done by position. Thus, the *VALUES* clause in *insert_stmt*
     must contain as many ':n' placeholders as there are elements in the tuples found in the
     list provided in *insert_vals*, where 'n' is the 1-based position of the data in the tuple.
 
@@ -146,16 +147,16 @@
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
-    curr_conn: Connection = conn or _connect(errors=errors,
-                                             logger=logger)
+    curr_conn: Connection = conn or connect(errors=errors,
+                                            logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
             cursor.executemany(statement=insert_stmt,
                                parameters=insert_vals)
@@ -179,39 +180,39 @@
                 errors=errors,
                 stmt=insert_stmt,
                 bind_vals=insert_vals[0])
 
     return result
 
 
-def _update_lob(errors: list[str],
-                lob_table: str,
-                lob_column: str,
-                pk_columns: list[str],
-                pk_vals: tuple,
-                lob_file: str | Path,
-                chunk_size: int,
-                conn: Connection,
-                logger: Logger) -> None:
+def update_lob(errors: list[str],
+               lob_table: str,
+               lob_column: str,
+               pk_columns: list[str],
+               pk_vals: tuple,
+               lob_file: str | Path,
+               chunk_size: int,
+               conn: Connection,
+               logger: Logger) -> None:
     """
     Update a large binary objects (LOB) in the given table and column.
 
     :param errors: incidental error messages
     :param lob_table: the table to be update with the new LOB
     :param lob_column: the column to be updated with the new LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param pk_vals: values with which to locate the tuple to be updated
     :param lob_file: file holding the LOB (a file object or a valid path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     """
     # make sure to have a connection
-    curr_conn: Connection = conn or _connect(errors=errors,
-                                             logger=logger)
+    curr_conn: Connection = conn or connect(errors=errors,
+                                            logger=logger)
 
     # make sure to have a data file
     data_file: Path = Path(lob_file) if isinstance(lob_file, str) else lob_file
 
     # normalize the chunk size
     if not chunk_size:
         chunk_size = -1
@@ -256,19 +257,19 @@
                 err_msg=err_msg,
                 engine="oracle",
                 errors=errors,
                 stmt=update_stmt,
                 bind_vals=pk_vals)
 
 
-def _execute(errors: list[str],
-             exc_stmt: str,
-             bind_vals: tuple,
-             conn: Connection,
-             logger: Logger) -> int:
+def execute(errors: list[str],
+            exc_stmt: str,
+            bind_vals: tuple,
+            conn: Connection,
+            logger: Logger) -> int:
     """
     Execute the command *exc_stmt* on the database.
 
     This command might be a DML ccommand modifying the database, such as
     inserting, updating or deleting tuples, or it might be a DDL statement,
     or it might even be an environment-related command.
     The optional bind values for this operation are in *bind_vals*.
@@ -283,16 +284,16 @@
     :param logger: optional logger
     :return: the return value from the command execution
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
-    curr_conn: Connection = conn or _connect(errors=errors,
-                                             logger=logger)
+    curr_conn: Connection = conn or connect(errors=errors,
+                                            logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
             cursor.execute(statement=exc_stmt,
                            parameters=bind_vals)
@@ -319,19 +320,19 @@
                 bind_vals=bind_vals)
 
     return result
 
 
 # TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
 # noinspection PyUnusedLocal
-def _call_function(errors: list[str],
-                   func_name: str,
-                   func_vals: tuple,
-                   conn: Connection,
-                   logger: Logger) -> list[tuple]:
+def call_function(errors: list[str],
+                  func_name: str,
+                  func_vals: tuple,
+                  conn: Connection,
+                  logger: Logger) -> list[tuple]:
     """
     Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
 
     :param errors: incidental error messages
     :param func_name: name of the stored function
     :param func_vals: parameters for the stored function
     :param conn: optional connection to use (obtains a new one, if not provided)
@@ -341,35 +342,35 @@
     # initialize the return variable
     result: list[tuple] = []
 
     return result
 
 
 # TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
-def _call_procedure(errors: list[str],
-                    proc_name: str,
-                    proc_vals: tuple,
-                    conn: Connection,
-                    logger: Logger) -> list[tuple]:
+def call_procedure(errors: list[str],
+                   proc_name: str,
+                   proc_vals: tuple,
+                   conn: Connection,
+                   logger: Logger) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
     :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
-    curr_conn: Connection = conn or _connect(errors=errors,
-                                             logger=logger)
+    curr_conn: Connection = conn or connect(errors=errors,
+                                            logger=logger)
 
     # execute the stored procedure
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
             cursor.callproc(name=proc_name,
@@ -398,16 +399,16 @@
                 stmt=proc_name,
                 bind_vals=proc_vals)
 
     return result
 
 __is_initialized: str | None = None
 
-def _initialize(errors: list[str],
-                logger: Logger) -> bool:
+def initialize(errors: list[str],
+               logger: Logger) -> bool:
     """
     Prepare the oracle engine to access the database throught the installed client software.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: False if an error happened, True otherwise
     """
```

### Comparing `pypomes_db-0.8.5/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.8.6/src/pypomes_db/postgres_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # noinspection DuplicatedCode
+import psycopg2
 from logging import WARNING, Logger
 from pathlib import Path
-from psycopg2 import Binary, connect
+from psycopg2 import Binary
 from psycopg2.extras import execute_values
 # noinspection PyProtectedMember
 from psycopg2._psycopg import connection
 from typing import Any
 
 from .db_common import (
     _db_assert_query_quota, _db_get_params,
     _db_log, _db_except_msg, _db_remove_nulls
 )
 
 
-def _connect(errors: list[str],
-             logger: Logger = None) -> connection:
+def connect(errors: list[str],
+            logger: Logger = None) -> connection:
     """
     Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
     """
@@ -27,19 +28,19 @@
 
     # retrieve the connection parameters
     name, user, pwd, host, port = _db_get_params("postgres")
 
     # obtain a connection to the database
     err_msg: str | None = None
     try:
-        result = connect(host=host,
-                         port=port,
-                         database=name,
-                         user=user,
-                         password=pwd)
+        result = psycopg2.connect(host=host,
+                                  port=port,
+                                  database=name,
+                                  user=user,
+                                  password=pwd)
         # make sure the connection is not in autocommit mode
         result.autocommit = False
     except Exception as e:
         err_msg = _db_except_msg(e, "postgres")
 
     # log the results
     _db_log(logger=logger,
@@ -47,21 +48,21 @@
             err_msg=err_msg,
             errors=errors,
             stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
-def _select_all(errors: list[str],
-                sel_stmt: str,
-                where_vals: tuple,
-                require_min: int,
-                require_max: int,
-                conn: connection,
-                logger: Logger) -> list[tuple]:
+def select_all(errors: list[str],
+               sel_stmt: str,
+               where_vals: tuple,
+               require_min: int,
+               require_max: int,
+               conn: connection,
+               logger: Logger) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
     If the search is empty, an empty list is returned.
@@ -75,16 +76,16 @@
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
-    curr_conn: connection = conn or _connect(errors=errors,
-                                             logger=logger)
+    curr_conn: connection = conn or connect(errors=errors,
+                                            logger=logger)
 
     if isinstance(require_max, int) and require_max >= 0:
         sel_stmt += f" LIMIT {require_max}"
 
     err_msg: str | None = None
     try:
         # obtain a cursor and execute the operation
@@ -125,19 +126,19 @@
                 errors=errors,
                 stmt=sel_stmt,
                 bind_vals=where_vals)
 
     return result
 
 
-def _bulk_insert(errors: list[str],
-                 insert_stmt: str,
-                 insert_vals: list[tuple],
-                 conn: connection,
-                 logger: Logger) -> int:
+def bulk_insert(errors: list[str],
+                insert_stmt: str,
+                insert_vals: list[tuple],
+                conn: connection,
+                logger: Logger) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     The *VALUES* clause in *insert_stmt* must be simply *VALUES %s*.
     Note that, after the execution of *execute_values*, the *cursor.rowcount* property
     will not contain a total result, and thus the value 1 (one) is returned on success.
 
@@ -148,16 +149,16 @@
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
-    curr_conn: connection = conn or _connect(errors=errors,
-                                             logger=logger)
+    curr_conn: connection = conn or connect(errors=errors,
+                                            logger=logger)
 
     # execute the bulk insert
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
             execute_values(cur=cursor,
@@ -183,19 +184,19 @@
                 if cleaned_row:
                     # yes, register it
                     cleaned_rows.append((inx, cleaned_row))
             # replace the cleaned rows
             for cleaned_row in cleaned_rows:
                 insert_vals[cleaned_row[0]] = tuple(cleaned_row[1])
             # bulk insert the cleaned data
-            _bulk_insert(errors=errors,
-                         insert_stmt=insert_stmt,
-                         insert_vals=insert_vals,
-                         conn=conn,
-                         logger=logger)
+            bulk_insert(errors=errors,
+                        insert_stmt=insert_stmt,
+                        insert_vals=insert_vals,
+                        conn=conn,
+                        logger=logger)
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
@@ -209,39 +210,39 @@
                 err_msg=err_msg,
                 errors=errors,
                 stmt=insert_stmt)
 
     return result
 
 
-def _update_lob(errors: list[str],
-                lob_table: str,
-                lob_column: str,
-                pk_columns: list[str],
-                pk_vals: tuple,
-                lob_file: str | Path,
-                chunk_size: int,
-                conn: connection,
-                logger: Logger) -> None:
+def update_lob(errors: list[str],
+               lob_table: str,
+               lob_column: str,
+               pk_columns: list[str],
+               pk_vals: tuple,
+               lob_file: str | Path,
+               chunk_size: int,
+               conn: connection,
+               logger: Logger) -> None:
     """
     Update a large binary objects (LOB) in the given table and column.
 
     :param errors: incidental error messages
     :param lob_table: the table to be update with the new LOB
     :param lob_column: the column to be updated with the new LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param pk_vals: values with which to locate the tuple to be updated
     :param lob_file: file holding the LOB (a file object or a valid path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     """
     # make sure to have a connection
-    curr_conn: connection = conn or _connect(errors=errors,
-                                             logger=logger)
+    curr_conn: connection = conn or connect(errors=errors,
+                                            logger=logger)
 
     # make sure to have a data file
     data_file: Path = Path(lob_file) if isinstance(lob_file, str) else lob_file
 
     # normalize the chunk size
     if not chunk_size:
         chunk_size = -1
@@ -310,16 +311,16 @@
     :param logger: optional logger
     :return: the return value from the command execution
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
-    curr_conn: connection = conn or _connect(errors=errors,
-                                             logger=logger)
+    curr_conn: connection = conn or connect(errors=errors,
+                                            logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
             cursor.execute(query=f"{exc_stmt};",
                            vars=bind_vals)
@@ -345,46 +346,46 @@
                 stmt=exc_stmt,
                 bind_vals=bind_vals)
 
     return result
 
 
 
-def _call_procedure(errors: list[str],
-                    proc_name: str,
-                    proc_vals: tuple,
-                    conn: connection,
-                    logger: Logger) -> list[tuple]:
+def call_procedure(errors: list[str],
+                   proc_name: str,
+                   proc_vals: tuple,
+                   conn: connection,
+                   logger: Logger) -> list[tuple]:
     """
     Execute the stored procedure *proc_name*, with the arguments given in *proc_vals*.
 
     :param errors:  incidental error messages
     :param proc_name: the name of the sotred procedure
     :param proc_vals: the arguments to be passed
     :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     result: list[tuple] = [()]
 
     # make sure to have a connection
-    curr_conn: connection = conn or _connect(errors=errors,
-                                             logger=logger)
+    curr_conn: connection = conn or connect(errors=errors,
+                                            logger=logger)
 
     # build the command
     proc_stmt: str = f"{proc_name}(" + "%s, " * (len(proc_vals) - 1) + "%s)"
 
     # execute the stored procedure
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
             cursor.execute(query=proc_stmt,
-                           argslist=proc_vals)
+                           vars=proc_vals)
             # retrieve the returned tuples
             result = list(cursor)
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
```

### Comparing `pypomes_db-0.8.5/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.8.6/src/pypomes_db/sqlserver_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # noinspection DuplicatedCode
+import pyodbc
 from logging import Logger
-from pyodbc import Binary, Connection, Row, connect
+from pyodbc import Binary, Connection, Row
 from pathlib import Path
 
 from .db_common import (
     _db_assert_query_quota, _db_get_params, _db_log, _db_except_msg
 )
 
 
-def _connect(errors: list[str],
-             logger: Logger = None) -> Connection:
+def connect(errors: list[str],
+            logger: Logger = None) -> Connection:
     """
     Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
     """
@@ -26,15 +27,15 @@
         f"DRIVER={{{driver}}};SERVER={host},{port};"
         f"DATABASE={name};UID={user};PWD={pwd};TrustServerCertificate=yes;"
     )
 
     # obtain a connection to the database
     err_msg: str | None = None
     try:
-        result = connect(connection_kwargs)
+        result = pyodbc.connect(connection_kwargs)
         # make sure the connection is not in autocommit mode
         result.autocommit = False
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
 
     # log the results
@@ -43,21 +44,21 @@
             err_msg=err_msg,
             errors=errors,
             stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
-def _select_all(errors: list[str],
-                sel_stmt: str,
-                where_vals: tuple,
-                require_min: int,
-                require_max: int,
-                conn: Connection,
-                logger: Logger) -> list[tuple]:
+def select_all(errors: list[str],
+               sel_stmt: str,
+               where_vals: tuple,
+               require_min: int,
+               require_max: int,
+               conn: Connection,
+               logger: Logger) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
     If the search is empty, an empty list is returned.
@@ -71,16 +72,16 @@
     :param logger: optional logger
     :return: tuple containing the search result, [] if the search was empty, or None if there was an error
     """
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
-    curr_conn: Connection = conn or _connect(errors=errors,
-                                             logger=logger)
+    curr_conn: Connection = conn or connect(errors=errors,
+                                            logger=logger)
 
     err_msg: str | None = None
     if isinstance(require_max, int) and require_max > 0:
         sel_stmt: str = sel_stmt.replace("SELECT", f"SELECT TOP {require_max}", 1)
 
     try:
         # obtain a cursor and execute the operation
@@ -120,19 +121,19 @@
                 errors=errors,
                 stmt=sel_stmt,
                 bind_vals=where_vals)
 
     return result
 
 
-def _bulk_insert(errors: list[str],
-                 insert_stmt: str,
-                 insert_vals: list[tuple],
-                 conn: Connection,
-                 logger: Logger) -> int:
+def bulk_insert(errors: list[str],
+                insert_stmt: str,
+                insert_vals: list[tuple],
+                conn: Connection,
+                logger: Logger) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     The *VALUES* clause in *insert_stmt* must contain as many '%s' placeholders
     as there are elements in the tuples found in the list provided in *insert_vals*.
 
     :param errors: incidental error messages
@@ -142,16 +143,16 @@
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
-    curr_conn: Connection = conn or _connect(errors=errors,
-                                             logger=logger)
+    curr_conn: Connection = conn or connect(errors=errors,
+                                            logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
             cursor.fast_executemany = True
             try:
@@ -179,39 +180,39 @@
                 errors=errors,
                 stmt=insert_stmt,
                 bind_vals=insert_vals[0])
 
     return result
 
 
-def _update_lob(errors: list[str],
-                lob_table: str,
-                lob_column: str,
-                pk_columns: list[str],
-                pk_vals: tuple,
-                lob_file: str | Path,
-                chunk_size: int,
-                conn: Connection,
-                logger: Logger) -> None:
+def update_lob(errors: list[str],
+               lob_table: str,
+               lob_column: str,
+               pk_columns: list[str],
+               pk_vals: tuple,
+               lob_file: str | Path,
+               chunk_size: int,
+               conn: Connection,
+               logger: Logger) -> None:
     """
     Update a large binary objects (LOB) in the given table and column.
 
     :param errors: incidental error messages
     :param lob_table: the table to be update with the new LOB
     :param lob_column: the column to be updated with the new LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param pk_vals: values with which to locate the tuple to be updated
     :param lob_file: file holding the LOB (a file object or a valid path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     """
     # make sure to have a connection
-    curr_conn: Connection = conn or _connect(errors=errors,
-                                             logger=logger)
+    curr_conn: Connection = conn or connect(errors=errors,
+                                            logger=logger)
 
     # make sure to have a data file
     data_file: Path = Path(lob_file) if isinstance(lob_file, str) else lob_file
 
     # normalize the chunk size
     if not chunk_size:
         chunk_size = -1
@@ -253,19 +254,19 @@
                 engine="sqlserver",
                 err_msg=err_msg,
                 errors=errors,
                 stmt=update_stmt,
                 bind_vals=pk_vals)
 
 
-def _execute(errors: list[str],
-             exc_stmt: str,
-             bind_vals: tuple,
-             conn: Connection,
-             logger: Logger) -> int:
+def execute(errors: list[str],
+            exc_stmt: str,
+            bind_vals: tuple,
+            conn: Connection,
+            logger: Logger) -> int:
     """
     Execute the command *exc_stmt* on the database.
 
     This command might be a DML ccommand modifying the database, such as
     inserting, updating or deleting tuples, or it might be a DDL statement,
     or it might even be an environment-related command.
     The optional bind values for this operation are in *bind_vals*.
@@ -280,16 +281,16 @@
     :param logger: optional logger
     :return: the return value from the command execution
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
-    curr_conn: Connection = conn or _connect(errors=errors,
-                                             logger=logger)
+    curr_conn: Connection = conn or connect(errors=errors,
+                                            logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
             cursor.execute(exc_stmt, bind_vals)
             result = cursor.rowcount
@@ -313,35 +314,35 @@
                 errors=errors,
                 stmt=exc_stmt,
                 bind_vals=bind_vals)
 
     return result
 
 
-def _call_procedure(errors: list[str],
-                    proc_name: str,
-                    proc_vals: tuple,
-                    conn: Connection,
-                    logger: Logger = None) -> list[tuple]:
+def call_procedure(errors: list[str],
+                   proc_name: str,
+                   proc_vals: tuple,
+                   conn: Connection,
+                   logger: Logger = None) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
     :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     result: list[tuple] | None = None
 
     # make sure to have a connection
-    curr_conn: Connection = conn or _connect(errors=errors,
-                                             logger=logger)
+    curr_conn: Connection = conn or connect(errors=errors,
+                                            logger=logger)
 
     # build the command
     proc_stmt: str | None = None
 
     # execute the stored procedure
     err_msg: str | None = None
     try:
```

### Comparing `pypomes_db-0.8.5/LICENSE` & `pypomes_db-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.5/pyproject.toml` & `pypomes_db-0.8.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.8.5"
+version = "0.8.6"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.8.5/PKG-INFO` & `pypomes_db-0.8.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.8.5
+Version: 0.8.6
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


# Comparing `tmp/pypomes_db-0.8.6.tar.gz` & `tmp/pypomes_db-0.8.7.tar.gz`

## Comparing `pypomes_db-0.8.6.tar` & `pypomes_db-0.8.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    31452 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    18598 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    15146 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    13914 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.8.7/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 pypomes_db-0.8.7/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    34799 2020-02-02 00:00:00.000000 pypomes_db-0.8.7/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    18598 2020-02-02 00:00:00.000000 pypomes_db-0.8.7/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.7/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 pypomes_db-0.8.7/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    16635 2020-02-02 00:00:00.000000 pypomes_db-0.8.7/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    15386 2020-02-02 00:00:00.000000 pypomes_db-0.8.7/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.8.7/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.8.7/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.7/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.8.7/PKG-INFO
```

### Comparing `pypomes_db-0.8.6/src/pypomes_db/__init__.py` & `pypomes_db-0.8.7/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.6/src/pypomes_db/db_common.py` & `pypomes_db-0.8.7/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.6/src/pypomes_db/db_pomes.py` & `pypomes_db-0.8.7/src/pypomes_db/db_pomes.py`

 * *Files 14% similar despite different names*

```diff
@@ -125,22 +125,24 @@
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def db_connect(errors: list[str] | None,
+               autocommit: bool = False,
                engine: str = None,
                logger: Logger = None) -> Any:
     """
     Obtain and return a connection to the database, or *None* if the connection cannot be obtained.
 
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
+    :param autocommit: whether the connection is to be in autocommit mode (defaults to False)
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param logger: optional logger
     :return: the connection to the database
     """
     # initialize the return variable
     result: Any = None
 
@@ -173,28 +175,30 @@
 
 def db_exists(errors: list[str],
               table: str,
               where_attrs: list[str] = None,
               where_vals: tuple = None,
               engine: str = None,
               conn: Any = None,
+              committable: bool = True,
               logger: Logger = None) -> bool:
     """
     Determine whether the table *table* in the database contains at least one tuple.
 
     For this determination, *where_attrs* are made equal to *where_values* in the query, respectively.
     If more than one, the attributes are concatenated by the *AND* logical connector.
     The targer database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param table: the table to be searched
     :param where_attrs: the search attributes
     :param where_vals: the values for the search attributes
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: True if at least one tuple was found
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     # noinspection PyDataSource
@@ -203,14 +207,15 @@
         sel_stmt += " WHERE " + "".join(f"{attr} = %s AND " for attr in where_attrs)[0:-5]
     rec: tuple = db_select_one(errors=op_errors,
                                sel_stmt=sel_stmt,
                                where_vals=where_vals,
                                require_nonempty=False,
                                engine = engine,
                                conn=conn,
+                               committable=committable,
                                logger=logger)
     result: bool = None if op_errors else rec is not None
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
@@ -218,14 +223,15 @@
 
 def db_select_one(errors: list[str] | None,
                   sel_stmt: str,
                   where_vals: tuple = None,
                   require_nonempty: bool = False,
                   engine: str = None,
                   conn: Any = None,
+                  committable: bool = True,
                   logger: Logger = None) -> tuple:
     """
     Search the database and return the first tuple that satisfies the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. In case of error, or if the search is empty, *None* is returned.
@@ -233,26 +239,28 @@
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: values to be associated with the search criteria
     :param require_nonempty: defines whether an empty search should be considered an error
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: tuple containing the search result, [] if the search was empty, or None if there was an error
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     require_min: int = 1 if require_nonempty else None
     reply: list[tuple] = db_select_all(errors=op_errors,
                                        sel_stmt=sel_stmt,
                                        where_vals=where_vals,
                                        require_min=require_min,
                                        require_max=1,
+                                       committable=committable,
                                        engine=engine,
                                        conn=conn,
                                        logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
@@ -262,14 +270,15 @@
 def db_select_all(errors: list[str] | None,
                   sel_stmt: str,
                   where_vals: tuple = None,
                   require_min: int = None,
                   require_max: int = None,
                   engine: str = None,
                   conn: Any = None,
+                  committable: bool = True,
                   logger: Logger = None) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
@@ -279,14 +288,15 @@
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] | None = None
 
     # initialize the local errors list
@@ -301,95 +311,103 @@
         from . import oracle_pomes
         result = oracle_pomes.select_all(errors=op_errors,
                                          sel_stmt=sel_stmt,
                                          where_vals=where_vals,
                                          require_min=require_min,
                                          require_max=require_max,
                                          conn=conn,
+                                         committable=committable,
                                          logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
         result = postgres_pomes.select_all(errors=op_errors,
                                            sel_stmt=sel_stmt,
                                            where_vals=where_vals,
                                            require_min=require_min,
                                            require_max=require_max,
                                            conn=conn,
+                                           committable=committable,
                                            logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
         result = sqlserver_pomes.select_all(errors=op_errors,
                                             sel_stmt=sel_stmt,
                                             where_vals=where_vals,
                                             require_min=require_min,
                                             require_max=require_max,
                                             conn=conn,
+                                            committable=committable,
                                             logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def db_insert(errors: list[str] | None,
               insert_stmt: str,
               insert_vals: tuple,
               engine: str = None,
               conn: Any = None,
+              committable: bool = True,
               logger: Logger = None) -> int:
     """
     Insert a tuple, with values defined in *insert_vals*, into the database.
 
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the values to be inserted
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: the number of inserted tuples (0 ou 1), or None if an error occurred
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     result: int = db_execute(errors=op_errors,
                              exc_stmt=insert_stmt,
                              bind_vals=insert_vals,
                              engine=engine,
                              conn=conn,
+                             committable=committable,
                              logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def db_update(errors: list[str] | None,
               update_stmt: str,
               update_vals: tuple = None,
               where_vals: tuple = None,
               engine: str = None,
               conn: Any = None,
+              committable: bool = True,
               logger: Logger = None) -> int:
     """
     Update one or more tuples in the database, as defined by the command *update_stmt*.
 
     The values for this update are in *update_vals*.
     The values for selecting the tuples to be updated are in *where_vals*.
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param update_stmt: the UPDATE command
     :param update_vals: the values for the update operation
     :param where_vals: the values to be associated with the search criteria
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: the number of updated tuples, or None if an error occurred
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     bind_vals: tuple | None = None
@@ -400,74 +418,80 @@
     elif where_vals:
         bind_vals = where_vals
     result: int = db_execute(errors=op_errors,
                              exc_stmt=update_stmt,
                              bind_vals=bind_vals,
                              engine=engine,
                              conn=conn,
+                             committable=committable,
                              logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def db_delete(errors: list[str] | None,
               delete_stmt: str,
               where_vals: tuple = None,
               engine: str = None,
               conn: Any = None,
+              committable: bool = True,
               logger: Logger = None) -> int:
     """
     Delete one or more tuples in the database, as defined by the *delete_stmt* command.
 
     The values for selecting the tuples to be deleted are in *where_vals*.
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param delete_stmt: the DELETE command
     :param where_vals: the values to be associated with the search criteria
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: the number of deleted tuples, or None if an error occurred
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     result: int = db_execute(errors=op_errors,
                              exc_stmt=delete_stmt,
                              bind_vals=where_vals,
                              engine=engine,
                              conn=conn,
+                             committable=committable,
                              logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def db_bulk_insert(errors: list[str] | None,
                    insert_stmt: str,
                    insert_vals: list[tuple],
                    engine: str = None,
                    conn: Any = None,
+                   committable: bool = True,
                    logger: Logger = None) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     # initialize the local errors list
@@ -480,28 +504,31 @@
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
         result = oracle_pomes.bulk_insert(errors=op_errors,
                                           insert_stmt=insert_stmt,
                                           insert_vals=insert_vals,
                                           conn=conn,
+                                          committable=committable,
                                           logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
         result = postgres_pomes.bulk_insert(errors=op_errors,
                                             insert_stmt=insert_stmt,
                                             insert_vals=insert_vals,
                                             conn=conn,
+                                            committable=committable,
                                             logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
         result = sqlserver_pomes.bulk_insert(errors=op_errors,
                                              insert_stmt=insert_stmt,
                                              insert_vals=insert_vals,
                                              conn=conn,
+                                             committable=committable,
                                              logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
@@ -511,27 +538,29 @@
                   lob_column: str,
                   pk_columns: list[str],
                   pk_vals: tuple,
                   lob_file: str | Path,
                   chunk_size: int,
                   engine: str = None,
                   conn: Any = None,
+                  committable: bool = True,
                   logger: Logger = None) -> None:
     """
     Update a large binary objects (LOB) in the given table and column.
 
     :param errors: incidental error messages
     :param lob_table: the table to be update with the new LOB
     :param lob_column: the column to be updated with the new LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param pk_vals: values with which to locate the tuple to be updated
     :param lob_file: file holding the LOB (a file object or a valid path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: number of LOBs effectively copied
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     # determine the database engine
@@ -545,47 +574,51 @@
                                 lob_table=lob_table,
                                 lob_column=lob_column,
                                 pk_columns=pk_columns,
                                 pk_vals=pk_vals,
                                 lob_file=lob_file,
                                 chunk_size=chunk_size,
                                 conn=conn,
+                                committable=committable,
                                 logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
         postgres_pomes.update_lob(errors=op_errors,
                                   lob_table=lob_table,
                                   lob_column=lob_column,
                                   pk_columns=pk_columns,
                                   pk_vals=pk_vals,
                                   lob_file=lob_file,
                                   chunk_size=chunk_size,
                                   conn=conn,
+                                  committable=committable,
                                   logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
         sqlserver_pomes.update_lob(errors=op_errors,
                                    lob_table=lob_table,
                                    lob_column=lob_column,
                                    pk_columns=pk_columns,
                                    pk_vals=pk_vals,
                                    lob_file=lob_file,
                                    chunk_size=chunk_size,
                                    conn=conn,
+                                   committable=committable,
                                    logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
 
 def db_execute(errors: list[str] | None,
                exc_stmt: str,
                bind_vals: tuple = None,
                engine: str = None,
                conn: Any = None,
+               committable: bool = True,
                logger: Logger = None) -> int:
     """
     Execute the command *exc_stmt* on the database.
 
     This command might be a DML ccommand modifying the database, such as
     inserting, updating or deleting tuples, or it might be a DDL statement,
     or it might even be an environment-related command.
@@ -595,14 +628,15 @@
     ou None if an error occurred.
 
     :param errors: incidental error messages
     :param exc_stmt: the command to execute
     :param bind_vals: optional bind values
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: the return value from the command execution
     """
     # initialize the return variable
     result: int | None = None
 
     # initialize the local errors list
@@ -615,52 +649,57 @@
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
         result = oracle_pomes.execute(errors=op_errors,
                                       exc_stmt=exc_stmt,
                                       bind_vals=bind_vals,
                                       conn=conn,
+                                      committable=committable,
                                       logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
         result = postgres_pomes.db_execute(errors=op_errors,
                                            exc_stmt=exc_stmt,
                                            bind_vals=bind_vals,
                                            conn=conn,
+                                           committable=committable,
                                            logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
         result = sqlserver_pomes.execute(errors=op_errors,
                                          exc_stmt=exc_stmt,
                                          bind_vals=bind_vals,
                                          conn=conn,
+                                         committable=committable,
                                          logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def db_call_function(errors: list[str] | None,
                      func_name: str,
                      func_vals: tuple = None,
                      engine: str = None,
                      conn: Any = None,
+                     committable: bool = True,
                      logger: Logger = None) -> list[tuple]:
     """
     Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
 
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param func_name: name of the stored function
     :param func_vals: parameters for the stored function
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: the data returned by the function
     """
     # initialize the return variable
     result: Any = None
 
     # initialize the local errors list
@@ -673,52 +712,57 @@
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
         result = oracle_pomes.call_function(errors=op_errors,
                                             func_name=func_name,
                                             func_vals=func_vals,
                                             conn=conn,
+                                            committable=committable,
                                             logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
         result = postgres_pomes.call_procedure(errors=op_errors,
                                                proc_name=func_name,
                                                proc_vals=func_vals,
                                                conn=conn,
+                                               committable=committable,
                                                logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
         result = sqlserver_pomes.call_procedure(errors=op_errors,
                                                 proc_name=func_name,
                                                 proc_vals=func_vals,
                                                 conn=conn,
+                                                committable=committable,
                                                 logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def db_call_procedure(errors: list[str] | None,
                       proc_name: str,
                       proc_vals: tuple = None,
                       engine: str = None,
                       conn: Any = None,
+                      committable: bool = True,
                       logger: Logger = None) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     result: Any = None
 
     # initialize the local errors list
@@ -731,27 +775,30 @@
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
         result = oracle_pomes.call_procedure(errors=op_errors,
                                              proc_name=proc_name,
                                              proc_vals=proc_vals,
                                              conn=conn,
+                                             committable=committable,
                                              logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
         result = postgres_pomes.call_procedure(errors=op_errors,
                                                proc_name=proc_name,
                                                proc_vals=proc_vals,
                                                conn=conn,
+                                               committable=committable,
                                                logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
         result = sqlserver_pomes.call_procedure(errors=op_errors,
                                                 proc_name=proc_name,
                                                 proc_vals=proc_vals,
                                                 conn=conn,
+                                                committable=committable,
                                                 logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
```

### Comparing `pypomes_db-0.8.6/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.8.7/src/pypomes_db/migration_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.6/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.8.7/src/pypomes_db/postgres_pomes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,70 @@
 # noinspection DuplicatedCode
-import oracledb
-from logging import Logger
-from oracledb import Connection, init_oracle_client
+import psycopg2
+from logging import WARNING, Logger
 from pathlib import Path
+from psycopg2 import Binary
+from psycopg2.extras import execute_values
+# noinspection PyProtectedMember
+from psycopg2._psycopg import connection
+from typing import Any
 
 from .db_common import (
-    _DB_CONN_DATA,
-    _db_assert_query_quota, _db_get_params, _db_log, _db_except_msg
+    _db_assert_query_quota, _db_get_params,
+    _db_log, _db_except_msg, _db_remove_nulls
 )
 
 
 def connect(errors: list[str],
-            logger: Logger) -> Connection:
+            autocommit: bool,
+            logger: Logger = None) -> connection:
     """
     Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
     :param errors: incidental error messages
+    :param autocommit: whether the connection is to be in autocommit mode
     :param logger: optional logger
     :return: the connection to the database
     """
     # initialize the return variable
-    result: Connection | None = None
+    result: connection | None = None
 
     # retrieve the connection parameters
-    name, user, pwd, host, port = _db_get_params("oracle")
+    name, user, pwd, host, port = _db_get_params("postgres")
 
     # obtain a connection to the database
     err_msg: str | None = None
     try:
-        result = oracledb.connect(service_name=name,
-                                  host=host,
+        result = psycopg2.connect(host=host,
                                   port=port,
+                                  database=name,
                                   user=user,
                                   password=pwd)
-        # make sure the connection is not in autocommit mode
-        result.autocommit = False
+        # establish the connection's autocommit mode
+        result.autocommit = autocommit
     except Exception as e:
-        err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+        err_msg = _db_except_msg(e, "postgres")
 
     # log the results
     _db_log(logger=logger,
-            engine="oracle",
+            engine="postgres",
             err_msg=err_msg,
             errors=errors,
             stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
 def select_all(errors: list[str],
                sel_stmt: str,
                where_vals: tuple,
                require_min: int,
                require_max: int,
-               conn: Connection,
+               conn: connection,
+               committable: bool,
                logger: Logger) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
@@ -66,210 +72,248 @@
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
-    :return: tuple containing the search result, [] if the search was empty, or None if there was an error
+    :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
-    curr_conn: Connection = conn or connect(errors=errors,
+    curr_conn: connection = conn or connect(errors=errors,
+                                            autocommit=False,
                                             logger=logger)
 
-    if isinstance(require_max, int) and require_max > 0:
-        sel_stmt: str = f"{sel_stmt} FETCH NEXT {require_max} ROWS ONLY"
+    if isinstance(require_max, int) and require_max >= 0:
+        sel_stmt += f" LIMIT {require_max}"
 
     err_msg: str | None = None
     try:
-        # obtain a cursor and perform the operation
+        # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
-            # execute the query
-            cursor.execute(statement=sel_stmt,
-                           parameters=where_vals)
+            cursor.execute(query=f"{sel_stmt};",
+                           vars=where_vals)
             # obtain the number of tuples returned
             count: int = cursor.rowcount
 
             # has the query quota been satisfied ?
             if _db_assert_query_quota(errors=errors,
-                                      engine="oracle",
+                                      engine="postgres",
                                       query=sel_stmt,
                                       where_vals=where_vals,
                                       count=count,
                                       require_min=require_min,
                                       require_max=require_max):
                 # yes, retrieve the returned tuples
-                rows: list = cursor.fetchall()
-                result = [tuple(row) for row in rows]
-        # commit the transaction
-        curr_conn.commit()
+                result = list(cursor)
+
+        # commit the transaction, if appropriate
+        if committable or not conn:
+            curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine="postgres")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
         _db_log(logger=logger,
-                engine="oracle",
+                engine="postgres",
                 err_msg=err_msg,
                 errors=errors,
                 stmt=sel_stmt,
                 bind_vals=where_vals)
 
     return result
 
 
 def bulk_insert(errors: list[str],
                 insert_stmt: str,
                 insert_vals: list[tuple],
-                conn: Connection,
+                conn: connection,
+                committable: bool,
                 logger: Logger) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
-    The binding must be done by position. Thus, the *VALUES* clause in *insert_stmt*
-    must contain as many ':n' placeholders as there are elements in the tuples found in the
-    list provided in *insert_vals*, where 'n' is the 1-based position of the data in the tuple.
+    The *VALUES* clause in *insert_stmt* must be simply *VALUES %s*.
+    Note that, after the execution of *execute_values*, the *cursor.rowcount* property
+    will not contain a total result, and thus the value 1 (one) is returned on success.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
-    curr_conn: Connection = conn or connect(errors=errors,
+    curr_conn: connection = conn or connect(errors=errors,
+                                            autocommit=False,
                                             logger=logger)
 
+    # execute the bulk insert
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
-            cursor.executemany(statement=insert_stmt,
-                               parameters=insert_vals)
+            execute_values(cur=cursor,
+                           sql=insert_stmt,
+                           argslist=insert_vals)
             result = len(insert_vals)
-        curr_conn.commit()
+
+        # commit the transaction, if appropriate
+        if committable or not conn:
+            curr_conn.commit()
+    except ValueError as e:
+        curr_conn.rollback()
+        # is the exception ValueError("A string literal cannot contain NUL (0x00) characters.") ?
+        if "contain NUL" in e.args[0]:
+            # yes, log the occurrence, remove the NULLs, and try again
+            _db_log(logger=logger,
+                    engine="postgres",
+                    level=WARNING,
+                    stmt=f"Found NULLs in values for {insert_stmt}")
+            # search for NULLs in input data
+            cleaned_rows: list[tuple[int, list]] = []
+            for inx, vals in enumerate(insert_vals):
+                cleaned_row: list[Any] = _db_remove_nulls(vals)
+                # has the row been cleaned ?
+                if cleaned_row:
+                    # yes, register it
+                    cleaned_rows.append((inx, cleaned_row))
+            # replace the cleaned rows
+            for cleaned_row in cleaned_rows:
+                insert_vals[cleaned_row[0]] = tuple(cleaned_row[1])
+            # bulk insert the cleaned data
+            bulk_insert(errors=errors,
+                        insert_stmt=insert_stmt,
+                        insert_vals=insert_vals,
+                        conn=conn,
+                        committable=committable,
+                        logger=logger)
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine="postgres")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
         _db_log(logger=logger,
-                engine="oracle",
+                engine="postgres",
                 err_msg=err_msg,
                 errors=errors,
-                stmt=insert_stmt,
-                bind_vals=insert_vals[0])
+                stmt=insert_stmt)
 
     return result
 
 
 def update_lob(errors: list[str],
                lob_table: str,
                lob_column: str,
                pk_columns: list[str],
                pk_vals: tuple,
                lob_file: str | Path,
                chunk_size: int,
-               conn: Connection,
+               conn: connection,
+               committable: bool,
                logger: Logger) -> None:
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
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     """
     # make sure to have a connection
-    curr_conn: Connection = conn or connect(errors=errors,
+    curr_conn: connection = conn or connect(errors=errors,
+                                            autocommit=False,
                                             logger=logger)
 
     # make sure to have a data file
     data_file: Path = Path(lob_file) if isinstance(lob_file, str) else lob_file
 
     # normalize the chunk size
     if not chunk_size:
         chunk_size = -1
 
     # build the UPDATE query
-    where_clause: str = " AND ".join([f"{column} = :{inx}"
-                                      for column, inx in enumerate(iterable=pk_columns,
-                                                                   start=2)])
+    where_clause: str = " AND ".join([f"{column} = %s" for column in pk_columns])
     update_stmt: str = (f"UPDATE {lob_table} "
-                        f"SET {lob_column} = :1 "
+                        f"SET {lob_column} = %s "
                         f"WHERE {where_clause}")
 
     err_msg: str | None = None
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
 
             # retrieve the lob data from file in chunks and write to the file
             lob_data : bytes
             with data_file.open("rb") as file:
                 lob_data = file.read(chunk_size)
                 while lob_data:
-                    cursor.execute(statement=update_stmt,
-                                   parameters=(lob_data, *pk_vals))
+                    cursor.execute(update_stmt, (Binary(lob_data), *pk_vals))
                     lob_data = file.read(chunk_size)
 
-        # commit the transaction
-        curr_conn.commit()
+        # commit the transaction, if appropriate
+        if committable or not conn:
+            curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine="postgres")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
         _db_log(logger=logger,
+                engine="postgres",
                 err_msg=err_msg,
-                engine="oracle",
                 errors=errors,
                 stmt=update_stmt,
                 bind_vals=pk_vals)
 
 
-def execute(errors: list[str],
-            exc_stmt: str,
-            bind_vals: tuple,
-            conn: Connection,
-            logger: Logger) -> int:
+def db_execute(errors: list[str],
+               exc_stmt: str,
+               bind_vals: tuple,
+               conn: connection,
+               committable: bool,
+               logger: Logger) -> int:
     """
     Execute the command *exc_stmt* on the database.
 
     This command might be a DML ccommand modifying the database, such as
     inserting, updating or deleting tuples, or it might be a DDL statement,
     or it might even be an environment-related command.
     The optional bind values for this operation are in *bind_vals*.
@@ -277,160 +321,114 @@
     It might be the number of inserted, modified, or deleted tuples,
     ou None if an error occurred.
 
     :param errors: incidental error messages
     :param exc_stmt: the command to execute
     :param bind_vals: optional bind values
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: the return value from the command execution
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
-    curr_conn: Connection = conn or connect(errors=errors,
+    curr_conn: connection = conn or connect(errors=errors,
+                                            autocommit=False,
                                             logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
-            cursor.execute(statement=exc_stmt,
-                           parameters=bind_vals)
+            cursor.execute(query=f"{exc_stmt};",
+                           vars=bind_vals)
             result = cursor.rowcount
-        # commit the transaction
-        curr_conn.commit()
+
+        # commit the transaction, if appropriate
+        if committable or not conn:
+            curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine="postgres")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
         _db_log(logger=logger,
-                engine="oracle",
+                engine="postgres",
                 err_msg=err_msg,
                 errors=errors,
                 stmt=exc_stmt,
                 bind_vals=bind_vals)
 
     return result
 
 
-# TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
-# noinspection PyUnusedLocal
-def call_function(errors: list[str],
-                  func_name: str,
-                  func_vals: tuple,
-                  conn: Connection,
-                  logger: Logger) -> list[tuple]:
-    """
-    Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
-
-    :param errors: incidental error messages
-    :param func_name: name of the stored function
-    :param func_vals: parameters for the stored function
-    :param conn: optional connection to use (obtains a new one, if not provided)
-    :param logger: optional logger
-    :return: the data returned by the function
-    """
-    # initialize the return variable
-    result: list[tuple] = []
-
-    return result
-
 
-# TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
 def call_procedure(errors: list[str],
                    proc_name: str,
                    proc_vals: tuple,
-                   conn: Connection,
+                   conn: connection,
+                   committable: bool,
                    logger: Logger) -> list[tuple]:
     """
-    Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
+    Execute the stored procedure *proc_name*, with the arguments given in *proc_vals*.
 
-    :param errors: incidental error messages
-    :param proc_name: name of the stored procedure
-    :param proc_vals: parameters for the stored procedure
+    :param errors:  incidental error messages
+    :param proc_name: the name of the sotred procedure
+    :param proc_vals: the arguments to be passed
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
-    result: list[tuple] = []
+    result: list[tuple] = [()]
 
     # make sure to have a connection
-    curr_conn: Connection = conn or connect(errors=errors,
+    curr_conn: connection = conn or connect(errors=errors,
+                                            autocommit=False,
                                             logger=logger)
 
+    # build the command
+    proc_stmt: str = f"{proc_name}(" + "%s, " * (len(proc_vals) - 1) + "%s)"
+
     # execute the stored procedure
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
-            cursor.callproc(name=proc_name,
-                            parameters=proc_vals)
-
+            cursor.execute(query=proc_stmt,
+                           vars=proc_vals)
             # retrieve the returned tuples
             result = list(cursor)
-        # commit the transaction
-        curr_conn.commit()
+
+        # commit the transaction, if appropriate
+        if committable or not conn:
+            curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine="postgres")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
         _db_log(logger=logger,
-                engine="oracle",
+                engine="postgres",
                 err_msg=err_msg,
                 errors=errors,
-                stmt=proc_name,
+                stmt=proc_stmt,
                 bind_vals=proc_vals)
 
     return result
-
-__is_initialized: str | None = None
-
-def initialize(errors: list[str],
-               logger: Logger) -> bool:
-    """
-    Prepare the oracle engine to access the database throught the installed client software.
-
-    :param errors: incidental error messages
-    :param logger: optional logger
-    :return: False if an error happened, True otherwise
-    """
-    # initialize the return variable
-    result: bool = True
-
-    global __is_initialized
-    if not __is_initialized:
-        err_msg: str | None = None
-        client: str = _DB_CONN_DATA["oracle"]["client"]
-        try:
-            init_oracle_client(client)
-            __is_initialized = True
-        except Exception as e:
-            result = False
-            err_msg = _db_except_msg(exception=e,
-                                     engine="oracle")
-        # log the results
-        _db_log(logger=logger,
-                engine="oracle",
-                err_msg=err_msg,
-                errors=errors,
-                stmt="Initializing the client")
-
-    return result
```

### Comparing `pypomes_db-0.8.6/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.8.7/src/pypomes_db/sqlserver_pomes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,66 @@
 # noinspection DuplicatedCode
-import psycopg2
-from logging import WARNING, Logger
+import pyodbc
+from logging import Logger
+from pyodbc import Binary, Connection, Row
 from pathlib import Path
-from psycopg2 import Binary
-from psycopg2.extras import execute_values
-# noinspection PyProtectedMember
-from psycopg2._psycopg import connection
-from typing import Any
 
 from .db_common import (
-    _db_assert_query_quota, _db_get_params,
-    _db_log, _db_except_msg, _db_remove_nulls
+    _db_assert_query_quota, _db_get_params, _db_log, _db_except_msg
 )
 
 
 def connect(errors: list[str],
-            logger: Logger = None) -> connection:
+            autocommit: bool,
+            logger: Logger = None) -> Connection:
     """
     Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
     :param errors: incidental error messages
+    :param autocommit: whether the connection is to be in autocommit mode
     :param logger: optional logger
     :return: the connection to the database
     """
-    # initialize the return variable
-    result: connection | None = None
+    # initialize the return valiable
+    result: Connection | None = None
 
-    # retrieve the connection parameters
-    name, user, pwd, host, port = _db_get_params("postgres")
+    # retrieve the connection parameters and build the connection string
+    name, user, pwd, host, port, driver = _db_get_params("sqlserver")
+    connection_kwargs: str = (
+        f"DRIVER={{{driver}}};SERVER={host},{port};"
+        f"DATABASE={name};UID={user};PWD={pwd};TrustServerCertificate=yes;"
+    )
 
     # obtain a connection to the database
     err_msg: str | None = None
     try:
-        result = psycopg2.connect(host=host,
-                                  port=port,
-                                  database=name,
-                                  user=user,
-                                  password=pwd)
-        # make sure the connection is not in autocommit mode
-        result.autocommit = False
+        result = pyodbc.connect(connection_kwargs)
+        # establish the connection's autocommit mode
+        result.autocommit = autocommit
     except Exception as e:
-        err_msg = _db_except_msg(e, "postgres")
+        err_msg = _db_except_msg(exception=e,
+                                 engine="sqlserver")
 
     # log the results
     _db_log(logger=logger,
-            engine="postgres",
+            engine="sqlserver",
             err_msg=err_msg,
             errors=errors,
             stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
 def select_all(errors: list[str],
                sel_stmt: str,
                where_vals: tuple,
                require_min: int,
                require_max: int,
-               conn: connection,
+               conn: Connection,
+               committable: bool,
                logger: Logger) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
@@ -69,192 +68,179 @@
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
-    :return: list of tuples containing the search result, or [] if the search is empty
+    :return: tuple containing the search result, [] if the search was empty, or None if there was an error
     """
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
-    curr_conn: connection = conn or connect(errors=errors,
+    curr_conn: Connection = conn or connect(errors=errors,
+                                            autocommit=False,
                                             logger=logger)
 
-    if isinstance(require_max, int) and require_max >= 0:
-        sel_stmt += f" LIMIT {require_max}"
-
     err_msg: str | None = None
+    if isinstance(require_max, int) and require_max > 0:
+        sel_stmt: str = sel_stmt.replace("SELECT", f"SELECT TOP {require_max}", 1)
+
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
-            cursor.execute(query=f"{sel_stmt};",
-                           vars=where_vals)
+            cursor.execute(sel_stmt, where_vals)
             # obtain the number of tuples returned
             count: int = cursor.rowcount
 
             # has the query quota been satisfied ?
             if _db_assert_query_quota(errors=errors,
-                                      engine="postgres",
+                                      engine="sqlserver",
                                       query=sel_stmt,
                                       where_vals=where_vals,
                                       count=count,
                                       require_min=require_min,
                                       require_max=require_max):
                 # yes, retrieve the returned tuples
-                result = list(cursor)
+                rows: list[Row] = cursor.fetchall()
+                result = [tuple(row) for row in rows]
 
-        # commit the transaction
-        curr_conn.commit()
+        # commit the transaction, if appropriate
+        if committable or not conn:
+            curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="postgres")
+                                 engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
         _db_log(logger=logger,
-                engine="postgres",
+                engine="sqlserver",
                 err_msg=err_msg,
                 errors=errors,
                 stmt=sel_stmt,
                 bind_vals=where_vals)
 
     return result
 
 
 def bulk_insert(errors: list[str],
                 insert_stmt: str,
                 insert_vals: list[tuple],
-                conn: connection,
+                conn: Connection,
+                committable: bool,
                 logger: Logger) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
-    The *VALUES* clause in *insert_stmt* must be simply *VALUES %s*.
-    Note that, after the execution of *execute_values*, the *cursor.rowcount* property
-    will not contain a total result, and thus the value 1 (one) is returned on success.
+    The *VALUES* clause in *insert_stmt* must contain as many '%s' placeholders
+    as there are elements in the tuples found in the list provided in *insert_vals*.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
-    curr_conn: connection = conn or connect(errors=errors,
+    curr_conn: Connection = conn or connect(errors=errors,
+                                            autocommit=False,
                                             logger=logger)
 
-    # execute the bulk insert
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
-            execute_values(cur=cursor,
-                           sql=insert_stmt,
-                           argslist=insert_vals)
-            result = len(insert_vals)
-        # commit the transaction
-        curr_conn.commit()
-    except ValueError as e:
-        curr_conn.rollback()
-        # is the exception ValueError("A string literal cannot contain NUL (0x00) characters.") ?
-        if "contain NUL" in e.args[0]:
-            # yes, log the occurrence, remove the NULLs, and try again
-            _db_log(logger=logger,
-                    engine="postgres",
-                    level=WARNING,
-                    stmt=f"Found NULLs in values for {insert_stmt}")
-            # search for NULLs in input data
-            cleaned_rows: list[tuple[int, list]] = []
-            for inx, vals in enumerate(insert_vals):
-                cleaned_row: list[Any] = _db_remove_nulls(vals)
-                # has the row been cleaned ?
-                if cleaned_row:
-                    # yes, register it
-                    cleaned_rows.append((inx, cleaned_row))
-            # replace the cleaned rows
-            for cleaned_row in cleaned_rows:
-                insert_vals[cleaned_row[0]] = tuple(cleaned_row[1])
-            # bulk insert the cleaned data
-            bulk_insert(errors=errors,
-                        insert_stmt=insert_stmt,
-                        insert_vals=insert_vals,
-                        conn=conn,
-                        logger=logger)
+            cursor.fast_executemany = True
+            try:
+                cursor.executemany(insert_stmt, insert_vals)
+                result = len(insert_vals)
+            except Exception:
+                conn.rollback()
+                raise
+
+        # commit the transaction, if appropriate
+        if committable or not conn:
+            curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="postgres")
+                                 engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
         _db_log(logger=logger,
-                engine="postgres",
+                engine="sqlserver",
                 err_msg=err_msg,
                 errors=errors,
-                stmt=insert_stmt)
+                stmt=insert_stmt,
+                bind_vals=insert_vals[0])
 
     return result
 
 
 def update_lob(errors: list[str],
                lob_table: str,
                lob_column: str,
                pk_columns: list[str],
                pk_vals: tuple,
                lob_file: str | Path,
                chunk_size: int,
-               conn: connection,
+               conn: Connection,
+               committable: bool,
                logger: Logger) -> None:
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
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     """
     # make sure to have a connection
-    curr_conn: connection = conn or connect(errors=errors,
+    curr_conn: Connection = conn or connect(errors=errors,
+                                            autocommit=False,
                                             logger=logger)
 
     # make sure to have a data file
     data_file: Path = Path(lob_file) if isinstance(lob_file, str) else lob_file
 
     # normalize the chunk size
     if not chunk_size:
         chunk_size = -1
 
     # build the UPDATE query
-    where_clause: str = " AND ".join([f"{column} = %s" for column in pk_columns])
+    where_clause: str = " AND ".join([f"{column} = ?" for column in pk_columns])
     update_stmt: str = (f"UPDATE {lob_table} "
-                        f"SET {lob_column} = %s "
+                        f"SET {lob_column} = ? "
                         f"WHERE {where_clause}")
 
     err_msg: str | None = None
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
 
@@ -262,41 +248,43 @@
             lob_data : bytes
             with data_file.open("rb") as file:
                 lob_data = file.read(chunk_size)
                 while lob_data:
                     cursor.execute(update_stmt, (Binary(lob_data), *pk_vals))
                     lob_data = file.read(chunk_size)
 
-        # commit the transaction
-        curr_conn.commit()
+        # commit the transaction, if appropriate
+        if committable or not conn:
+            curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="postgres")
+                                 engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
         _db_log(logger=logger,
-                engine="postgres",
+                engine="sqlserver",
                 err_msg=err_msg,
                 errors=errors,
                 stmt=update_stmt,
                 bind_vals=pk_vals)
 
 
-def db_execute(errors: list[str],
-               exc_stmt: str,
-               bind_vals: tuple,
-               conn: connection,
-               logger: Logger) -> int:
+def execute(errors: list[str],
+            exc_stmt: str,
+            bind_vals: tuple,
+            conn: Connection,
+            committable: bool,
+            logger: Logger) -> int:
     """
     Execute the command *exc_stmt* on the database.
 
     This command might be a DML ccommand modifying the database, such as
     inserting, updating or deleting tuples, or it might be a DDL statement,
     or it might even be an environment-related command.
     The optional bind values for this operation are in *bind_vals*.
@@ -304,105 +292,113 @@
     It might be the number of inserted, modified, or deleted tuples,
     ou None if an error occurred.
 
     :param errors: incidental error messages
     :param exc_stmt: the command to execute
     :param bind_vals: optional bind values
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: the return value from the command execution
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
-    curr_conn: connection = conn or connect(errors=errors,
+    curr_conn: Connection = conn or connect(errors=errors,
+                                            autocommit=False,
                                             logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
-            cursor.execute(query=f"{exc_stmt};",
-                           vars=bind_vals)
+            cursor.execute(exc_stmt, bind_vals)
             result = cursor.rowcount
-        # commit the transaction
-        curr_conn.commit()
+
+        # commit the transaction, if appropriate
+        if committable or not conn:
+            curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="postgres")
+                                 engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
         _db_log(logger=logger,
-                engine="postgres",
+                engine="sqlserver",
                 err_msg=err_msg,
                 errors=errors,
                 stmt=exc_stmt,
                 bind_vals=bind_vals)
 
     return result
 
 
-
 def call_procedure(errors: list[str],
                    proc_name: str,
                    proc_vals: tuple,
-                   conn: connection,
-                   logger: Logger) -> list[tuple]:
+                   conn: Connection,
+                   committable: bool,
+                   logger: Logger = None) -> list[tuple]:
     """
-    Execute the stored procedure *proc_name*, with the arguments given in *proc_vals*.
+    Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
-    :param errors:  incidental error messages
-    :param proc_name: the name of the sotred procedure
-    :param proc_vals: the arguments to be passed
+    :param errors: incidental error messages
+    :param proc_name: name of the stored procedure
+    :param proc_vals: parameters for the stored procedure
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
-    result: list[tuple] = [()]
+    result: list[tuple] | None = None
 
     # make sure to have a connection
-    curr_conn: connection = conn or connect(errors=errors,
+    curr_conn: Connection = conn or connect(errors=errors,
+                                            autocommit=False,
                                             logger=logger)
 
     # build the command
-    proc_stmt: str = f"{proc_name}(" + "%s, " * (len(proc_vals) - 1) + "%s)"
+    proc_stmt: str | None = None
 
     # execute the stored procedure
     err_msg: str | None = None
     try:
-        # obtain a cursor and perform the operation
+        # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
-            cursor.execute(query=proc_stmt,
-                           vars=proc_vals)
+            proc_stmt = f"SET NOCOUNT ON; EXEC {proc_name} {','.join(('?',) * len(proc_vals))}"
+            cursor.execute(proc_stmt, proc_vals)
             # retrieve the returned tuples
-            result = list(cursor)
-        # commit the transaction
-        curr_conn.commit()
+            rows: list[Row] = cursor.fetchall()
+            result = [tuple(row) for row in rows]
+
+        # commit the transaction, if appropriate
+        if committable or not conn:
+            curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="postgres")
+                                 engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
         _db_log(logger=logger,
-                engine="postgres",
+                engine="sqlserver",
                 err_msg=err_msg,
                 errors=errors,
                 stmt=proc_stmt,
                 bind_vals=proc_vals)
 
     return result
```

### Comparing `pypomes_db-0.8.6/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.8.7/src/pypomes_db/oracle_pomes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,67 @@
 # noinspection DuplicatedCode
-import pyodbc
+import oracledb
 from logging import Logger
-from pyodbc import Binary, Connection, Row
+from oracledb import Connection, init_oracle_client
 from pathlib import Path
 
 from .db_common import (
+    _DB_CONN_DATA,
     _db_assert_query_quota, _db_get_params, _db_log, _db_except_msg
 )
 
 
 def connect(errors: list[str],
-            logger: Logger = None) -> Connection:
+            autocommit: bool,
+            logger: Logger) -> Connection:
     """
     Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
     :param errors: incidental error messages
+    :param autocommit: whether the connection is to be in autocommit mode
     :param logger: optional logger
     :return: the connection to the database
     """
-    # initialize the return valiable
+    # initialize the return variable
     result: Connection | None = None
 
-    # retrieve the connection parameters and build the connection string
-    name, user, pwd, host, port, driver = _db_get_params("sqlserver")
-    connection_kwargs: str = (
-        f"DRIVER={{{driver}}};SERVER={host},{port};"
-        f"DATABASE={name};UID={user};PWD={pwd};TrustServerCertificate=yes;"
-    )
+    # retrieve the connection parameters
+    name, user, pwd, host, port = _db_get_params("oracle")
 
     # obtain a connection to the database
     err_msg: str | None = None
     try:
-        result = pyodbc.connect(connection_kwargs)
-        # make sure the connection is not in autocommit mode
-        result.autocommit = False
+        result = oracledb.connect(service_name=name,
+                                  host=host,
+                                  port=port,
+                                  user=user,
+                                  password=pwd)
+        # establish the connection's autocommit mode
+        result.autocommit = autocommit
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+                                 engine="oracle")
 
     # log the results
     _db_log(logger=logger,
-            engine="sqlserver",
+            engine="oracle",
             err_msg=err_msg,
             errors=errors,
             stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
 def select_all(errors: list[str],
                sel_stmt: str,
                where_vals: tuple,
                require_min: int,
                require_max: int,
                conn: Connection,
+               committable: bool,
                logger: Logger) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
@@ -65,121 +69,129 @@
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: tuple containing the search result, [] if the search was empty, or None if there was an error
     """
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
     curr_conn: Connection = conn or connect(errors=errors,
+                                            autocommit=False,
                                             logger=logger)
 
-    err_msg: str | None = None
     if isinstance(require_max, int) and require_max > 0:
-        sel_stmt: str = sel_stmt.replace("SELECT", f"SELECT TOP {require_max}", 1)
+        sel_stmt: str = f"{sel_stmt} FETCH NEXT {require_max} ROWS ONLY"
 
+    err_msg: str | None = None
     try:
-        # obtain a cursor and execute the operation
+        # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
-            cursor.execute(sel_stmt, where_vals)
+            # execute the query
+            cursor.execute(statement=sel_stmt,
+                           parameters=where_vals)
             # obtain the number of tuples returned
             count: int = cursor.rowcount
 
             # has the query quota been satisfied ?
             if _db_assert_query_quota(errors=errors,
-                                      engine="sqlserver",
+                                      engine="oracle",
                                       query=sel_stmt,
                                       where_vals=where_vals,
                                       count=count,
                                       require_min=require_min,
                                       require_max=require_max):
                 # yes, retrieve the returned tuples
-                rows: list[Row] = cursor.fetchall()
+                rows: list = cursor.fetchall()
                 result = [tuple(row) for row in rows]
-        # commit the transaction
-        curr_conn.commit()
+        # commit the transaction, if appropriate
+        if committable or not conn:
+            curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+                                 engine="oracle")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
         _db_log(logger=logger,
-                engine="sqlserver",
+                engine="oracle",
                 err_msg=err_msg,
                 errors=errors,
                 stmt=sel_stmt,
                 bind_vals=where_vals)
 
     return result
 
 
 def bulk_insert(errors: list[str],
                 insert_stmt: str,
                 insert_vals: list[tuple],
                 conn: Connection,
+                committable: bool,
                 logger: Logger) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
-    The *VALUES* clause in *insert_stmt* must contain as many '%s' placeholders
-    as there are elements in the tuples found in the list provided in *insert_vals*.
+    The binding must be done by position. Thus, the *VALUES* clause in *insert_stmt*
+    must contain as many ':n' placeholders as there are elements in the tuples found in the
+    list provided in *insert_vals*, where 'n' is the 1-based position of the data in the tuple.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
     curr_conn: Connection = conn or connect(errors=errors,
+                                            autocommit=False,
                                             logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
-            cursor.fast_executemany = True
-            try:
-                cursor.executemany(insert_stmt, insert_vals)
-                result = len(insert_vals)
-            except Exception:
-                conn.rollback()
-                raise
-        curr_conn.commit()
+            cursor.executemany(statement=insert_stmt,
+                               parameters=insert_vals)
+            result = len(insert_vals)
+
+        # commit the transaction, if appropriate
+        if committable or not conn:
+            curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+                                 engine="oracle")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
         _db_log(logger=logger,
-                engine="sqlserver",
+                engine="oracle",
                 err_msg=err_msg,
                 errors=errors,
                 stmt=insert_stmt,
                 bind_vals=insert_vals[0])
 
     return result
 
@@ -188,84 +200,92 @@
                lob_table: str,
                lob_column: str,
                pk_columns: list[str],
                pk_vals: tuple,
                lob_file: str | Path,
                chunk_size: int,
                conn: Connection,
+               committable: bool,
                logger: Logger) -> None:
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
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     """
     # make sure to have a connection
     curr_conn: Connection = conn or connect(errors=errors,
+                                            autocommit=False,
                                             logger=logger)
 
     # make sure to have a data file
     data_file: Path = Path(lob_file) if isinstance(lob_file, str) else lob_file
 
     # normalize the chunk size
     if not chunk_size:
         chunk_size = -1
 
     # build the UPDATE query
-    where_clause: str = " AND ".join([f"{column} = ?" for column in pk_columns])
+    where_clause: str = " AND ".join([f"{column} = :{inx}"
+                                      for column, inx in enumerate(iterable=pk_columns,
+                                                                   start=2)])
     update_stmt: str = (f"UPDATE {lob_table} "
-                        f"SET {lob_column} = ? "
+                        f"SET {lob_column} = :1 "
                         f"WHERE {where_clause}")
 
     err_msg: str | None = None
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
 
             # retrieve the lob data from file in chunks and write to the file
             lob_data : bytes
             with data_file.open("rb") as file:
                 lob_data = file.read(chunk_size)
                 while lob_data:
-                    cursor.execute(update_stmt, (Binary(lob_data), *pk_vals))
+                    cursor.execute(statement=update_stmt,
+                                   parameters=(lob_data, *pk_vals))
                     lob_data = file.read(chunk_size)
 
-        # commit the transaction
-        curr_conn.commit()
+        # commit the transaction, if appropriate
+        if committable or not conn:
+            curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+                                 engine="oracle")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
         _db_log(logger=logger,
-                engine="sqlserver",
                 err_msg=err_msg,
+                engine="oracle",
                 errors=errors,
                 stmt=update_stmt,
                 bind_vals=pk_vals)
 
 
 def execute(errors: list[str],
             exc_stmt: str,
             bind_vals: tuple,
             conn: Connection,
+            committable: bool,
             logger: Logger) -> int:
     """
     Execute the command *exc_stmt* on the database.
 
     This command might be a DML ccommand modifying the database, such as
     inserting, updating or deleting tuples, or it might be a DDL statement,
     or it might even be an environment-related command.
@@ -274,104 +294,171 @@
     It might be the number of inserted, modified, or deleted tuples,
     ou None if an error occurred.
 
     :param errors: incidental error messages
     :param exc_stmt: the command to execute
     :param bind_vals: optional bind values
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: the return value from the command execution
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
     curr_conn: Connection = conn or connect(errors=errors,
+                                            autocommit=False,
                                             logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
-            cursor.execute(exc_stmt, bind_vals)
+            cursor.execute(statement=exc_stmt,
+                           parameters=bind_vals)
             result = cursor.rowcount
-        # commit the transaction
-        curr_conn.commit()
+
+        # commit the transaction, if appropriate
+        if committable or not conn:
+            curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+                                 engine="oracle")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
         _db_log(logger=logger,
-                engine="sqlserver",
+                engine="oracle",
                 err_msg=err_msg,
                 errors=errors,
                 stmt=exc_stmt,
                 bind_vals=bind_vals)
 
     return result
 
 
+# TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
+# noinspection PyUnusedLocal
+def call_function(errors: list[str],
+                  func_name: str,
+                  func_vals: tuple,
+                  conn: Connection,
+                  committable: bool,
+                  logger: Logger) -> list[tuple]:
+    """
+    Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
+
+    :param errors: incidental error messages
+    :param func_name: name of the stored function
+    :param func_vals: parameters for the stored function
+    :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param logger: optional logger
+    :return: the data returned by the function
+    """
+    # initialize the return variable
+    result: list[tuple] = []
+
+    return result
+
+
+# TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
 def call_procedure(errors: list[str],
                    proc_name: str,
                    proc_vals: tuple,
                    conn: Connection,
-                   logger: Logger = None) -> list[tuple]:
+                   committable: bool,
+                   logger: Logger) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
     :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
-    result: list[tuple] | None = None
+    result: list[tuple] = []
 
     # make sure to have a connection
     curr_conn: Connection = conn or connect(errors=errors,
+                                            autocommit=False,
                                             logger=logger)
 
-    # build the command
-    proc_stmt: str | None = None
-
     # execute the stored procedure
     err_msg: str | None = None
     try:
-        # obtain a cursor and execute the operation
+        # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
-            proc_stmt = f"SET NOCOUNT ON; EXEC {proc_name} {','.join(('?',) * len(proc_vals))}"
-            cursor.execute(proc_stmt, proc_vals)
+            cursor.callproc(name=proc_name,
+                            parameters=proc_vals)
+
             # retrieve the returned tuples
-            rows: list[Row] = cursor.fetchall()
-            result = [tuple(row) for row in rows]
-        # commit the transaction
-        curr_conn.commit()
+            result = list(cursor)
+
+        # commit the transaction, if appropriate
+        if committable or not conn:
+            curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+                                 engine="oracle")
     finally:
         # close the connection, if locally acquired
         if curr_conn and not conn:
             curr_conn.close()
 
     # log eventual errors
     if errors or err_msg:
         _db_log(logger=logger,
-                engine="sqlserver",
+                engine="oracle",
                 err_msg=err_msg,
                 errors=errors,
-                stmt=proc_stmt,
+                stmt=proc_name,
                 bind_vals=proc_vals)
 
     return result
+
+__is_initialized: str | None = None
+
+def initialize(errors: list[str],
+               logger: Logger) -> bool:
+    """
+    Prepare the oracle engine to access the database throught the installed client software.
+
+    :param errors: incidental error messages
+    :param logger: optional logger
+    :return: False if an error happened, True otherwise
+    """
+    # initialize the return variable
+    result: bool = True
+
+    global __is_initialized
+    if not __is_initialized:
+        err_msg: str | None = None
+        client: str = _DB_CONN_DATA["oracle"]["client"]
+        try:
+            init_oracle_client(client)
+            __is_initialized = True
+        except Exception as e:
+            result = False
+            err_msg = _db_except_msg(exception=e,
+                                     engine="oracle")
+        # log the results
+        _db_log(logger=logger,
+                engine="oracle",
+                err_msg=err_msg,
+                errors=errors,
+                stmt="Initializing the client")
+
+    return result
```

### Comparing `pypomes_db-0.8.6/LICENSE` & `pypomes_db-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.6/pyproject.toml` & `pypomes_db-0.8.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.8.6"
+version = "0.8.7"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -20,15 +20,15 @@
 ]
 dependencies = [
     "pip>=24.0",
 #   "mysql-connector-python>=8.4.0",
 #   "oracledb>=2.2.0",
 #   "psycopg2-binary>=2.9.9",
 #   "pyodbc>=5.1.0",
-    "pypomes_core>=1.0.4",
+    "pypomes_core>=1.0.5",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-DB"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-DB/issues"
```

### Comparing `pypomes_db-0.8.6/PKG-INFO` & `pypomes_db-0.8.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.8.6
+Version: 0.8.7
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=1.0.4
+Requires-Dist: pypomes-core>=1.0.5
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```


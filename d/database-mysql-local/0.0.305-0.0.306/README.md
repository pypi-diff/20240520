# Comparing `tmp/database_mysql_local-0.0.305.tar.gz` & `tmp/database_mysql_local-0.0.306.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.305.tar", last modified: Sun May 19 04:23:32 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.306.tar", last modified: Sun May 19 17:17:00 2024, max compression
```

## Comparing `database_mysql_local-0.0.305.tar` & `database_mysql_local-0.0.306.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:23:32.472463 database_mysql_local-0.0.305/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-19 04:23:32.472463 database_mysql_local-0.0.305/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:23:32.464463 database_mysql_local-0.0.305/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:23:32.472463 database_mysql_local-0.0.305/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    51401 2024-05-19 04:23:02.000000 database_mysql_local-0.0.305/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30908 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-19 04:22:59.000000 database_mysql_local-0.0.305/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:23:32.472463 database_mysql_local-0.0.305/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-19 04:23:32.000000 database_mysql_local-0.0.305/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-19 04:23:32.000000 database_mysql_local-0.0.305/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 04:23:32.000000 database_mysql_local-0.0.305/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 04:23:32.000000 database_mysql_local-0.0.305/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 04:23:32.000000 database_mysql_local-0.0.305/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 04:23:32.472463 database_mysql_local-0.0.305/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:17:00.386645 database_mysql_local-0.0.306/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-19 17:17:00.386645 database_mysql_local-0.0.306/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:17:00.378645 database_mysql_local-0.0.306/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:17:00.382645 database_mysql_local-0.0.306/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51501 2024-05-19 17:16:21.000000 database_mysql_local-0.0.306/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30908 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-19 17:16:19.000000 database_mysql_local-0.0.306/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:17:00.382645 database_mysql_local-0.0.306/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-19 17:17:00.000000 database_mysql_local-0.0.306/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-19 17:17:00.000000 database_mysql_local-0.0.306/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:17:00.000000 database_mysql_local-0.0.306/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 17:17:00.000000 database_mysql_local-0.0.306/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 17:17:00.000000 database_mysql_local-0.0.306/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:17:00.386645 database_mysql_local-0.0.306/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-19 17:16:21.000000 database_mysql_local-0.0.306/setup.py
```

### Comparing `database_mysql_local-0.0.305/PKG-INFO` & `database_mysql_local-0.0.306/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.305
+Version: 0.0.306
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.305/README.md` & `database_mysql_local-0.0.306/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.305/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.306/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.305/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.306/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.305/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.306/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.305/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.306/database_mysql_local/src/generic_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from .table_definition import table_definition
 from .utils import (process_insert_data_dict, process_update_data_dict, get_where_params, where_skip_null_values,
                     validate_none_select_table_name, validate_single_clause_value,
                     validate_select_table_name, detect_if_is_test_data,
                     generate_view_name, generate_column_name, get_entity_type_by_table_name)
 
 
-# TODO: this file is too big, can we break it down into smaller files?
 class GenericCRUD(metaclass=MetaLogger, object=LOGGER_CRUD_CODE_OBJECT):
     """A class that provides generic CRUD functionality.
     There are 4 main functions to create, read, update, and delete data from the database.
     The rest of the functions are helper functions or wrappers around the main functions."""
 
     # TODO add default_select_clause_value and default_where in all functions not only in select_multi_tuple_by_where
     #   (no need to add to the the selects, as they all call select_multi_tuple_by_where)
@@ -62,15 +61,14 @@
         return column_name
 
     def insert(self, *, schema_name: str = None, table_name: str = None, data_dict: dict = None, data_json: dict = None,
                ignore_duplicate: bool = False, commit_changes: bool = True) -> int:
         """Inserts a new row into the table and returns the id of the new row or -1 if an error occurred."""
         data_dict = data_json or self._data_json_to_dict(data_dict)
         if ignore_duplicate:
-            # TODO Also display the data_dict
             self.logger.warning(f"GenericCRUD.insert({schema_name}.{table_name}) using ignore_duplicate, is it needed?",
                                 object={"data_dict": data_dict})
 
         table_name = table_name or self.default_table_name
         schema_name = schema_name or self.default_schema_name
         self._validate_args(args=locals())
 
@@ -124,16 +122,17 @@
 
     def insert_many(self, *, schema_name: str = None, table_name: str = None, data_dict: dict[str, list or tuple],
                     commit_changes: bool = True) -> None:
         """Inserts multiple rows into the table.
         data_dict should be in the following format: {col1: [val1, val2], col2: [val3, val4], ...}
         """
         if not data_dict:
-            self.logger.warning("GenericCRUD.insert_many: data_dict is empty")
-            return
+            error = "GenericCRUD.insert_many: data_dict is empty"
+            self.logger.error(error)
+            raise ValueError(error)
 
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
 
         self._validate_args(args=locals())
         # TODO: I am not sure we can use process_insert_data_dict here
 
@@ -461,16 +460,17 @@
             id_column_value=id_column_value, distinct=distinct, order_by=order_by, skip_null_values=skip_null_values)
 
     def select_one_value_by_column_and_value(
             self, *, select_clause_value: str, schema_name: str = None, view_table_name: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, order_by: str = "", skip_null_values: bool = True) -> Any:
         """Selects one value from the table by ID and returns it."""
-        column_name = column_name or id_column_name
+        column_name = self._deprecated_id_column(id_column_name, column_name)
         column_value = column_value or id_column_value
+        column_name = column_name or self.default_column_name
         select_clause_value = select_clause_value or self.default_select_clause_value
         validate_single_clause_value(select_clause_value)
         where, params = get_where_params(column_name, column_value)
         where = where_skip_null_values(where, select_clause_value, skip_null_values)
         result = self.select_one_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, order_by=order_by)
@@ -528,16 +528,17 @@
 
     def select_multi_value_by_column_and_value(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = "",
             skip_null_values: bool = True) -> list:
         """Selects multiple values from the table by ID and returns them as a list."""
-        column_name = column_name or id_column_name
+        column_name = self._deprecated_id_column(id_column_name, column_name)
         column_value = column_value or id_column_value
+        column_name = column_name or self.default_column_name
         select_clause_value = select_clause_value or self.default_select_clause_value
         validate_single_clause_value(select_clause_value)
         where, params = get_where_params(column_name, column_value)
         where = where_skip_null_values(where, select_clause_value, skip_null_values)
         result = self.select_multi_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
```

### Comparing `database_mysql_local-0.0.305/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.306/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.305/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.306/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.305/database_mysql_local/src/point.py` & `database_mysql_local-0.0.306/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.305/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.306/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.305/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.306/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.305/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.306/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.305/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.306/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.305/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.306/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.305/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.306/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.305
+Version: 0.0.306
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.305/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.306/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.305/pyproject.toml` & `database_mysql_local-0.0.306/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.305/setup.py` & `database_mysql_local-0.0.306/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 # TODO: we are migrating from database_mysql_local to database_mysql_local
 #  but in the meantime we want to keep both names
 old_name = "database_mysql_local"
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.305',
+    version='0.0.306',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir, old_name],
     package_dir={package_dir: f'{package_dir}/src', old_name: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```


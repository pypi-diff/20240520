# Comparing `tmp/database_mysql_local-0.0.306.tar.gz` & `tmp/database_mysql_local-0.0.307.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.306.tar", last modified: Sun May 19 17:17:00 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.307.tar", last modified: Mon May 20 08:39:00 2024, max compression
```

## Comparing `database_mysql_local-0.0.306.tar` & `database_mysql_local-0.0.307.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:17:00.386645 database_mysql_local-0.0.306/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-19 17:17:00.386645 database_mysql_local-0.0.306/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:17:00.378645 database_mysql_local-0.0.306/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:17:00.382645 database_mysql_local-0.0.306/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    51501 2024-05-19 17:16:21.000000 database_mysql_local-0.0.306/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30908 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-19 17:16:19.000000 database_mysql_local-0.0.306/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:17:00.382645 database_mysql_local-0.0.306/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-19 17:17:00.000000 database_mysql_local-0.0.306/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-19 17:17:00.000000 database_mysql_local-0.0.306/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:17:00.000000 database_mysql_local-0.0.306/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 17:17:00.000000 database_mysql_local-0.0.306/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 17:17:00.000000 database_mysql_local-0.0.306/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-19 17:15:47.000000 database_mysql_local-0.0.306/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:17:00.386645 database_mysql_local-0.0.306/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-19 17:16:21.000000 database_mysql_local-0.0.306/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:39:00.307808 database_mysql_local-0.0.307/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-20 08:39:00.307808 database_mysql_local-0.0.307/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:39:00.303808 database_mysql_local-0.0.307/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:39:00.307808 database_mysql_local-0.0.307/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51501 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31714 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-20 08:38:26.000000 database_mysql_local-0.0.307/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:39:00.307808 database_mysql_local-0.0.307/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-20 08:39:00.000000 database_mysql_local-0.0.307/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-20 08:39:00.000000 database_mysql_local-0.0.307/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 08:39:00.000000 database_mysql_local-0.0.307/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 08:39:00.000000 database_mysql_local-0.0.307/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 08:39:00.000000 database_mysql_local-0.0.307/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 08:39:00.307808 database_mysql_local-0.0.307/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/setup.py
```

### Comparing `database_mysql_local-0.0.306/PKG-INFO` & `database_mysql_local-0.0.307/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.306
+Version: 0.0.307
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.306/README.md` & `database_mysql_local-0.0.307/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.306/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.307/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.306/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.307/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.306/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.307/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.306/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.307/database_mysql_local/src/generic_crud.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.306/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.307/database_mysql_local/src/generic_crud_ml.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,31 +11,32 @@
 
 IS_MAIN_COLUMN_NAME = "is_main"
 
 
 class GenericCRUDML(GenericCRUD, metaclass=MetaLogger, object=LOGGER_CRUD_ML_CODE_OBJECT):
     """A class that provides generic CRUD functionality for tables with multi-language support."""
 
-    def __init__(self, default_schema_name: str, default_table_name: str = None,
-                 default_column_name: str = None, default_id_column_name: str = None,
+    def __init__(self, default_schema_name: str, default_table_name: str = None, default_view_table_name: str = None,
+                 default_ml_view_table_name: str = None, default_column_name: str = None, default_id_column_name: str = None,
                  is_main_column_name: str = IS_MAIN_COLUMN_NAME,
                  is_test_data: bool = False) -> None:
         """Initializes the GenericCRUDML class. If connection is not provided,
         a new connection will be created."""
         if default_table_name is not None:
             self.default_ml_table_name = self._create_ml_table_name(default_table_name)
-            self.default_view_table_name = self._get_ml_view_name(default_table_name)
+            default_view_table_name = default_view_table_name
+            self.default_ml_view_table_name = default_ml_view_table_name or self._get_ml_view_name(default_table_name)
         else:
             self.default_ml_table_name = None
-            self.default_view_table_name = None
+            default_view_table_name = None
         self.logger.info("GenericCRUDML.__init__", object={"default_ml_table_name": self.default_ml_table_name,
-                                                           "default_view_table_name": self.default_view_table_name})
+                                                           "default_view_table_name": default_view_table_name})
         GenericCRUD.__init__(self, default_schema_name=default_schema_name,
                              default_table_name=default_table_name,
-                             default_view_table_name=self.default_view_table_name,
+                             default_view_table_name=default_view_table_name,
                              default_column_name=default_column_name or default_id_column_name,
                              is_test_data=is_test_data)
         self.user_context = UserContext()
         # TODO: we may have to change it to a list when we will have multiple is_main columns
         self.is_main_column_name = is_main_column_name
 
     def sql_in_list_by_entity_list_id(self, schema_name: str, entity_name: str, entity_list_id: int) -> str:
@@ -204,14 +205,15 @@
                      is_main: int = 0, table_name: str = None,
                      ml_table_name: str = None, schema_name: str = None,
                      compare_view_name: str = None,
                      limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> tuple:
         # TODO: after we delete data_ml_json parameter, make data_ml_dict without default value and we can delete the following raise
         if not data_ml_dict and not data_ml_json:
             raise ValueError("data_ml_dict or data_ml_json is required for upsert_value")
+        compare_view_name = compare_view_name or self.default_ml_view_table_name
         data_dict = data_json or self._data_json_to_dict(data_dict)
         data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
         self.default_schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
         column_name = generate_column_name(table_name)
         ml_column_name = generate_column_name(ml_table_name)
@@ -248,14 +250,15 @@
                                         table_name: str = None,
                                         ml_table_name: str = None, schema_name: str = None,
                                         compare_view_name: str = None,
                                         limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> tuple:
         # TODO: after we delete data_ml_json parameter, make data_ml_dict without default value and we can delete the following raise
         if not data_ml_dict and not data_ml_json:
             raise ValueError("data_ml_dict or data_ml_json is required for upsert_value")
+        compare_view_name = compare_view_name or self.default_ml_view_table_name
         data_dict = data_json or self._data_json_to_dict(data_dict)
         data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
         self.default_schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
         column_name = generate_column_name(table_name)
         ml_column_name = generate_column_name(ml_table_name)
@@ -333,64 +336,69 @@
 
     def get_values_tuple(self, table_id: int, lang_code: LangCode = None,
                          column_name: str = None, id_column_name: str = None, select_clause_value: str = "*",
                          order_by: str = None) -> tuple:
         column_name = self._deprecated_id_column(id_column_name, column_name)
         lang_code_str = self._get_lang_code_str(lang_code=lang_code)
         column_name = column_name or generate_column_name(self.default_table_name)
-        result = self.select_one_tuple_by_where(where=f"{column_name}=%s AND lang_code=%s",
+        result = self.select_one_tuple_by_where(view_table_name=self.default_ml_view_table_name,
+                                                where=f"{column_name}=%s AND lang_code=%s",
                                                 params=(table_id, lang_code_str),
                                                 select_clause_value=select_clause_value,
                                                 order_by=order_by)
 
         return result
 
     def get_values_dict(self, table_id: int, lang_code: LangCode = None,
                         column_name: str = None, id_column_name: str = None, order_by: str = None) -> dict:
         column_name = self._deprecated_id_column(id_column_name, column_name)
         lang_code_str = self._get_lang_code_str(lang_code=lang_code)
         column_name = column_name or generate_column_name(
             self.default_table_name)
-        result = self.select_one_dict_by_where(where=f"{column_name}=%s AND lang_code=%s",
+        result = self.select_one_dict_by_where(view_table_name=self.default_ml_view_table_name,
+                                               where=f"{column_name}=%s AND lang_code=%s",
                                                params=(table_id, lang_code_str),
                                                order_by=order_by or f"{column_name} DESC")
 
         return result
 
     def get_values_dict_list(self, table_id: int, lang_code: LangCode = None,
                              column_name: str = None, id_column_name: str = None,
                              order_by: str = None) -> list:
         column_name = self._deprecated_id_column(id_column_name, column_name)
         lang_code_str = self._get_lang_code_str(lang_code=lang_code)
         column_name = column_name or generate_column_name(
             self.default_table_name)
-        result = self.select_multi_dict_by_where(where=f"{column_name}=%s AND lang_code=%s",
+        result = self.select_multi_dict_by_where(view_table_name=self.default_ml_view_table_name,
+                                                 where=f"{column_name}=%s AND lang_code=%s",
                                                  params=(table_id, lang_code_str),
                                                  order_by=order_by)
         return result
 
     def get_main_values_tuple(self, table_id: int, column_name: str = None, id_column_name: str = None,
                               select_clause_value: str = "*",
                               order_by: str = None) -> tuple:
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_name = column_name or generate_column_name(
             self.default_table_name)
-        result = self.select_one_tuple_by_where(where=f"{column_name}=%s AND is_main=1",
+        result = self.select_one_tuple_by_where(view_table_name=self.default_ml_view_table_name,
+                                                where=f"{column_name}=%s AND is_main=1",
                                                 params=(table_id,),
                                                 select_clause_value=select_clause_value,
                                                 order_by=order_by or f"{column_name} DESC")
 
         return result
 
     def get_main_values_dict(self, table_id: int, column_name: str = None, id_column_name: str = None,
                              select_clause_value: str = "*", order_by: str = None) -> dict:
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_name = column_name or generate_column_name(
             self.default_table_name)
-        result = self.select_one_dict_by_where(where=f"{column_name}=%s AND is_main=1",
+        result = self.select_one_dict_by_where(view_table_name=self.default_ml_view_table_name,
+                                               where=f"{column_name}=%s AND is_main=1",
                                                params=(table_id,),
                                                select_clause_value=select_clause_value,
                                                order_by=order_by)
 
         return result
 
     def get_id_by_name(self, name: str, table_name: str = None, ml_table_name: str = None, lang_code: LangCode = None,
@@ -455,15 +463,15 @@
                                                   order_by=order_by)
         return [row[0] for row in result]
 
     def delete_by_name(self, name: str,
                        lang_code: LangCode = None) -> None:
 
         lang_code_str = self._get_lang_code_str(lang_code=lang_code, name=name)
-        if GenericCRUD.is_column_in_table(self, table_name=self.default_view_table_name, column_name="title"):
+        if GenericCRUD.is_column_in_table(self, table_name=self.default_ml_view_table_name, column_name="title"):
             self.delete_by_where(table_name=self.default_ml_table_name, where="title=%s AND lang_code=%s",
                                  params=(name, lang_code_str))
         else:
             self.delete_by_where(table_name=self.default_ml_table_name, where="`name`=%s AND lang_code=%s",
                                  params=(name, lang_code_str))
 
     @staticmethod
```

### Comparing `database_mysql_local-0.0.306/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.307/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.306/database_mysql_local/src/point.py` & `database_mysql_local-0.0.307/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.306/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.307/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.306/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.307/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.306/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.307/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.306/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.307/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.306/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.307/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.306/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.307/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.306
+Version: 0.0.307
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.306/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.307/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.306/pyproject.toml` & `database_mysql_local-0.0.307/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "database-mysql-local"
-version = "0.0.302" # https://pypi.org/project/database-mysql-local
+version = "0.0.307" # https://pypi.org/project/database-mysql-local
 description = "database-mysql-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
 
 # dephell deps convert --from pyproject.toml --from-format poetry --to setup.py --to-format setuppy
```

### Comparing `database_mysql_local-0.0.306/setup.py` & `database_mysql_local-0.0.307/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 # TODO: we are migrating from database_mysql_local to database_mysql_local
 #  but in the meantime we want to keep both names
 old_name = "database_mysql_local"
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.306',
+    version='0.0.307',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir, old_name],
     package_dir={package_dir: f'{package_dir}/src', old_name: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```


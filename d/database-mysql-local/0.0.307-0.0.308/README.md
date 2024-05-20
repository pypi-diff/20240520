# Comparing `tmp/database_mysql_local-0.0.307.tar.gz` & `tmp/database_mysql_local-0.0.308.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.307.tar", last modified: Mon May 20 08:39:00 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.308.tar", last modified: Mon May 20 11:16:53 2024, max compression
```

## Comparing `database_mysql_local-0.0.307.tar` & `database_mysql_local-0.0.308.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:39:00.307808 database_mysql_local-0.0.307/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-20 08:39:00.307808 database_mysql_local-0.0.307/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:39:00.303808 database_mysql_local-0.0.307/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:39:00.307808 database_mysql_local-0.0.307/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    51501 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    31714 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-20 08:38:26.000000 database_mysql_local-0.0.307/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:39:00.307808 database_mysql_local-0.0.307/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-20 08:39:00.000000 database_mysql_local-0.0.307/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-20 08:39:00.000000 database_mysql_local-0.0.307/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 08:39:00.000000 database_mysql_local-0.0.307/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 08:39:00.000000 database_mysql_local-0.0.307/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 08:39:00.000000 database_mysql_local-0.0.307/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 08:39:00.307808 database_mysql_local-0.0.307/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-20 08:38:01.000000 database_mysql_local-0.0.307/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:16:53.489167 database_mysql_local-0.0.308/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-20 11:16:53.489167 database_mysql_local-0.0.308/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:16:53.481167 database_mysql_local-0.0.308/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:16:53.485167 database_mysql_local-0.0.308/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51501 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31830 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-20 11:16:18.000000 database_mysql_local-0.0.308/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:16:53.489167 database_mysql_local-0.0.308/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-20 11:16:53.000000 database_mysql_local-0.0.308/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-20 11:16:53.000000 database_mysql_local-0.0.308/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:16:53.000000 database_mysql_local-0.0.308/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 11:16:53.000000 database_mysql_local-0.0.308/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 11:16:53.000000 database_mysql_local-0.0.308/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 11:16:53.489167 database_mysql_local-0.0.308/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-20 11:15:50.000000 database_mysql_local-0.0.308/setup.py
```

### Comparing `database_mysql_local-0.0.307/PKG-INFO` & `database_mysql_local-0.0.308/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.307
+Version: 0.0.308
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.307/README.md` & `database_mysql_local-0.0.308/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.307/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.308/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.307/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.308/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.307/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.308/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.307/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.308/database_mysql_local/src/generic_crud.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.307/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.308/database_mysql_local/src/generic_crud_ml.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,18 +72,20 @@
         old_cursor = self.cursor
         cursor = None
         try:
             cursor = self.connection.cursor()
             self.cursor = cursor
 
             # if this is the first insert of this data, is_main should be 1
-            if table_id is None:
-                is_main = 1
-            elif is_main == 1:
-                self._update_old_main_value_to_zero(table_id, table_name)
+            if is_main is not None:
+                if table_id is None:
+                    is_main = 1
+                elif is_main == 1:
+                    self._update_old_main_value_to_zero(table_id, table_name)
+                data_ml_dict[self.is_main_column_name] = is_main
 
             # id is the id value of the row in the table_name table
             table_id = table_id or self.insert(data_dict=data_dict, ignore_duplicate=True,
                                                table_name=table_name, commit_changes=False)
             if table_id is None:  # TODO: delete
                 self.logger.error("Error inserting data_dict", object={"data_dict": data_dict})
                 self.connection.rollback()
@@ -92,15 +94,14 @@
             if data_ml_dict is None or data_ml_dict == {}:
                 self.connection.commit()
                 return table_id, None
 
             column_name = re.sub(r'(_table)$', '_id', table_name)
             data_ml_dict[column_name] = table_id
             data_ml_dict["lang_code"] = lang_code_str
-            data_ml_dict[self.is_main_column_name] = is_main
 
             # ml_id is the id value of the row in the ml_table_name table
             ml_table_id = self.insert(data_dict=data_ml_dict, table_name=ml_table_name, ignore_duplicate=True,
                                       commit_changes=False)
 
             self.connection.commit()
         except Exception as e:
@@ -170,23 +171,24 @@
 
         old_cursor = self.cursor
         cursor = None
         try:
             cursor = self.connection.cursor()
             self.cursor = cursor
 
-            if is_main == 1:
-                self._update_old_main_value_to_zero(table_id, table_name)
-            if data_dict:
-                self.update_by_id(data_dict=data_dict, table_name=table_name, column_name=column_name,
-                                  id_column_value=table_id, limit=limit, order_by=order_by, commit_changes=False)
+            if is_main is not None:
+                if is_main == 1:
+                    self._update_old_main_value_to_zero(table_id, table_name)
+                if data_dict:
+                    self.update_by_id(data_dict=data_dict, table_name=table_name, column_name=column_name,
+                                      id_column_value=table_id, limit=limit, order_by=order_by, commit_changes=False)
+                data_ml_dict[self.is_main_column_name] = is_main
 
             data_ml_dict[column_name] = table_id
             data_ml_dict["lang_code"] = lang_code_str
-            data_ml_dict[self.is_main_column_name] = is_main
             column_name = generate_column_name(ml_table_name)
 
             self.update_by_id(data_dict=data_ml_dict, table_name=ml_table_name, column_name=column_name,
                               id_column_value=ml_table_id, limit=limit, order_by=order_by, commit_changes=False)
 
             self.connection.commit()
         except Exception as e:
```

### Comparing `database_mysql_local-0.0.307/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.308/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.307/database_mysql_local/src/point.py` & `database_mysql_local-0.0.308/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.307/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.308/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.307/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.308/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.307/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.308/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.307/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.308/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.307/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.308/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.307/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.308/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.307
+Version: 0.0.308
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.307/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.308/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.307/pyproject.toml` & `database_mysql_local-0.0.308/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "database-mysql-local"
-version = "0.0.307" # https://pypi.org/project/database-mysql-local
+version = "0.0.308" # https://pypi.org/project/database-mysql-local
 description = "database-mysql-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
 
 # dephell deps convert --from pyproject.toml --from-format poetry --to setup.py --to-format setuppy
```

### Comparing `database_mysql_local-0.0.307/setup.py` & `database_mysql_local-0.0.308/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 # TODO: we are migrating from database_mysql_local to database_mysql_local
 #  but in the meantime we want to keep both names
 old_name = "database_mysql_local"
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.307',
+    version='0.0.308',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir, old_name],
     package_dir={package_dir: f'{package_dir}/src', old_name: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```


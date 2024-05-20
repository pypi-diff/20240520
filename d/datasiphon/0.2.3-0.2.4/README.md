# Comparing `tmp/datasiphon-0.2.3.tar.gz` & `tmp/datasiphon-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasiphon-0.2.3.tar", last modified: Tue May  7 09:12:53 2024, max compression
+gzip compressed data, was "datasiphon-0.2.4.tar", last modified: Mon May 20 10:07:02 2024, max compression
```

## Comparing `datasiphon-0.2.3.tar` & `datasiphon-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-07 09:12:53.441638 datasiphon-0.2.3/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-07 09:12:53.441638 datasiphon-0.2.3/PKG-INFO
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5119 2024-03-04 08:16:45.000000 datasiphon-0.2.3/README.md
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     1318 2024-01-29 12:20:19.000000 datasiphon-0.2.3/pyproject.toml
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)       38 2024-05-07 09:12:53.441638 datasiphon-0.2.3/setup.cfg
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-07 09:12:53.439638 datasiphon-0.2.3/src/
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-07 09:12:53.441638 datasiphon-0.2.3/src/datasiphon.egg-info/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-07 09:12:53.000000 datasiphon-0.2.3/src/datasiphon.egg-info/PKG-INFO
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)      311 2024-05-07 09:12:53.000000 datasiphon-0.2.3/src/datasiphon.egg-info/SOURCES.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)        1 2024-05-07 09:12:53.000000 datasiphon-0.2.3/src/datasiphon.egg-info/dependency_links.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)       33 2024-05-07 09:12:53.000000 datasiphon-0.2.3/src/datasiphon.egg-info/requires.txt
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)        7 2024-05-07 09:12:53.000000 datasiphon-0.2.3/src/datasiphon.egg-info/top_level.txt
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-07 09:12:53.440638 datasiphon-0.2.3/src/siphon/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)      211 2024-05-07 09:10:52.000000 datasiphon-0.2.3/src/siphon/__init__.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     1127 2024-05-07 09:10:36.000000 datasiphon-0.2.3/src/siphon/base.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)     4314 2024-05-07 09:10:38.000000 datasiphon-0.2.3/src/siphon/nosql.py
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)    22292 2024-05-07 09:10:59.000000 datasiphon-0.2.3/src/siphon/sql.py
-drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-07 09:12:53.441638 datasiphon-0.2.3/tests/
--rw-r--r--   0 nemeth    (1000) nemeth    (1000)    16693 2024-05-07 09:11:07.000000 datasiphon-0.2.3/tests/test_sql.py
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-20 10:07:02.612306 datasiphon-0.2.4/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-20 10:07:02.612306 datasiphon-0.2.4/PKG-INFO
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5119 2024-03-04 08:16:45.000000 datasiphon-0.2.4/README.md
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     1318 2024-01-29 12:20:19.000000 datasiphon-0.2.4/pyproject.toml
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)       38 2024-05-20 10:07:02.612306 datasiphon-0.2.4/setup.cfg
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-20 10:07:02.611307 datasiphon-0.2.4/src/
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-20 10:07:02.612306 datasiphon-0.2.4/src/datasiphon.egg-info/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     5958 2024-05-20 10:07:02.000000 datasiphon-0.2.4/src/datasiphon.egg-info/PKG-INFO
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)      311 2024-05-20 10:07:02.000000 datasiphon-0.2.4/src/datasiphon.egg-info/SOURCES.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)        1 2024-05-20 10:07:02.000000 datasiphon-0.2.4/src/datasiphon.egg-info/dependency_links.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)       33 2024-05-20 10:07:02.000000 datasiphon-0.2.4/src/datasiphon.egg-info/requires.txt
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)        7 2024-05-20 10:07:02.000000 datasiphon-0.2.4/src/datasiphon.egg-info/top_level.txt
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-20 10:07:02.612306 datasiphon-0.2.4/src/siphon/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)      211 2024-05-20 10:06:35.000000 datasiphon-0.2.4/src/siphon/__init__.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     1127 2024-05-07 09:15:29.000000 datasiphon-0.2.4/src/siphon/base.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)     4314 2024-05-07 09:15:29.000000 datasiphon-0.2.4/src/siphon/nosql.py
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)    24289 2024-05-20 09:58:29.000000 datasiphon-0.2.4/src/siphon/sql.py
+drwxr-xr-x   0 nemeth    (1000) nemeth    (1000)        0 2024-05-20 10:07:02.612306 datasiphon-0.2.4/tests/
+-rw-r--r--   0 nemeth    (1000) nemeth    (1000)    21235 2024-05-20 10:04:47.000000 datasiphon-0.2.4/tests/test_sql.py
```

### Comparing `datasiphon-0.2.3/PKG-INFO` & `datasiphon-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasiphon
-Version: 0.2.3
+Version: 0.2.4
 Summary: Dynamic building of filtered database queries
 Author-email: Marek Nemeth <99m.nemeth@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Nemulo/libs-datasiphon
 Project-URL: Bug Tracker, https://github.com/Nemulo/libs-datasiphon/issues
 Project-URL: Documentation, https://github.com/Nemulo/libs-datasiphon/blob/main/README.md
 Keywords: database,sql,filtering,query
```

### Comparing `datasiphon-0.2.3/README.md` & `datasiphon-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.3/pyproject.toml` & `datasiphon-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.3/src/datasiphon.egg-info/PKG-INFO` & `datasiphon-0.2.4/src/datasiphon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasiphon
-Version: 0.2.3
+Version: 0.2.4
 Summary: Dynamic building of filtered database queries
 Author-email: Marek Nemeth <99m.nemeth@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Nemulo/libs-datasiphon
 Project-URL: Bug Tracker, https://github.com/Nemulo/libs-datasiphon/issues
 Project-URL: Documentation, https://github.com/Nemulo/libs-datasiphon/blob/main/README.md
 Keywords: database,sql,filtering,query
```

### Comparing `datasiphon-0.2.3/src/siphon/base.py` & `datasiphon-0.2.4/src/siphon/base.py`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.3/src/siphon/nosql.py` & `datasiphon-0.2.4/src/siphon/nosql.py`

 * *Files identical despite different names*

### Comparing `datasiphon-0.2.3/src/siphon/sql.py` & `datasiphon-0.2.4/src/siphon/sql.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,16 @@
     FilterFormatError,
     FilterColumnError,
     InvalidOperatorError,
     InvalidValueError,
     InvalidRestrictionModel,
     SiphonError,
 )
+import sqlalchemy.sql.elements as sql_elements
+import sqlalchemy.sql.operators as sql_operators
 import sqlalchemy as sa
 import typing as t
 from pydantic import BaseModel, model_validator, ValidationError
 from pydantic.fields import FieldInfo
 import re
 from copy import copy
 from sqlalchemy.sql.base import ReadOnlyColumnCollection
@@ -417,14 +419,56 @@
         filter_data = FilterBuilder.construct_clause(qs_filter, column_collection)
         query = query.where(*filter_data)
         keyword_data = FilterBuilder.extract_keywords(qs_filter)
         query = keyword_data.apply_on_query(query)
         return query
 
     @staticmethod
+    def is_query_paginable(query: sa.Select, pagination_columns: list[str]) -> bool:
+        """
+        Check if a query is paginable
+
+        :param query: The query to check
+
+        :return: Whether the query is paginable
+        """
+
+        def get_column_from_binary_expression(binary_expression: sql_elements.BinaryExpression) -> str:
+            if isinstance(binary_expression.left, sa.Column):
+                return binary_expression.left.name
+            elif isinstance(binary_expression.right, sa.Column):
+                return binary_expression.right.name
+            else:
+                return None
+
+        if query.whereclause is None:
+            return True
+        if isinstance(query.whereclause, sql_elements.BinaryExpression):
+            column = get_column_from_binary_expression(query.whereclause)
+            if column in pagination_columns and query.whereclause.operator in [sql_operators.eq, sql_operators.ne]:
+                return False
+        elif isinstance(query.whereclause, sql_elements.BooleanClauseList):
+            for clause in query.whereclause.clauses:
+                if isinstance(clause, sql_elements.BinaryExpression):
+                    column = get_column_from_binary_expression(clause)
+                    if column in pagination_columns and clause.operator in [sql_operators.eq, sql_operators.ne]:
+                        return False
+                    if query.whereclause.operator == sql_operators.and_:
+                        if column not in pagination_columns and clause.operator not in [
+                            sql_operators.eq,
+                            sql_operators.ne,
+                        ]:
+                            return False
+                else:
+                    return False
+        else:
+            raise TypeError(f"Unrecognized type: {type(query.whereclause)}")
+        return True
+
+    @staticmethod
     def eq(column: sa.Column, value: t.Any) -> sa.ColumnElement:
         process_type_func = FilterTypeParser.parse_type(column.type.python_type)
         return column == process_type_func(value)
 
     @staticmethod
     def ne(column: sa.Column, value: t.Any) -> sa.ColumnElement:
         process_type_func = FilterTypeParser.parse_type(column.type.python_type)
```

### Comparing `datasiphon-0.2.3/tests/test_sql.py` & `datasiphon-0.2.4/tests/test_sql.py`

 * *Files 18% similar despite different names*

```diff
@@ -442,10 +442,134 @@
 
         # test valid time stamp
         self.assertEqual(
             str(ds.sql.SQL.build(data.timestamp_table_select, {"created_at": {"eq": "2021-01-01T12:00:00"}})),
             str(data.timestamp_table_select.where(data.table_with_time_stamp.c.created_at == "2021-01-01T12:00:00")),
         )
 
+    def test_pointer_paginable_items(self):
+        import src.siphon as ds
+        from sqlalchemy.sql import operators
+
+        test_query = (
+            data.table_with_time_stamp.select()
+            .where(
+                sa.and_(
+                    data.table_with_time_stamp.c.created_at >= "2021-01-01T12:00:00",
+                    sa.or_(
+                        data.table_with_time_stamp.c.name == "John",
+                        data.table_with_time_stamp.c.name == "Alex",
+                    ),
+                )
+            )
+            .order_by(data.table_with_time_stamp.c.created_at.desc())
+        )
+        second_test_query = data.table_with_time_stamp.select()
+
+        # nested clauses for pointer will not be paginable
+        self.assertFalse(ds.sql.SQL.is_query_paginable(test_query, ["created_at"]))
+
+        # simple query will be paginable
+        self.assertTrue(ds.sql.SQL.is_query_paginable(second_test_query, ["created_at"]))
+
+        # if operator is eq or ne, it will not be paginable
+        self.assertFalse(
+            ds.sql.SQL.is_query_paginable(
+                second_test_query.where(data.table_with_time_stamp.c.name == "John"), ["name"]
+            )
+        )
+        self.assertFalse(
+            ds.sql.SQL.is_query_paginable(
+                second_test_query.where(data.table_with_time_stamp.c.name != "John"), ["name"]
+            )
+        )
+
+        # if operator is one of gt, ge etc.., it will be paginable
+        self.assertTrue(
+            ds.sql.SQL.is_query_paginable(
+                second_test_query.where(data.table_with_time_stamp.c.name >= "John"), ["name"]
+            )
+        )
+        self.assertTrue(
+            ds.sql.SQL.is_query_paginable(second_test_query.where(data.table_with_time_stamp.c.name < "John"), ["name"])
+        )
+
+        # on single grouping, allow paginable - paginated clauses must not have eq or ne
+        # if grouping with and_ : all other where clauses except the paginated ones should be eq or ne
+        self.assertTrue(
+            ds.sql.SQL.is_query_paginable(
+                second_test_query.where(
+                    sa.or_(
+                        data.table_with_time_stamp.c.name >= "John",
+                        data.table_with_time_stamp.c.created_at == "2024-04-05",
+                    )
+                ),
+                ["name"],
+            )
+        )
+        self.assertFalse(
+            ds.sql.SQL.is_query_paginable(
+                second_test_query.where(
+                    sa.or_(
+                        data.table_with_time_stamp.c.name == "John",
+                        data.table_with_time_stamp.c.created_at == "2024-04-05",
+                    )
+                ),
+                ["name"],
+            )
+        )
+
+        # test and junction
+        self.assertTrue(
+            ds.sql.SQL.is_query_paginable(
+                second_test_query.where(
+                    sa.and_(
+                        data.table_with_time_stamp.c.name >= "John",
+                        data.table_with_time_stamp.c.created_at == "2024-04-05",
+                    )
+                ),
+                ["name"],
+            )
+        )
+        self.assertFalse(
+            ds.sql.SQL.is_query_paginable(
+                second_test_query.where(
+                    sa.and_(
+                        data.table_with_time_stamp.c.name >= "John",
+                        data.table_with_time_stamp.c.created_at >= "2024-04-05",
+                    )
+                ),
+                ["name"],
+            )
+        )
+
+        # test multiple order by columns
+        self.assertTrue(ds.sql.SQL.is_query_paginable(second_test_query, ["name", "created_at"]))
+
+        # test multiple order by columns with filtered query
+        self.assertTrue(
+            ds.sql.SQL.is_query_paginable(
+                second_test_query.where(
+                    sa.and_(
+                        data.table_with_time_stamp.c.name >= "John",
+                        data.table_with_time_stamp.c.created_at >= "2024-04-05",
+                    )
+                ),
+                ["name", "created_at"],
+            )
+        )
+
+        self.assertFalse(
+            ds.sql.SQL.is_query_paginable(
+                second_test_query.where(
+                    sa.and_(
+                        data.table_with_time_stamp.c.name >= "John",
+                        data.table_with_time_stamp.c.created_at == "2024-04-05",
+                    )
+                ),
+                ["name", "created_at"],
+            )
+        )
+
 
 if __name__ == "__main__":
     unittest.main()
```


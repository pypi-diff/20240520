# Comparing `tmp/ja_basedb-0.0.14.tar.gz` & `tmp/ja_basedb-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ja_basedb-0.0.14.tar", last modified: Sun Jan  7 02:44:02 2024, max compression
+gzip compressed data, was "ja_basedb-0.0.15.tar", last modified: Mon May 20 14:44:53 2024, max compression
```

## Comparing `ja_basedb-0.0.14.tar` & `ja_basedb-0.0.15.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2024-01-07 02:44:02.779787 ja_basedb-0.0.14/
--rw-r--r--   0 areeda     (501) staff       (20)      659 2023-12-18 00:06:26.000000 ja_basedb-0.0.14/.gitignore
--rw-r--r--   0 areeda     (501) staff       (20)    35147 2023-01-24 03:02:43.000000 ja_basedb-0.0.14/LICENSE.txt
--rw-r--r--   0 areeda     (501) staff       (20)     1139 2024-01-07 02:44:02.779637 ja_basedb-0.0.14/PKG-INFO
--rw-r--r--   0 areeda     (501) staff       (20)        0 2023-01-24 03:02:43.000000 ja_basedb-0.0.14/README.md
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2024-01-07 02:44:02.771395 ja_basedb-0.0.14/UnitTests/
--rw-r--r--   0 areeda     (501) staff       (20)      120 2023-01-24 03:02:43.000000 ja_basedb-0.0.14/UnitTests/pytest.ini
--rw-r--r--   0 areeda     (501) staff       (20)     1464 2023-12-17 02:56:46.000000 ja_basedb-0.0.14/UnitTests/test_column.py
--rw-r--r--   0 areeda     (501) staff       (20)     1597 2023-12-17 02:56:46.000000 ja_basedb-0.0.14/UnitTests/test_database.py
--rw-r--r--   0 areeda     (501) staff       (20)     1966 2024-01-07 02:18:50.000000 ja_basedb-0.0.14/UnitTests/test_table.py
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2024-01-07 02:44:02.775615 ja_basedb-0.0.14/basedb/
--rw-r--r--   0 areeda     (501) staff       (20)      916 2023-12-17 23:43:55.000000 ja_basedb-0.0.14/basedb/__init__.py
--rw-r--r--   0 areeda     (501) staff       (20)      413 2024-01-07 02:44:02.000000 ja_basedb-0.0.14/basedb/_version.py
--rw-r--r--   0 areeda     (501) staff       (20)     7203 2023-12-17 23:28:36.000000 ja_basedb-0.0.14/basedb/column.py
--rw-r--r--   0 areeda     (501) staff       (20)     4849 2023-12-17 23:28:36.000000 ja_basedb-0.0.14/basedb/database.py
--rw-r--r--   0 areeda     (501) staff       (20)     9306 2023-12-17 23:28:36.000000 ja_basedb-0.0.14/basedb/row.py
--rw-r--r--   0 areeda     (501) staff       (20)     7920 2024-01-07 02:07:51.000000 ja_basedb-0.0.14/basedb/table.py
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2024-01-07 02:44:02.778923 ja_basedb-0.0.14/ja_basedb.egg-info/
--rw-r--r--   0 areeda     (501) staff       (20)     1139 2024-01-07 02:44:02.000000 ja_basedb-0.0.14/ja_basedb.egg-info/PKG-INFO
--rw-r--r--   0 areeda     (501) staff       (20)      439 2024-01-07 02:44:02.000000 ja_basedb-0.0.14/ja_basedb.egg-info/SOURCES.txt
--rw-r--r--   0 areeda     (501) staff       (20)        1 2024-01-07 02:44:02.000000 ja_basedb-0.0.14/ja_basedb.egg-info/dependency_links.txt
--rw-r--r--   0 areeda     (501) staff       (20)        6 2024-01-07 02:44:02.000000 ja_basedb-0.0.14/ja_basedb.egg-info/requires.txt
--rw-r--r--   0 areeda     (501) staff       (20)        7 2024-01-07 02:44:02.000000 ja_basedb-0.0.14/ja_basedb.egg-info/top_level.txt
--rw-r--r--   0 areeda     (501) staff       (20)     1428 2023-12-17 23:22:28.000000 ja_basedb-0.0.14/pyproject.toml
--rw-r--r--   0 areeda     (501) staff       (20)        0 2023-02-02 03:57:04.000000 ja_basedb-0.0.14/requirements.txt
--rw-r--r--   0 areeda     (501) staff       (20)      405 2024-01-07 02:44:02.780616 ja_basedb-0.0.14/setup.cfg
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2024-05-20 14:44:53.190054 ja_basedb-0.0.15/
+-rw-r--r--   0 areeda     (501) staff       (20)      659 2023-12-18 00:06:26.000000 ja_basedb-0.0.15/.gitignore
+-rw-r--r--   0 areeda     (501) staff       (20)    35147 2023-01-24 03:02:43.000000 ja_basedb-0.0.15/LICENSE.txt
+-rw-r--r--   0 areeda     (501) staff       (20)     1139 2024-05-20 14:44:53.189898 ja_basedb-0.0.15/PKG-INFO
+-rw-r--r--   0 areeda     (501) staff       (20)        0 2023-01-24 03:02:43.000000 ja_basedb-0.0.15/README.md
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2024-05-20 14:44:53.182763 ja_basedb-0.0.15/UnitTests/
+-rw-r--r--   0 areeda     (501) staff       (20)      120 2023-01-24 03:02:43.000000 ja_basedb-0.0.15/UnitTests/pytest.ini
+-rw-r--r--   0 areeda     (501) staff       (20)     1464 2023-12-17 02:56:46.000000 ja_basedb-0.0.15/UnitTests/test_column.py
+-rw-r--r--   0 areeda     (501) staff       (20)     1597 2023-12-17 02:56:46.000000 ja_basedb-0.0.15/UnitTests/test_database.py
+-rw-r--r--   0 areeda     (501) staff       (20)     1966 2024-01-07 02:18:50.000000 ja_basedb-0.0.15/UnitTests/test_table.py
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2024-05-20 14:44:53.186594 ja_basedb-0.0.15/basedb/
+-rw-r--r--   0 areeda     (501) staff       (20)      916 2023-12-17 23:43:55.000000 ja_basedb-0.0.15/basedb/__init__.py
+-rw-r--r--   0 areeda     (501) staff       (20)      413 2024-05-20 14:44:52.000000 ja_basedb-0.0.15/basedb/_version.py
+-rw-r--r--   0 areeda     (501) staff       (20)     7203 2023-12-17 23:28:36.000000 ja_basedb-0.0.15/basedb/column.py
+-rw-r--r--   0 areeda     (501) staff       (20)     4896 2024-01-09 05:22:38.000000 ja_basedb-0.0.15/basedb/database.py
+-rw-r--r--   0 areeda     (501) staff       (20)     9306 2023-12-17 23:28:36.000000 ja_basedb-0.0.15/basedb/row.py
+-rw-r--r--   0 areeda     (501) staff       (20)     7913 2024-05-17 20:19:29.000000 ja_basedb-0.0.15/basedb/table.py
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2024-05-20 14:44:53.189203 ja_basedb-0.0.15/ja_basedb.egg-info/
+-rw-r--r--   0 areeda     (501) staff       (20)     1139 2024-05-20 14:44:53.000000 ja_basedb-0.0.15/ja_basedb.egg-info/PKG-INFO
+-rw-r--r--   0 areeda     (501) staff       (20)      439 2024-05-20 14:44:53.000000 ja_basedb-0.0.15/ja_basedb.egg-info/SOURCES.txt
+-rw-r--r--   0 areeda     (501) staff       (20)        1 2024-05-20 14:44:53.000000 ja_basedb-0.0.15/ja_basedb.egg-info/dependency_links.txt
+-rw-r--r--   0 areeda     (501) staff       (20)        6 2024-05-20 14:44:53.000000 ja_basedb-0.0.15/ja_basedb.egg-info/requires.txt
+-rw-r--r--   0 areeda     (501) staff       (20)        7 2024-05-20 14:44:53.000000 ja_basedb-0.0.15/ja_basedb.egg-info/top_level.txt
+-rw-r--r--   0 areeda     (501) staff       (20)     1428 2023-12-17 23:22:28.000000 ja_basedb-0.0.15/pyproject.toml
+-rw-r--r--   0 areeda     (501) staff       (20)        0 2023-02-02 03:57:04.000000 ja_basedb-0.0.15/requirements.txt
+-rw-r--r--   0 areeda     (501) staff       (20)      405 2024-05-20 14:44:53.190985 ja_basedb-0.0.15/setup.cfg
```

### Comparing `ja_basedb-0.0.14/.gitignore` & `ja_basedb-0.0.15/.gitignore`

 * *Files identical despite different names*

### Comparing `ja_basedb-0.0.14/LICENSE.txt` & `ja_basedb-0.0.15/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ja_basedb-0.0.14/PKG-INFO` & `ja_basedb-0.0.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ja_basedb
-Version: 0.0.14
+Version: 0.0.15
 Summary: Classes wrapping database functions
 Author-email: Joseph Areeda <joe@areeda.com>
 Maintainer-email: Joseph Areeda <joe@areeda.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ja_basedb-0.0.14/UnitTests/test_column.py` & `ja_basedb-0.0.15/UnitTests/test_column.py`

 * *Files identical despite different names*

### Comparing `ja_basedb-0.0.14/UnitTests/test_database.py` & `ja_basedb-0.0.15/UnitTests/test_database.py`

 * *Files identical despite different names*

### Comparing `ja_basedb-0.0.14/UnitTests/test_table.py` & `ja_basedb-0.0.15/UnitTests/test_table.py`

 * *Files identical despite different names*

### Comparing `ja_basedb-0.0.14/basedb/__init__.py` & `ja_basedb-0.0.15/basedb/__init__.py`

 * *Files identical despite different names*

### Comparing `ja_basedb-0.0.14/basedb/column.py` & `ja_basedb-0.0.15/basedb/column.py`

 * *Files identical despite different names*

### Comparing `ja_basedb-0.0.14/basedb/database.py` & `ja_basedb-0.0.15/basedb/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 """Class wrapping a maridb connection"""
-
+import re
 import time
 import logging
 
 import mysql.connector
 
 
 __author__ = 'joseph areeda'
@@ -104,14 +104,17 @@
         """Execute a sql statement that does not return a result set"""
         cursor = self.connection.cursor()
         cursor.execute(sql)
         if commit:
             self.connection.commit()
         cursor.close()
 
+    def get_cursor(self):
+        return self.connection.cursor()
+
     def commit(self):
         self.connection.commit()
 
     def execute_query(self, sql):
         """Execute a sql query returning a cursor object.
         Don't forget to close it when finished."""
         cursor = self.connection.cursor()
@@ -129,15 +132,15 @@
 
     def escape_str(self, instr):
         """
         Escape any special chars like single, double quotes
         :param instr: input string
         :return: escaped string as utf-8 string
         """
-        ret = self.connection.escape_string(instr).decode()
+        ret = re.escape(instr)
         return ret
 
     def __del__(self):
         """ Make sure connection is closed when an object goes out of scope"""
         self.close()
 
     def cursor2list(self, cursor, columns):
```

### Comparing `ja_basedb-0.0.14/basedb/row.py` & `ja_basedb-0.0.15/basedb/row.py`

 * *Files identical despite different names*

### Comparing `ja_basedb-0.0.14/basedb/table.py` & `ja_basedb-0.0.15/basedb/table.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,39 +111,42 @@
 
     def insert(self, rows, commit=True):
         """
         Insert one or more rows into this table.
         Note all rows should have same keys in data dict as only keys in first
         row will be written
         :param rows: a single row or list of rows
+        param
         :return: None
         """
         if isinstance(rows, list) and len(rows) > 0:
             # bulk insert
             prefix = 'INSERT INTO {} '.format(self.name)
             col_names = list(rows[0].data.keys())
             prefix += ' ({}) VALUES \n'.format(', '.join(col_names))
             vals = ''
+            nrows = len(rows)
+            if nrows > 1:
+                # batch insert
+                self.db.execute(f'ALTER TABLE {self.name} DISABLE KEYS;')
             for row in rows:
                 if vals:
                     vals += ',\n'
                 v = row.get_insert_vals(col_names, self.db)
                 vals += '({})'.format(v)
-                if len(vals) > 500000:
-                    stmt = 'ALTER TABLE {} DISABLE KEYS;\n{} {}; \n' \
-                           'ALTER TABLE {} ENABLE KEYS;'.\
-                        format(self.name, prefix, vals, self.name)
-                    self.db.execute(stmt)
+                if len(vals) > 20000:
+                    stmt = f'{prefix} {vals}'
+                    self.db.execute(stmt, commit=commit)
                     vals = ''
 
             if len(vals) > 0:
-                stmt = 'ALTER TABLE {} DISABLE KEYS;\n{} {}; \n' \
-                       'ALTER TABLE {} ENABLE KEYS;'. \
-                    format(self.name, prefix, vals, self.name)
+                stmt = f'{prefix} {vals}'
                 self.db.execute(stmt, commit=commit)
+            if nrows > 1:
+                self.db.execute(f'ALTER TABLE {self.name} ENABLE KEYS;')
         else:
             stmt = 'INSERT INTO {} '.format(self.name)
             col_names = list(rows.data.keys())
             stmt += ' ({}) VALUES \n'.format(', '.join(col_names))
             stmt += '({})'.format(rows.get_insert_vals(col_names))
             self.db.execute(stmt, commit=commit)
```

### Comparing `ja_basedb-0.0.14/ja_basedb.egg-info/PKG-INFO` & `ja_basedb-0.0.15/ja_basedb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ja_basedb
-Version: 0.0.14
+Version: 0.0.15
 Summary: Classes wrapping database functions
 Author-email: Joseph Areeda <joe@areeda.com>
 Maintainer-email: Joseph Areeda <joe@areeda.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ja_basedb-0.0.14/pyproject.toml` & `ja_basedb-0.0.15/pyproject.toml`

 * *Files identical despite different names*


# Comparing `tmp/django_d1db-0.0.3.tar.gz` & `tmp/django_d1db-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_d1db-0.0.3.tar", last modified: Mon May 20 17:28:25 2024, max compression
+gzip compressed data, was "django_d1db-0.0.4.tar", last modified: Mon May 20 21:47:04 2024, max compression
```

## Comparing `django_d1db-0.0.3.tar` & `django_d1db-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 gmassadas   (502) staff       (20)        0 2024-05-20 17:28:25.594466 django_d1db-0.0.3/
--rw-r--r--   0 gmassadas   (502) staff       (20)     1073 2024-05-20 16:10:54.000000 django_d1db-0.0.3/LICENSE
--rw-r--r--   0 gmassadas   (502) staff       (20)     1563 2024-05-20 17:28:25.594038 django_d1db-0.0.3/PKG-INFO
--rw-r--r--   0 gmassadas   (502) staff       (20)      771 2024-05-20 17:09:44.000000 django_d1db-0.0.3/README.md
-drwxr-xr-x   0 gmassadas   (502) staff       (20)        0 2024-05-20 17:28:25.591341 django_d1db-0.0.3/django_d1/
--rw-r--r--   0 gmassadas   (502) staff       (20)        0 2024-05-19 10:45:59.000000 django_d1db-0.0.3/django_d1/__init__.py
--rw-r--r--   0 gmassadas   (502) staff       (20)     2685 2024-05-20 17:27:20.000000 django_d1db-0.0.3/django_d1/base.py
--rw-r--r--   0 gmassadas   (502) staff       (20)      140 2024-05-20 16:15:05.000000 django_d1db-0.0.3/django_d1/client.py
--rw-r--r--   0 gmassadas   (502) staff       (20)      150 2024-05-20 16:12:43.000000 django_d1db-0.0.3/django_d1/creation.py
--rw-r--r--   0 gmassadas   (502) staff       (20)     5222 2024-05-20 16:10:01.000000 django_d1db-0.0.3/django_d1/database.py
--rw-r--r--   0 gmassadas   (502) staff       (20)      738 2024-05-20 17:18:25.000000 django_d1db-0.0.3/django_d1/features.py
--rw-r--r--   0 gmassadas   (502) staff       (20)      175 2024-05-20 16:18:30.000000 django_d1db-0.0.3/django_d1/introspection.py
--rw-r--r--   0 gmassadas   (502) staff       (20)     2470 2024-05-20 16:20:43.000000 django_d1db-0.0.3/django_d1/operations.py
--rw-r--r--   0 gmassadas   (502) staff       (20)      415 2024-05-20 17:07:10.000000 django_d1db-0.0.3/django_d1/schema.py
-drwxr-xr-x   0 gmassadas   (502) staff       (20)        0 2024-05-20 17:28:25.593565 django_d1db-0.0.3/django_d1db.egg-info/
--rw-r--r--   0 gmassadas   (502) staff       (20)     1563 2024-05-20 17:28:25.000000 django_d1db-0.0.3/django_d1db.egg-info/PKG-INFO
--rw-r--r--   0 gmassadas   (502) staff       (20)      369 2024-05-20 17:28:25.000000 django_d1db-0.0.3/django_d1db.egg-info/SOURCES.txt
--rw-r--r--   0 gmassadas   (502) staff       (20)        1 2024-05-20 17:28:25.000000 django_d1db-0.0.3/django_d1db.egg-info/dependency_links.txt
--rw-r--r--   0 gmassadas   (502) staff       (20)       10 2024-05-20 17:28:25.000000 django_d1db-0.0.3/django_d1db.egg-info/top_level.txt
--rw-r--r--   0 gmassadas   (502) staff       (20)      785 2024-05-20 17:28:09.000000 django_d1db-0.0.3/pyproject.toml
--rw-r--r--   0 gmassadas   (502) staff       (20)       38 2024-05-20 17:28:25.594562 django_d1db-0.0.3/setup.cfg
+drwxr-xr-x   0 gmassadas   (502) staff       (20)        0 2024-05-20 21:47:04.723789 django_d1db-0.0.4/
+-rw-r--r--   0 gmassadas   (502) staff       (20)     1073 2024-05-20 16:10:54.000000 django_d1db-0.0.4/LICENSE
+-rw-r--r--   0 gmassadas   (502) staff       (20)     1563 2024-05-20 21:47:04.723010 django_d1db-0.0.4/PKG-INFO
+-rw-r--r--   0 gmassadas   (502) staff       (20)      771 2024-05-20 17:09:44.000000 django_d1db-0.0.4/README.md
+drwxr-xr-x   0 gmassadas   (502) staff       (20)        0 2024-05-20 21:47:04.719098 django_d1db-0.0.4/django_d1/
+-rw-r--r--   0 gmassadas   (502) staff       (20)        0 2024-05-19 10:45:59.000000 django_d1db-0.0.4/django_d1/__init__.py
+-rw-r--r--   0 gmassadas   (502) staff       (20)     2674 2024-05-20 20:58:52.000000 django_d1db-0.0.4/django_d1/base.py
+-rw-r--r--   0 gmassadas   (502) staff       (20)      140 2024-05-20 17:29:56.000000 django_d1db-0.0.4/django_d1/client.py
+-rw-r--r--   0 gmassadas   (502) staff       (20)      150 2024-05-20 17:29:56.000000 django_d1db-0.0.4/django_d1/creation.py
+-rw-r--r--   0 gmassadas   (502) staff       (20)     5219 2024-05-20 20:46:35.000000 django_d1db-0.0.4/django_d1/database.py
+-rw-r--r--   0 gmassadas   (502) staff       (20)     1277 2024-05-20 21:46:50.000000 django_d1db-0.0.4/django_d1/features.py
+-rw-r--r--   0 gmassadas   (502) staff       (20)      175 2024-05-20 17:29:56.000000 django_d1db-0.0.4/django_d1/introspection.py
+-rw-r--r--   0 gmassadas   (502) staff       (20)     2719 2024-05-20 21:42:30.000000 django_d1db-0.0.4/django_d1/operations.py
+-rw-r--r--   0 gmassadas   (502) staff       (20)      415 2024-05-20 17:29:56.000000 django_d1db-0.0.4/django_d1/schema.py
+drwxr-xr-x   0 gmassadas   (502) staff       (20)        0 2024-05-20 21:47:04.722125 django_d1db-0.0.4/django_d1db.egg-info/
+-rw-r--r--   0 gmassadas   (502) staff       (20)     1563 2024-05-20 21:47:04.000000 django_d1db-0.0.4/django_d1db.egg-info/PKG-INFO
+-rw-r--r--   0 gmassadas   (502) staff       (20)      369 2024-05-20 21:47:04.000000 django_d1db-0.0.4/django_d1db.egg-info/SOURCES.txt
+-rw-r--r--   0 gmassadas   (502) staff       (20)        1 2024-05-20 21:47:04.000000 django_d1db-0.0.4/django_d1db.egg-info/dependency_links.txt
+-rw-r--r--   0 gmassadas   (502) staff       (20)       10 2024-05-20 21:47:04.000000 django_d1db-0.0.4/django_d1db.egg-info/top_level.txt
+-rw-r--r--   0 gmassadas   (502) staff       (20)      785 2024-05-20 21:46:50.000000 django_d1db-0.0.4/pyproject.toml
+-rw-r--r--   0 gmassadas   (502) staff       (20)       38 2024-05-20 21:47:04.723960 django_d1db-0.0.4/setup.cfg
```

### Comparing `django_d1db-0.0.3/LICENSE` & `django_d1db-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_d1db-0.0.3/PKG-INFO` & `django_d1db-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-d1db
-Version: 0.0.3
+Version: 0.0.4
 Summary: Django backend for Cloudflare D1
 Author: Gabriel Massadas
 Project-URL: Bug Reports, https://github.com/G4brym/django-d1/issues
 Project-URL: Source, https://github.com/G4brym/django-d1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 5.0
```

### Comparing `django_d1db-0.0.3/README.md` & `django_d1db-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `django_d1db-0.0.3/django_d1/base.py` & `django_d1db-0.0.4/django_d1/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,18 @@
     client_class = DatabaseClient
     creation_class = DatabaseCreation
     # Classes instantiated in __init__().
     features_class = DatabaseFeatures
     introspection_class = DatabaseIntrospection
     ops_class = DatabaseOperations
 
-    transaction_modes = frozenset(["IMMEDIATE"])
+    transaction_modes = frozenset([])
 
     def get_database_version(self):
-        return (1,)
+        return (4,)
 
     def get_connection_params(self):
         settings_dict = self.settings_dict
         if not settings_dict["CLOUDFLARE_DATABASE_ID"]:
             raise ImproperlyConfigured(
                 "settings.DATABASES is improperly configured. "
                 "Please supply the CLOUDFLARE_DATABASE_ID value."
```

### Comparing `django_d1db-0.0.3/django_d1/database.py` & `django_d1db-0.0.4/django_d1/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,36 +95,37 @@
 
     def commit(self):
         return  # No commits allowed
 
     def rollback(self):
         return  # No commits allowed
 
-    def get_query(self):
-        query = self.query
+    def process_query(self, query):
         query = query.replace('%s', '?')
 
         if self._defer_foreign_keys:
             return f'''
             PRAGMA defer_foreign_keys = on
             
             {query}
 
             PRAGMA defer_foreign_keys = off
             '''
 
         return query
 
     @retry(times=3, exceptions=(InternalError,))
-    def run_query(self):
+    def run_query(self, query, params=None):
+        proc_query = self.process_query(query)
+
         conn = http.client.HTTPSConnection("api.cloudflare.com", timeout=20.0)
 
         payload = {
-            "params": self.params,
-            "sql": self.get_query()
+            "params": params,
+            "sql": proc_query
         }
 
         headers = {
             'Content-Type': "application/json",
             'Authorization': f"Bearer {self.token}"
         }
 
@@ -159,18 +160,15 @@
 
         return result
 
     query = None
     params = None
 
     def execute(self, query, params=None):
-        self.query = query
-        self.params = params
-
-        self.results = self.run_query()
+        self.results = self.run_query(query, params)
 
         return self
 
     def fetchone(self):
         if len(self.results.data) > 0:
             return self.results.data.pop()
         return None
```

### Comparing `django_d1db-0.0.3/django_d1/operations.py` & `django_d1db-0.0.4/django_d1/operations.py`

 * *Files 22% similar despite different names*

```diff
@@ -47,7 +47,12 @@
                 return sql % params
             except:
                 return sql
         # For consistency with SQLiteCursorWrapper.execute(), just return sql
         # when there are no parameters. See #13648 and #17158.
         else:
             return sql
+
+    def bulk_insert_sql(self, fields, placeholder_rows):
+        placeholder_rows_sql = (", ".join(row) for row in placeholder_rows)
+        values_sql = ", ".join("(%s)" % sql for sql in placeholder_rows_sql)
+        return "VALUES " + values_sql
```

### Comparing `django_d1db-0.0.3/django_d1db.egg-info/PKG-INFO` & `django_d1db-0.0.4/django_d1db.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-d1db
-Version: 0.0.3
+Version: 0.0.4
 Summary: Django backend for Cloudflare D1
 Author: Gabriel Massadas
 Project-URL: Bug Reports, https://github.com/G4brym/django-d1/issues
 Project-URL: Source, https://github.com/G4brym/django-d1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 5.0
```

### Comparing `django_d1db-0.0.3/pyproject.toml` & `django_d1db-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-d1db"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Gabriel Massadas" },
 ]
 description = "Django backend for Cloudflare D1"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```


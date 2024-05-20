# Comparing `tmp/bravaorm-0.0.8.tar.gz` & `tmp/bravaorm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bravaorm-0.0.8.tar", last modified: Thu Apr 29 01:37:54 2021, max compression
+gzip compressed data, was "dist/bravaorm-0.0.9.tar", last modified: Sat May  1 10:44:08 2021, max compression
```

## Comparing `bravaorm-0.0.8.tar` & `bravaorm-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 robertoneves   (501) staff       (20)        0 2021-04-29 01:37:54.551697 bravaorm-0.0.8/
--rw-r--r--   0 robertoneves   (501) staff       (20)     1070 2021-03-31 12:56:40.000000 bravaorm-0.0.8/LICENSE
--rw-r--r--   0 robertoneves   (501) staff       (20)      120 2021-03-31 12:55:55.000000 bravaorm-0.0.8/MANIFEST.in
--rw-r--r--   0 robertoneves   (501) staff       (20)    16389 2021-04-29 01:37:54.551968 bravaorm-0.0.8/PKG-INFO
--rw-r--r--   0 robertoneves   (501) staff       (20)    12818 2021-04-19 21:14:14.000000 bravaorm-0.0.8/README.md
-drwxr-xr-x   0 robertoneves   (501) staff       (20)        0 2021-04-29 01:37:54.538715 bravaorm-0.0.8/bravaorm/
--rw-r--r--   0 robertoneves   (501) staff       (20)      155 2021-04-09 15:01:53.000000 bravaorm-0.0.8/bravaorm/__init__.py
-drwxr-xr-x   0 robertoneves   (501) staff       (20)        0 2021-04-29 01:37:54.542770 bravaorm-0.0.8/bravaorm/context/
--rw-r--r--   0 robertoneves   (501) staff       (20)       23 2021-03-31 13:03:47.000000 bravaorm-0.0.8/bravaorm/context/__init__.py
--rw-r--r--   0 robertoneves   (501) staff       (20)    23405 2021-04-29 01:33:33.000000 bravaorm-0.0.8/bravaorm/context/connection.py
--rw-r--r--   0 robertoneves   (501) staff       (20)     4265 2021-04-29 01:33:36.000000 bravaorm-0.0.8/bravaorm/context/database.py
-drwxr-xr-x   0 robertoneves   (501) staff       (20)        0 2021-04-29 01:37:54.544923 bravaorm-0.0.8/bravaorm/entity/
--rw-r--r--   0 robertoneves   (501) staff       (20)       99 2021-04-08 11:03:25.000000 bravaorm-0.0.8/bravaorm/entity/__init__.py
--rw-r--r--   0 robertoneves   (501) staff       (20)     7823 2021-04-19 21:39:37.000000 bravaorm-0.0.8/bravaorm/entity/datatype.py
--rw-r--r--   0 robertoneves   (501) staff       (20)     3976 2021-04-19 16:59:13.000000 bravaorm-0.0.8/bravaorm/entity/entity.py
-drwxr-xr-x   0 robertoneves   (501) staff       (20)        0 2021-04-29 01:37:54.548545 bravaorm-0.0.8/bravaorm/utils/
--rw-r--r--   0 robertoneves   (501) staff       (20)        0 2021-03-31 12:59:51.000000 bravaorm-0.0.8/bravaorm/utils/__init__.py
--rw-r--r--   0 robertoneves   (501) staff       (20)     9423 2021-04-09 15:02:24.000000 bravaorm-0.0.8/bravaorm/utils/angular.py
--rw-r--r--   0 robertoneves   (501) staff       (20)    11542 2021-04-29 01:09:46.000000 bravaorm-0.0.8/bravaorm/utils/inflector.py
-drwxr-xr-x   0 robertoneves   (501) staff       (20)        0 2021-04-29 01:37:54.550546 bravaorm-0.0.8/bravaorm/utils/log/
--rw-r--r--   0 robertoneves   (501) staff       (20)     1715 2021-04-29 01:36:01.000000 bravaorm-0.0.8/bravaorm/utils/log/__init__.py
--rw-r--r--   0 robertoneves   (501) staff       (20)      796 2021-04-19 21:05:04.000000 bravaorm-0.0.8/bravaorm/utils/log/colored_log.py
--rw-r--r--   0 robertoneves   (501) staff       (20)     2735 2021-04-19 21:05:04.000000 bravaorm-0.0.8/bravaorm/utils/log/colors.py
--rw-r--r--   0 robertoneves   (501) staff       (20)    10796 2021-04-20 17:34:11.000000 bravaorm-0.0.8/bravaorm/utils/make.py
--rw-r--r--   0 robertoneves   (501) staff       (20)      259 2021-04-29 01:09:41.000000 bravaorm-0.0.8/bravaorm/utils/singleton.py
-drwxr-xr-x   0 robertoneves   (501) staff       (20)        0 2021-04-29 01:37:54.541015 bravaorm-0.0.8/bravaorm.egg-info/
--rw-r--r--   0 robertoneves   (501) staff       (20)    16389 2021-04-29 01:37:54.000000 bravaorm-0.0.8/bravaorm.egg-info/PKG-INFO
--rw-r--r--   0 robertoneves   (501) staff       (20)      655 2021-04-29 01:37:54.000000 bravaorm-0.0.8/bravaorm.egg-info/SOURCES.txt
--rw-r--r--   0 robertoneves   (501) staff       (20)        1 2021-04-29 01:37:54.000000 bravaorm-0.0.8/bravaorm.egg-info/dependency_links.txt
--rw-r--r--   0 robertoneves   (501) staff       (20)       23 2021-04-29 01:37:54.000000 bravaorm-0.0.8/bravaorm.egg-info/requires.txt
--rw-r--r--   0 robertoneves   (501) staff       (20)        9 2021-04-29 01:37:54.000000 bravaorm-0.0.8/bravaorm.egg-info/top_level.txt
--rw-r--r--   0 robertoneves   (501) staff       (20)       23 2021-03-31 12:57:08.000000 bravaorm-0.0.8/requirements.txt
--rw-r--r--   0 robertoneves   (501) staff       (20)      102 2021-04-29 01:37:54.552437 bravaorm-0.0.8/setup.cfg
--rw-r--r--   0 robertoneves   (501) staff       (20)      936 2021-04-29 01:37:24.000000 bravaorm-0.0.8/setup.py
-drwxr-xr-x   0 robertoneves   (501) staff       (20)        0 2021-04-29 01:37:54.551131 bravaorm-0.0.8/test/
--rw-r--r--   0 robertoneves   (501) staff       (20)      685 2021-04-19 21:56:19.000000 bravaorm-0.0.8/test/test.py
+drwxr-xr-x   0 robertoneves   (501) staff       (20)        0 2021-05-01 10:44:08.730086 bravaorm-0.0.9/
+-rw-r--r--   0 robertoneves   (501) staff       (20)     1070 2021-03-31 12:56:40.000000 bravaorm-0.0.9/LICENSE
+-rw-r--r--   0 robertoneves   (501) staff       (20)      120 2021-03-31 12:55:55.000000 bravaorm-0.0.9/MANIFEST.in
+-rw-r--r--   0 robertoneves   (501) staff       (20)    16389 2021-05-01 10:44:08.730558 bravaorm-0.0.9/PKG-INFO
+-rw-r--r--   0 robertoneves   (501) staff       (20)    12818 2021-04-19 21:14:14.000000 bravaorm-0.0.9/README.md
+drwxr-xr-x   0 robertoneves   (501) staff       (20)        0 2021-05-01 10:44:08.712782 bravaorm-0.0.9/bravaorm/
+-rw-r--r--   0 robertoneves   (501) staff       (20)      155 2021-04-09 15:01:53.000000 bravaorm-0.0.9/bravaorm/__init__.py
+drwxr-xr-x   0 robertoneves   (501) staff       (20)        0 2021-05-01 10:44:08.719745 bravaorm-0.0.9/bravaorm/context/
+-rw-r--r--   0 robertoneves   (501) staff       (20)       23 2021-03-31 13:03:47.000000 bravaorm-0.0.9/bravaorm/context/__init__.py
+-rw-r--r--   0 robertoneves   (501) staff       (20)    23453 2021-05-01 10:38:43.000000 bravaorm-0.0.9/bravaorm/context/connection.py
+-rw-r--r--   0 robertoneves   (501) staff       (20)     4265 2021-04-29 01:33:36.000000 bravaorm-0.0.9/bravaorm/context/database.py
+drwxr-xr-x   0 robertoneves   (501) staff       (20)        0 2021-05-01 10:44:08.722215 bravaorm-0.0.9/bravaorm/entity/
+-rw-r--r--   0 robertoneves   (501) staff       (20)       99 2021-04-08 11:03:25.000000 bravaorm-0.0.9/bravaorm/entity/__init__.py
+-rw-r--r--   0 robertoneves   (501) staff       (20)     7823 2021-04-19 21:39:37.000000 bravaorm-0.0.9/bravaorm/entity/datatype.py
+-rw-r--r--   0 robertoneves   (501) staff       (20)     3976 2021-04-19 16:59:13.000000 bravaorm-0.0.9/bravaorm/entity/entity.py
+drwxr-xr-x   0 robertoneves   (501) staff       (20)        0 2021-05-01 10:44:08.726041 bravaorm-0.0.9/bravaorm/utils/
+-rw-r--r--   0 robertoneves   (501) staff       (20)        0 2021-03-31 12:59:51.000000 bravaorm-0.0.9/bravaorm/utils/__init__.py
+-rw-r--r--   0 robertoneves   (501) staff       (20)     9423 2021-04-09 15:02:24.000000 bravaorm-0.0.9/bravaorm/utils/angular.py
+-rw-r--r--   0 robertoneves   (501) staff       (20)    11542 2021-04-29 01:09:46.000000 bravaorm-0.0.9/bravaorm/utils/inflector.py
+drwxr-xr-x   0 robertoneves   (501) staff       (20)        0 2021-05-01 10:44:08.728485 bravaorm-0.0.9/bravaorm/utils/log/
+-rw-r--r--   0 robertoneves   (501) staff       (20)     1715 2021-04-29 01:36:01.000000 bravaorm-0.0.9/bravaorm/utils/log/__init__.py
+-rw-r--r--   0 robertoneves   (501) staff       (20)      796 2021-04-19 21:05:04.000000 bravaorm-0.0.9/bravaorm/utils/log/colored_log.py
+-rw-r--r--   0 robertoneves   (501) staff       (20)     2735 2021-04-19 21:05:04.000000 bravaorm-0.0.9/bravaorm/utils/log/colors.py
+-rw-r--r--   0 robertoneves   (501) staff       (20)    10796 2021-04-20 17:34:11.000000 bravaorm-0.0.9/bravaorm/utils/make.py
+-rw-r--r--   0 robertoneves   (501) staff       (20)      259 2021-04-29 01:09:41.000000 bravaorm-0.0.9/bravaorm/utils/singleton.py
+drwxr-xr-x   0 robertoneves   (501) staff       (20)        0 2021-05-01 10:44:08.716912 bravaorm-0.0.9/bravaorm.egg-info/
+-rw-r--r--   0 robertoneves   (501) staff       (20)    16389 2021-05-01 10:44:08.000000 bravaorm-0.0.9/bravaorm.egg-info/PKG-INFO
+-rw-r--r--   0 robertoneves   (501) staff       (20)      655 2021-05-01 10:44:08.000000 bravaorm-0.0.9/bravaorm.egg-info/SOURCES.txt
+-rw-r--r--   0 robertoneves   (501) staff       (20)        1 2021-05-01 10:44:08.000000 bravaorm-0.0.9/bravaorm.egg-info/dependency_links.txt
+-rw-r--r--   0 robertoneves   (501) staff       (20)       23 2021-05-01 10:44:08.000000 bravaorm-0.0.9/bravaorm.egg-info/requires.txt
+-rw-r--r--   0 robertoneves   (501) staff       (20)        9 2021-05-01 10:44:08.000000 bravaorm-0.0.9/bravaorm.egg-info/top_level.txt
+-rw-r--r--   0 robertoneves   (501) staff       (20)       23 2021-03-31 12:57:08.000000 bravaorm-0.0.9/requirements.txt
+-rw-r--r--   0 robertoneves   (501) staff       (20)      102 2021-05-01 10:44:08.731270 bravaorm-0.0.9/setup.cfg
+-rw-r--r--   0 robertoneves   (501) staff       (20)      936 2021-05-01 10:43:08.000000 bravaorm-0.0.9/setup.py
+drwxr-xr-x   0 robertoneves   (501) staff       (20)        0 2021-05-01 10:44:08.729291 bravaorm-0.0.9/test/
+-rw-r--r--   0 robertoneves   (501) staff       (20)      685 2021-04-19 21:56:19.000000 bravaorm-0.0.9/test/test.py
```

### Comparing `bravaorm-0.0.8/LICENSE` & `bravaorm-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bravaorm-0.0.8/PKG-INFO` & `bravaorm-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bravaorm
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python ORM for MySQL
 Home-page: https://github.com/robertons/bravaorm
 Author: Roberto Neves
 Author-email: robertonsilva@gmail.com
 License: MIT
 Description:
```

### Comparing `bravaorm-0.0.8/README.md` & `bravaorm-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bravaorm-0.0.8/bravaorm/context/connection.py` & `bravaorm-0.0.9/bravaorm/context/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,17 +312,17 @@
 
     def __format_delete_query__(self):
         _where = [w for w in self._where if self.__is_clause_table__(w)]
         return f"DELETE FROM {self._table} WHERE ({' AND '.join(_where)})"
 
     def __format_object_insert_query__(self, obj):
         table =  self._inflector.tableize(obj.__class__.__name__)
-        keys = ', '.join([key for key, value in obj.__metadata__['data'].items() if value])
-        values = ', '.join([f'%({key})s' for key, value in obj.__metadata__['data'].items() if value])
-        on_keys = ', '.join([f"{key}=%({key})s" for key, value in obj.__metadata__['data'].items() if value])
+        keys = ', '.join([key for key, value in obj.__metadata__['data'].items() if value is not None])
+        values = ', '.join([f'%({key})s' for key, value in obj.__metadata__['data'].items() if value is not None])
+        on_keys = ', '.join([f"{key}=%({key})s" for key, value in obj.__metadata__['data'].items() if value is not None])
         return f"INSERT INTO {table} ({keys}) VALUES ({values}) ON DUPLICATE KEY UPDATE {on_keys}"
 
     def select(self, *fields):
         self._select = self.__format_fields__(*fields)
         return self
 
     def distinct(self, *fields):
@@ -448,15 +448,15 @@
             else:
                 raise Exception("delete method requires where condition or object")
 
     def __save__object__(self, obj):
         Debug("Saving Object")
         def do_object(_obj):
             _add_query = self.__format_object_insert_query__(_obj)
-            _last_row_id = self._conn.save(_add_query, {key:value for key, value in _obj.__metadata__['data'].items() if value})
+            _last_row_id = self._conn.save(_add_query, {key:value for key, value in _obj.__metadata__['data'].items() if value is not None})
             if _last_row_id:
                 _pk_key = obj.__metadata__['pk'][0]
                 _obj.__setattr__(_pk_key, _last_row_id)
 
         do_object(obj)
 
         def do_relacional(_rel, _obj, _sub_item):
```

### Comparing `bravaorm-0.0.8/bravaorm/context/database.py` & `bravaorm-0.0.9/bravaorm/context/database.py`

 * *Files identical despite different names*

### Comparing `bravaorm-0.0.8/bravaorm/entity/datatype.py` & `bravaorm-0.0.9/bravaorm/entity/datatype.py`

 * *Files identical despite different names*

### Comparing `bravaorm-0.0.8/bravaorm/entity/entity.py` & `bravaorm-0.0.9/bravaorm/entity/entity.py`

 * *Files identical despite different names*

### Comparing `bravaorm-0.0.8/bravaorm/utils/angular.py` & `bravaorm-0.0.9/bravaorm/utils/angular.py`

 * *Files identical despite different names*

### Comparing `bravaorm-0.0.8/bravaorm/utils/inflector.py` & `bravaorm-0.0.9/bravaorm/utils/inflector.py`

 * *Files identical despite different names*

### Comparing `bravaorm-0.0.8/bravaorm/utils/log/__init__.py` & `bravaorm-0.0.9/bravaorm/utils/log/__init__.py`

 * *Files identical despite different names*

### Comparing `bravaorm-0.0.8/bravaorm/utils/log/colored_log.py` & `bravaorm-0.0.9/bravaorm/utils/log/colored_log.py`

 * *Files identical despite different names*

### Comparing `bravaorm-0.0.8/bravaorm/utils/log/colors.py` & `bravaorm-0.0.9/bravaorm/utils/log/colors.py`

 * *Files identical despite different names*

### Comparing `bravaorm-0.0.8/bravaorm/utils/make.py` & `bravaorm-0.0.9/bravaorm/utils/make.py`

 * *Files identical despite different names*

### Comparing `bravaorm-0.0.8/bravaorm.egg-info/PKG-INFO` & `bravaorm-0.0.9/bravaorm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bravaorm
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python ORM for MySQL
 Home-page: https://github.com/robertons/bravaorm
 Author: Roberto Neves
 Author-email: robertonsilva@gmail.com
 License: MIT
 Description:
```

### Comparing `bravaorm-0.0.8/bravaorm.egg-info/SOURCES.txt` & `bravaorm-0.0.9/bravaorm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bravaorm-0.0.8/setup.py` & `bravaorm-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 readme = open('README.md').read()
 
 with open('requirements.txt') as reqs:
     requirements = reqs.read().split()
 
 setuptools.setup(
     name='bravaorm',
-    version='0.0.8',
+    version='0.0.9',
     description='Python ORM for MySQL',
     author='Roberto Neves',
     author_email='robertonsilva@gmail.com',
     url='https://github.com/robertons/bravaorm',
     packages=setuptools.find_packages(),
     install_requires=requirements,
     long_description=readme,
```

### Comparing `bravaorm-0.0.8/test/test.py` & `bravaorm-0.0.9/test/test.py`

 * *Files identical despite different names*


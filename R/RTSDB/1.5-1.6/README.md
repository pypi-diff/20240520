# Comparing `tmp/RTSDB-1.5.tar.gz` & `tmp/RTSDB-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RTSDB-1.5.tar", last modified: Mon Apr  1 12:58:17 2024, max compression
+gzip compressed data, was "RTSDB-1.6.tar", last modified: Sun May 19 19:01:24 2024, max compression
```

## Comparing `RTSDB-1.5.tar` & `RTSDB-1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 12:58:17.736977 RTSDB-1.5/
--rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTSDB-1.5/LICENCE
--rw-rw-rw-   0        0        0     7014 2024-04-01 12:58:17.736977 RTSDB-1.5/PKG-INFO
--rw-rw-rw-   0        0        0     6321 2024-04-01 09:45:01.000000 RTSDB-1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 12:58:17.711231 RTSDB-1.5/RTSDB.egg-info/
--rw-rw-rw-   0        0        0     7014 2024-04-01 12:58:17.000000 RTSDB-1.5/RTSDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-04-01 12:58:17.000000 RTSDB-1.5/RTSDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 12:58:17.000000 RTSDB-1.5/RTSDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-01 12:58:17.000000 RTSDB-1.5/RTSDB.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-01 12:58:17.713752 RTSDB-1.5/RTSDataBase/
--rw-rw-rw-   0        0        0    12015 2024-04-01 12:58:07.000000 RTSDB-1.5/RTSDataBase/RTSDB.py
--rw-rw-rw-   0        0        0       21 2024-04-01 08:52:47.000000 RTSDB-1.5/RTSDataBase/__init__.py
--rw-rw-rw-   0        0        0      600 2024-03-31 19:14:15.000000 RTSDB-1.5/RTSDataBase/exceptions.py
--rw-rw-rw-   0        0        0      569 2024-03-31 15:51:44.000000 RTSDB-1.5/RTSDataBase/typotest.py
--rw-rw-rw-   0        0        0       42 2024-04-01 12:58:17.736977 RTSDB-1.5/setup.cfg
--rw-rw-rw-   0        0        0      861 2024-04-01 12:58:16.000000 RTSDB-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:01:24.377465 RTSDB-1.6/
+-rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTSDB-1.6/LICENCE
+-rw-rw-rw-   0        0        0     7091 2024-05-19 19:01:24.376965 RTSDB-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6398 2024-05-19 19:00:44.000000 RTSDB-1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 19:01:24.372953 RTSDB-1.6/RTSDB.egg-info/
+-rw-rw-rw-   0        0        0     7091 2024-05-19 19:01:24.000000 RTSDB-1.6/RTSDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-05-19 19:01:24.000000 RTSDB-1.6/RTSDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 19:01:24.000000 RTSDB-1.6/RTSDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-19 19:01:24.000000 RTSDB-1.6/RTSDB.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 19:01:24.375965 RTSDB-1.6/RTSDataBase/
+-rw-rw-rw-   0        0        0    12025 2024-05-19 18:59:42.000000 RTSDB-1.6/RTSDataBase/RTSDB.py
+-rw-rw-rw-   0        0        0       21 2024-04-01 08:52:47.000000 RTSDB-1.6/RTSDataBase/__init__.py
+-rw-rw-rw-   0        0        0      600 2024-03-31 19:14:15.000000 RTSDB-1.6/RTSDataBase/exceptions.py
+-rw-rw-rw-   0        0        0      569 2024-03-31 15:51:44.000000 RTSDB-1.6/RTSDataBase/typotest.py
+-rw-rw-rw-   0        0        0       42 2024-05-19 19:01:24.377465 RTSDB-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      861 2024-05-19 19:00:53.000000 RTSDB-1.6/setup.py
```

### Comparing `RTSDB-1.5/LICENCE` & `RTSDB-1.6/LICENCE`

 * *Files identical despite different names*

### Comparing `RTSDB-1.5/PKG-INFO` & `RTSDB-1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTSDB
-Version: 1.5
+Version: 1.6
 Summary: Create yourself a simple database with this package.
 Home-page: https://github.com/RandomTimeLP/RTS_DataBase/
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: database
 Platform: UNKNOWN
@@ -17,14 +17,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # This is RTS_Simpledatabase
 
 a little module for Python to create databases.
 
+### "Patch notes"
+
+- Fixed a bug that prevented updates
+
+# How to use
+
 For the "How to use" lets get some sample data:
 
 | fieldname      | userid        | displayname   | balance  | joined     | note  
 |----------------|---------------|---------------|----------|------------|-------
 | example value  | 9783836285131 | randomtimetv  | 6.50     | 31.03.2024 |       
 | format         | str           | str           | float    | str        | str   
 | state          | unique        | modular       | modular  | locked     | loose
```

### Comparing `RTSDB-1.5/README.md` & `RTSDB-1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # This is RTS_Simpledatabase
 
 a little module for Python to create databases.
 
+### "Patch notes"
+
+- Fixed a bug that prevented updates
+
+# How to use
+
 For the "How to use" lets get some sample data:
 
 | fieldname      | userid        | displayname   | balance  | joined     | note  
 |----------------|---------------|---------------|----------|------------|-------
 | example value  | 9783836285131 | randomtimetv  | 6.50     | 31.03.2024 |       
 | format         | str           | str           | float    | str        | str   
 | state          | unique        | modular       | modular  | locked     | loose
```

### Comparing `RTSDB-1.5/RTSDB.egg-info/PKG-INFO` & `RTSDB-1.6/RTSDB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTSDB
-Version: 1.5
+Version: 1.6
 Summary: Create yourself a simple database with this package.
 Home-page: https://github.com/RandomTimeLP/RTS_DataBase/
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: database
 Platform: UNKNOWN
@@ -17,14 +17,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # This is RTS_Simpledatabase
 
 a little module for Python to create databases.
 
+### "Patch notes"
+
+- Fixed a bug that prevented updates
+
+# How to use
+
 For the "How to use" lets get some sample data:
 
 | fieldname      | userid        | displayname   | balance  | joined     | note  
 |----------------|---------------|---------------|----------|------------|-------
 | example value  | 9783836285131 | randomtimetv  | 6.50     | 31.03.2024 |       
 | format         | str           | str           | float    | str        | str   
 | state          | unique        | modular       | modular  | locked     | loose
```

### Comparing `RTSDB-1.5/RTSDataBase/RTSDB.py` & `RTSDB-1.6/RTSDataBase/RTSDB.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,19 +61,19 @@
             'int': int
         }
 
         field_type = self.header['format'][self.header['fields'].index(field)]
 
         if type == '__any':
             #print(f"Field {field} is type any")
-            return
+            return True
 
         if not isinstance(record[field], type_map[field_type]):
             raise InvalidType(f'⛔ InvalidType: "{field}" does not match typerule "{field_type}" in: {record}')
-        return
+        return True
 
     # Used only by Internal functions
     def _validate_create(self, record):
         if not isinstance(record, dict):
             raise ValueError(f"⚠️  ValueError: not a dict in {record}")
 
         # Check if there are extra fields in the record
```

### Comparing `RTSDB-1.5/RTSDataBase/exceptions.py` & `RTSDB-1.6/RTSDataBase/exceptions.py`

 * *Files identical despite different names*

### Comparing `RTSDB-1.5/RTSDataBase/typotest.py` & `RTSDB-1.6/RTSDataBase/typotest.py`

 * *Files identical despite different names*

### Comparing `RTSDB-1.5/setup.py` & `RTSDB-1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RTSDB',
-    version='1.5',
+    version='1.6',
     packages=find_packages(),
     description='Create yourself a simple database with this package.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='MIT with required credit to the author.',
```


# Comparing `tmp/RTSDB-1.6.tar.gz` & `tmp/RTSDB-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RTSDB-1.6.tar", last modified: Sun May 19 19:01:24 2024, max compression
+gzip compressed data, was "RTSDB-1.7.tar", last modified: Mon May 20 17:52:01 2024, max compression
```

## Comparing `RTSDB-1.6.tar` & `RTSDB-1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 19:01:24.377465 RTSDB-1.6/
--rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTSDB-1.6/LICENCE
--rw-rw-rw-   0        0        0     7091 2024-05-19 19:01:24.376965 RTSDB-1.6/PKG-INFO
--rw-rw-rw-   0        0        0     6398 2024-05-19 19:00:44.000000 RTSDB-1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 19:01:24.372953 RTSDB-1.6/RTSDB.egg-info/
--rw-rw-rw-   0        0        0     7091 2024-05-19 19:01:24.000000 RTSDB-1.6/RTSDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-05-19 19:01:24.000000 RTSDB-1.6/RTSDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 19:01:24.000000 RTSDB-1.6/RTSDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-19 19:01:24.000000 RTSDB-1.6/RTSDB.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-19 19:01:24.375965 RTSDB-1.6/RTSDataBase/
--rw-rw-rw-   0        0        0    12025 2024-05-19 18:59:42.000000 RTSDB-1.6/RTSDataBase/RTSDB.py
--rw-rw-rw-   0        0        0       21 2024-04-01 08:52:47.000000 RTSDB-1.6/RTSDataBase/__init__.py
--rw-rw-rw-   0        0        0      600 2024-03-31 19:14:15.000000 RTSDB-1.6/RTSDataBase/exceptions.py
--rw-rw-rw-   0        0        0      569 2024-03-31 15:51:44.000000 RTSDB-1.6/RTSDataBase/typotest.py
--rw-rw-rw-   0        0        0       42 2024-05-19 19:01:24.377465 RTSDB-1.6/setup.cfg
--rw-rw-rw-   0        0        0      861 2024-05-19 19:00:53.000000 RTSDB-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:52:01.676089 RTSDB-1.7/
+-rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTSDB-1.7/LICENCE
+-rw-rw-rw-   0        0        0     7166 2024-05-20 17:52:01.676089 RTSDB-1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6473 2024-05-20 17:51:19.000000 RTSDB-1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 17:52:01.671941 RTSDB-1.7/RTSDB.egg-info/
+-rw-rw-rw-   0        0        0     7166 2024-05-20 17:52:01.000000 RTSDB-1.7/RTSDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-05-20 17:52:01.000000 RTSDB-1.7/RTSDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 17:52:01.000000 RTSDB-1.7/RTSDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-20 17:52:01.000000 RTSDB-1.7/RTSDB.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 17:52:01.674786 RTSDB-1.7/RTSDataBase/
+-rw-rw-rw-   0        0        0    12139 2024-05-20 17:49:16.000000 RTSDB-1.7/RTSDataBase/RTSDB.py
+-rw-rw-rw-   0        0        0       21 2024-04-01 08:52:47.000000 RTSDB-1.7/RTSDataBase/__init__.py
+-rw-rw-rw-   0        0        0      600 2024-03-31 19:14:15.000000 RTSDB-1.7/RTSDataBase/exceptions.py
+-rw-rw-rw-   0        0        0      569 2024-03-31 15:51:44.000000 RTSDB-1.7/RTSDataBase/typotest.py
+-rw-rw-rw-   0        0        0       42 2024-05-20 17:52:01.676588 RTSDB-1.7/setup.cfg
+-rw-rw-rw-   0        0        0      861 2024-05-20 17:49:39.000000 RTSDB-1.7/setup.py
```

### Comparing `RTSDB-1.6/LICENCE` & `RTSDB-1.7/LICENCE`

 * *Files identical despite different names*

### Comparing `RTSDB-1.6/PKG-INFO` & `RTSDB-1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTSDB
-Version: 1.6
+Version: 1.7
 Summary: Create yourself a simple database with this package.
 Home-page: https://github.com/RandomTimeLP/RTS_DataBase/
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: database
 Platform: UNKNOWN
@@ -17,17 +17,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # This is RTS_Simpledatabase
 
 a little module for Python to create databases.
 
-### "Patch notes"
+### Fix notes
 
-- Fixed a bug that prevented updates
+- Fixed a bug that did not throw a readable error if you try to update a field, that is not present in the headers.
 
 # How to use
 
 For the "How to use" lets get some sample data:
 
 | fieldname      | userid        | displayname   | balance  | joined     | note  
 |----------------|---------------|---------------|----------|------------|-------
```

### Comparing `RTSDB-1.6/README.md` & `RTSDB-1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This is RTS_Simpledatabase
 
 a little module for Python to create databases.
 
-### "Patch notes"
+### Fix notes
 
-- Fixed a bug that prevented updates
+- Fixed a bug that did not throw a readable error if you try to update a field, that is not present in the headers.
 
 # How to use
 
 For the "How to use" lets get some sample data:
 
 | fieldname      | userid        | displayname   | balance  | joined     | note  
 |----------------|---------------|---------------|----------|------------|-------
```

### Comparing `RTSDB-1.6/RTSDB.egg-info/PKG-INFO` & `RTSDB-1.7/RTSDB.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTSDB
-Version: 1.6
+Version: 1.7
 Summary: Create yourself a simple database with this package.
 Home-page: https://github.com/RandomTimeLP/RTS_DataBase/
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: database
 Platform: UNKNOWN
@@ -17,17 +17,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # This is RTS_Simpledatabase
 
 a little module for Python to create databases.
 
-### "Patch notes"
+### Fix notes
 
-- Fixed a bug that prevented updates
+- Fixed a bug that did not throw a readable error if you try to update a field, that is not present in the headers.
 
 # How to use
 
 For the "How to use" lets get some sample data:
 
 | fieldname      | userid        | displayname   | balance  | joined     | note  
 |----------------|---------------|---------------|----------|------------|-------
```

### Comparing `RTSDB-1.6/RTSDataBase/RTSDB.py` & `RTSDB-1.7/RTSDataBase/RTSDB.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,29 +167,32 @@
                 #print("Final Value: ",value)
 
 
     
         #modular_fields = [field for field, state in zip(self.header["fields"], self.header["states"]) if state == "modular"]
         unique_fields = [field for field, state in zip(self.header["fields"], self.header["states"]) if state in ["unique"]]
         locked_fields = [field for field, state in zip(self.header["fields"], self.header["states"]) if state in ["locked", "index"]]
+        
+        # checks             locked?   exists?   valid?
+        # unique nostring    No        should    yes
+       
 
         if field not in locked_fields and field in self.header["fields"] and self._validate_update({field:value}):
             if field in unique_fields and value is not None and any(record.get(field) == value for record in self.data if record is not record_to_update):
-                raise DataNotUnique(f'⛔ DataNotUnique: "{field}" must contain a unique value among all records.')
-            #print(f"Updating field {field} to value {value}")
+                raise DataNotUnique(f'⛔ DataNotUnique:177 "{field}" must contain a unique value among all records.')
+            print(f"Updating field {field} to value {value}")
             record_to_update[field] = value
         else:
+            if field in self.header["fields"]:
+                raise ValueError(f'⛔ FieldNotInHeader:181 "{field}" is not initialized in the header. You need to recreate yuor database containing the new field.')
             if field in locked_fields:
-                raise LockedField(f'🔒 LockedField: "{field}" can not be updated.')
-            elif self._validate_update({field:value}):
-                raise InvalidField(f'⛔ InvalidField: "{field}" is not in the header')
-            elif not any(record.get(field) == value for record in self.data if record is not record_to_update):
-                raise DataNotUnique(f'⛔ DataNotUnique: "{field}" must contain a unique value among all records.')
-            else:
-                raise Exception('⚠️  UnknownError: You are not suposed to encounter this message, may report this issue to the developer.')
+                raise LockedField(f'🔒 LockedField:182 "{field}" can not be updated.')
+            if self._validate_update({field:value}):
+                raise InvalidField(f'⛔ InvalidField:184 "{field}" is not in the header')
+            raise Exception('⚠️  UnknownError:186 You are not suposed to encounter this message, may report this issue to the developer (RTSDB:188).')
         self._save()
 
     # See **Initiate the database** in the README.md
     def setHeader(self, header):
         if self.header is None:
             self.header = header
         else:
```

### Comparing `RTSDB-1.6/RTSDataBase/exceptions.py` & `RTSDB-1.7/RTSDataBase/exceptions.py`

 * *Files identical despite different names*

### Comparing `RTSDB-1.6/RTSDataBase/typotest.py` & `RTSDB-1.7/RTSDataBase/typotest.py`

 * *Files identical despite different names*

### Comparing `RTSDB-1.6/setup.py` & `RTSDB-1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RTSDB',
-    version='1.6',
+    version='1.7',
     packages=find_packages(),
     description='Create yourself a simple database with this package.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='MIT with required credit to the author.',
```


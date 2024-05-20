# Comparing `tmp/batch-framework-0.2.1.tar.gz` & `tmp/batch-framework-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batch-framework-0.2.1.tar", last modified: Sun May 19 15:20:43 2024, max compression
+gzip compressed data, was "batch-framework-0.2.2.tar", last modified: Sun May 19 15:59:18 2024, max compression
```

## Comparing `batch-framework-0.2.1.tar` & `batch-framework-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:20:43.133230 batch-framework-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-19 15:19:59.000000 batch-framework-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-19 15:20:43.133230 batch-framework-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-19 15:19:59.000000 batch-framework-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:20:43.129230 batch-framework-0.2.1/batch_framework/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/adaptor.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/etl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:20:43.133230 batch-framework-0.2.1/batch_framework/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/filesystem/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:20:43.133230 batch-framework-0.2.1/batch_framework/filesystem/dropbox/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/filesystem/dropbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/filesystem/dropbox/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/filesystem/dropbox/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/filesystem/dropbox/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/filesystem/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/parallize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/rdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:20:43.133230 batch-framework-0.2.1/batch_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-19 15:20:43.000000 batch-framework-0.2.1/batch_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-19 15:20:43.000000 batch-framework-0.2.1/batch_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 15:20:43.000000 batch-framework-0.2.1/batch_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-19 15:20:43.000000 batch-framework-0.2.1/batch_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 15:20:43.000000 batch-framework-0.2.1/batch_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 15:20:43.133230 batch-framework-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-19 15:19:59.000000 batch-framework-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:59:17.998653 batch-framework-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-19 15:58:34.000000 batch-framework-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-19 15:59:17.994653 batch-framework-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-19 15:58:34.000000 batch-framework-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:59:17.990653 batch-framework-0.2.2/batch_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 15:58:34.000000 batch-framework-0.2.2/batch_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-19 15:58:34.000000 batch-framework-0.2.2/batch_framework/adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-19 15:58:34.000000 batch-framework-0.2.2/batch_framework/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-19 15:58:34.000000 batch-framework-0.2.2/batch_framework/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-05-19 15:58:34.000000 batch-framework-0.2.2/batch_framework/etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-19 15:58:34.000000 batch-framework-0.2.2/batch_framework/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:59:17.994653 batch-framework-0.2.2/batch_framework/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-19 15:58:34.000000 batch-framework-0.2.2/batch_framework/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-19 15:58:34.000000 batch-framework-0.2.2/batch_framework/filesystem/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:59:17.994653 batch-framework-0.2.2/batch_framework/filesystem/dropbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-19 15:58:34.000000 batch-framework-0.2.2/batch_framework/filesystem/dropbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-19 15:58:34.000000 batch-framework-0.2.2/batch_framework/filesystem/dropbox/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-05-19 15:58:34.000000 batch-framework-0.2.2/batch_framework/filesystem/dropbox/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-19 15:58:34.000000 batch-framework-0.2.2/batch_framework/filesystem/dropbox/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-19 15:58:34.000000 batch-framework-0.2.2/batch_framework/filesystem/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-05-19 15:58:34.000000 batch-framework-0.2.2/batch_framework/parallize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-19 15:58:34.000000 batch-framework-0.2.2/batch_framework/rdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-19 15:58:34.000000 batch-framework-0.2.2/batch_framework/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 15:58:34.000000 batch-framework-0.2.2/batch_framework/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:59:17.994653 batch-framework-0.2.2/batch_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-19 15:59:17.000000 batch-framework-0.2.2/batch_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-19 15:59:17.000000 batch-framework-0.2.2/batch_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 15:59:17.000000 batch-framework-0.2.2/batch_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-19 15:59:17.000000 batch-framework-0.2.2/batch_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 15:59:17.000000 batch-framework-0.2.2/batch_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 15:59:17.998653 batch-framework-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-19 15:58:34.000000 batch-framework-0.2.2/setup.py
```

### Comparing `batch-framework-0.2.1/LICENSE` & `batch-framework-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.1/PKG-INFO` & `batch-framework-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batch-framework
-Version: 0.2.1
+Version: 0.2.2
 Summary: Generate Batch Framework
 Home-page: https://github.com/jeffrey82221/batch_framework
 Author: jeffreylin
 Author-email: jeffrey82221@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `batch-framework-0.2.1/batch_framework/adaptor.py` & `batch-framework-0.2.2/batch_framework/adaptor.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.1/batch_framework/base.py` & `batch-framework-0.2.2/batch_framework/base.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.1/batch_framework/etl.py` & `batch-framework-0.2.2/batch_framework/etl.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.1/batch_framework/executor.py` & `batch-framework-0.2.2/batch_framework/executor.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.1/batch_framework/filesystem/base.py` & `batch-framework-0.2.2/batch_framework/filesystem/base.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.1/batch_framework/filesystem/dropbox/config.py` & `batch-framework-0.2.2/batch_framework/filesystem/dropbox/config.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.1/batch_framework/filesystem/dropbox/dropbox.py` & `batch-framework-0.2.2/batch_framework/filesystem/dropbox/dropbox.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.1/batch_framework/filesystem/dropbox/util.py` & `batch-framework-0.2.2/batch_framework/filesystem/dropbox/util.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.1/batch_framework/filesystem/local.py` & `batch-framework-0.2.2/batch_framework/filesystem/local.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.1/batch_framework/parallize.py` & `batch-framework-0.2.2/batch_framework/parallize.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.1/batch_framework/rdb.py` & `batch-framework-0.2.2/batch_framework/rdb.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,38 +47,38 @@
         """
         raise NotImplementedError
 
 
 class DuckDBBackend(RDB):
     def __init__(
             self, persist_fs: Optional[FileSystem] = None, db_name: str = ''):
-        if persist_fs:
+        if persist_fs is not None:
             assert db_name != '', 'db_name should be provided when persist_fs is provided'
+            self._lb = LocalBackend('duckdb')
             if persist_fs.check_exists(db_name):
                 # download data to local from remote file system
                 buff = persist_fs.download_core(db_name)
                 buff.seek(0)
-                self._lb = LocalBackend('./duckdb')
                 self._lb.upload_core(buff, self._db_name)
                 assert os.path.exists(
-                    './duckdb/' + db_name), f'db_name: {db_name} does not exist'
+                    'duckdb/' + db_name), f'db_name: {db_name} does not exist'
         self._persist_fs = persist_fs
         super().__init__(db_name)
 
     @property
     def conn(self):
         """
         Get thread local used connection.
         """
         if self._conn is None:
             if self._persist_fs is None:
                 conn = duckdb.connect(database=':memory:')
             else:
                 conn = duckdb.connect(
-                    database='./duckdb/' + self._db_name)
+                    database='duckdb/' + self._db_name)
             self._conn = conn
         return self._conn
 
     def get_conn(self):
         return self.conn.cursor()
 
     def register(self, table_name: str, table: object):
```

### Comparing `batch-framework-0.2.1/batch_framework/storage.py` & `batch-framework-0.2.2/batch_framework/storage.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.1/batch_framework.egg-info/PKG-INFO` & `batch-framework-0.2.2/batch_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batch-framework
-Version: 0.2.1
+Version: 0.2.2
 Summary: Generate Batch Framework
 Home-page: https://github.com/jeffrey82221/batch_framework
 Author: jeffreylin
 Author-email: jeffrey82221@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `batch-framework-0.2.1/batch_framework.egg-info/SOURCES.txt` & `batch-framework-0.2.2/batch_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.1/setup.py` & `batch-framework-0.2.2/setup.py`

 * *Files identical despite different names*


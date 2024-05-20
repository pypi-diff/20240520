# Comparing `tmp/row64tools-1.0.2.tar.gz` & `tmp/row64tools-1.0.3.tar.gz`

## Comparing `row64tools-1.0.2.tar` & `row64tools-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 row64tools-1.0.2/src/row64tools/__init__.py
--rw-r--r--   0        0        0    61937 2020-02-02 00:00:00.000000 row64tools-1.0.2/src/row64tools/bytestream.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 row64tools-1.0.2/src/row64tools/example.ramdb
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 row64tools-1.0.2/src/row64tools/load_example.py
--rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 row64tools-1.0.2/src/row64tools/ramdb.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 row64tools-1.0.2/src/row64tools/save_example.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 row64tools-1.0.2/LICENSE
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 row64tools-1.0.2/README.md
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 row64tools-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 row64tools-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 row64tools-1.0.3/src/row64tools/__init__.py
+-rw-r--r--   0        0        0    61937 2020-02-02 00:00:00.000000 row64tools-1.0.3/src/row64tools/bytestream.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 row64tools-1.0.3/src/row64tools/example.ramdb
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 row64tools-1.0.3/src/row64tools/load_example.py
+-rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 row64tools-1.0.3/src/row64tools/ramdb.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 row64tools-1.0.3/src/row64tools/save_example.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 row64tools-1.0.3/LICENSE
+-rw-r--r--   0        0        0     4808 2020-02-02 00:00:00.000000 row64tools-1.0.3/README.md
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 row64tools-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 row64tools-1.0.3/PKG-INFO
```

### Comparing `row64tools-1.0.2/src/row64tools/bytestream.py` & `row64tools-1.0.3/src/row64tools/bytestream.py`

 * *Files identical despite different names*

### Comparing `row64tools-1.0.2/src/row64tools/example.ramdb` & `row64tools-1.0.3/src/row64tools/example.ramdb`

 * *Files identical despite different names*

### Comparing `row64tools-1.0.2/src/row64tools/load_example.py` & `row64tools-1.0.3/src/row64tools/load_example.py`

 * *Files identical despite different names*

### Comparing `row64tools-1.0.2/src/row64tools/ramdb.py` & `row64tools-1.0.3/src/row64tools/ramdb.py`

 * *Files identical despite different names*

### Comparing `row64tools-1.0.2/src/row64tools/save_example.py` & `row64tools-1.0.3/src/row64tools/save_example.py`

 * *Files identical despite different names*

### Comparing `row64tools-1.0.2/LICENSE` & `row64tools-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `row64tools-1.0.2/README.md` & `row64tools-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,28 +34,27 @@
 row64tools then correctly convert them to dates in your dashboard.
 
 
 Here's an example:
 
 ```
 import pandas as pd
-from ramdb import ramdb
+from row64tools import ramdb
 
 data = {
   "tier": [4, 2, 1],
   "active": [False, True, False],
   "name": ["David", "Mary", "John"],
   "points": [10.5, 6.5, 8.0],
   "sign up": ["09/01/2017","07/14/2022","04/03/2015"]
 }
 df = pd.DataFrame(data)
 df["sign up"] = pd.to_datetime(df["sign up"])
 
-rdb = ramdb()
-rdb.save_from_df(df, "c:\\Temp\\testSave.ramdb")
+ramdb.save_from_df(df, "c:\\Temp\\testSave.ramdb")
 ```
 
 
 Database Connector
 =======
 
 Next lets look at how to save a .ramdb into the Row64 Server on Linux.
```

### Comparing `row64tools-1.0.2/pyproject.toml` & `row64tools-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "row64tools"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Row64", email="info@row64.com" },
 ]
 description = "Tools for the Row64 Platform"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `row64tools-1.0.2/PKG-INFO` & `row64tools-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: row64tools
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tools for the Row64 Platform
 Project-URL: Homepage, https://github.com/Row64/row64tools
 Project-URL: Bug Tracker, https://github.com/Row64/row64tools/issues
 Author-email: Row64 <info@row64.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -49,28 +49,27 @@
 row64tools then correctly convert them to dates in your dashboard.
 
 
 Here's an example:
 
 ```
 import pandas as pd
-from ramdb import ramdb
+from row64tools import ramdb
 
 data = {
   "tier": [4, 2, 1],
   "active": [False, True, False],
   "name": ["David", "Mary", "John"],
   "points": [10.5, 6.5, 8.0],
   "sign up": ["09/01/2017","07/14/2022","04/03/2015"]
 }
 df = pd.DataFrame(data)
 df["sign up"] = pd.to_datetime(df["sign up"])
 
-rdb = ramdb()
-rdb.save_from_df(df, "c:\\Temp\\testSave.ramdb")
+ramdb.save_from_df(df, "c:\\Temp\\testSave.ramdb")
 ```
 
 
 Database Connector
 =======
 
 Next lets look at how to save a .ramdb into the Row64 Server on Linux.
```


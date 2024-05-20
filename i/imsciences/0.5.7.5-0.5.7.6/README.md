# Comparing `tmp/imsciences-0.5.7.5.tar.gz` & `tmp/imsciences-0.5.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.7.5.tar", last modified: Mon May 20 11:00:26 2024, max compression
+gzip compressed data, was "imsciences-0.5.7.6.tar", last modified: Mon May 20 11:58:06 2024, max compression
```

## Comparing `imsciences-0.5.7.5.tar` & `imsciences-0.5.7.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 11:00:26.335571 imsciences-0.5.7.5/
--rw-rw-rw-   0        0        0     9976 2024-05-20 11:00:26.329520 imsciences-0.5.7.5/PKG-INFO
--rw-rw-rw-   0        0        0     9471 2024-05-17 09:27:28.000000 imsciences-0.5.7.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 11:00:26.294531 imsciences-0.5.7.5/imsciences/
--rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.7.5/imsciences/__init__.py
--rw-rw-rw-   0        0        0    80106 2024-05-20 11:00:16.000000 imsciences-0.5.7.5/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-20 11:00:26.327519 imsciences-0.5.7.5/imsciences.egg-info/
--rw-rw-rw-   0        0        0     9976 2024-05-20 11:00:26.000000 imsciences-0.5.7.5/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-20 11:00:26.000000 imsciences-0.5.7.5/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 11:00:26.000000 imsciences-0.5.7.5/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-20 11:00:26.000000 imsciences-0.5.7.5/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-20 11:00:26.000000 imsciences-0.5.7.5/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 11:00:26.336535 imsciences-0.5.7.5/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-20 11:00:15.000000 imsciences-0.5.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:58:06.148142 imsciences-0.5.7.6/
+-rw-rw-rw-   0        0        0     9976 2024-05-20 11:58:06.143152 imsciences-0.5.7.6/PKG-INFO
+-rw-rw-rw-   0        0        0     9471 2024-05-17 09:27:28.000000 imsciences-0.5.7.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 11:58:06.094948 imsciences-0.5.7.6/imsciences/
+-rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.7.6/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    80097 2024-05-20 11:57:51.000000 imsciences-0.5.7.6/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:58:06.140132 imsciences-0.5.7.6/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     9976 2024-05-20 11:58:05.000000 imsciences-0.5.7.6/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-20 11:58:05.000000 imsciences-0.5.7.6/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 11:58:05.000000 imsciences-0.5.7.6/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-20 11:58:05.000000 imsciences-0.5.7.6/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-20 11:58:05.000000 imsciences-0.5.7.6/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 11:58:06.148142 imsciences-0.5.7.6/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-20 11:58:00.000000 imsciences-0.5.7.6/setup.py
```

### Comparing `imsciences-0.5.7.5/PKG-INFO` & `imsciences-0.5.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.7.5
+Version: 0.5.7.6
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.7.5/README.md` & `imsciences-0.5.7.6/README.md`

 * *Files identical despite different names*

### Comparing `imsciences-0.5.7.5/imsciences/datafunctions.py` & `imsciences-0.5.7.6/imsciences/datafunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1175,15 +1175,15 @@
         print("\n1. pull_fred_data")
         print("   - Description: Get data from FRED by using series id tokens.")
         print("   - Usage: pull_fred_data(week_commencing, series_id_list)")
         print("   - Example: pull_fred_data('sun', ['GPDIC1', 'Y057RX1Q020SBEA', 'GCEC1', 'ND000333Q', 'Y006RX1Q020SBEA'])")
     
     ###############################################################  MACRO ##########################################################################
 
-    def pull_fred_data(self, week_commencing: str = 'sun', series_id_list: list[str] = ["GPDIC1", "Y057RX1Q020SBEA", "GCEC1", "ND000333Q", "Y006RX1Q020SBEA"]) -> pd.DataFrame:
+    def pull_fred_data(self, week_commencing: str = 'mon', series_id_list: list[str] = ["GPDIC1", "Y057RX1Q020SBEA", "GCEC1", "ND000333Q", "Y006RX1Q020SBEA"]) -> pd.DataFrame:
         '''
         Parameters
         ----------
         week_commencing : str
             specify the day for the week commencing, the default is 'sun' (e.g., 'mon', 'tue', 'wed', 'thu', 'fri', 'sat', 'sun')
 
         series_id_list : list[str]
@@ -1205,15 +1205,15 @@
         # Fetch the metadata for each series to get the full names
         series_names = {series_id: fred.get_series_info(series_id).title for series_id in series_id_list}
 
         # Download data from series id list
         fred_series = {series_id: fred.get_series(series_id) for series_id in series_id_list}
 
         # Data processing
-        date_range = {'OBS': pd.date_range("1950-01-01", datetime.datetime.today().strftime('%Y-%m-%d'), freq='d')}
+        date_range = {'OBS': pd.date_range("1950-01-01", datetime.today().strftime('%Y-%m-%d'), freq='d')}
         fred_series_df = pd.DataFrame(date_range)
 
         for series_id, series_data in fred_series.items():
             series_data = series_data.reset_index()
             series_data.columns = ['OBS', series_names[series_id]]  # Use the series name as the column header
             fred_series_df = pd.merge_asof(fred_series_df, series_data, on='OBS', direction='backward')
```

### Comparing `imsciences-0.5.7.5/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.7.6/imsciences.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.7.5
+Version: 0.5.7.6
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.7.5/setup.py` & `imsciences-0.5.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.7.5'
+VERSION = '0.5.7.6'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```

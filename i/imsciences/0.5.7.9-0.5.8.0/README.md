# Comparing `tmp/imsciences-0.5.7.9.tar.gz` & `tmp/imsciences-0.5.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.7.9.tar", last modified: Mon May 20 12:23:03 2024, max compression
+gzip compressed data, was "imsciences-0.5.8.0.tar", last modified: Mon May 20 12:24:57 2024, max compression
```

## Comparing `imsciences-0.5.7.9.tar` & `imsciences-0.5.8.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 12:23:03.717345 imsciences-0.5.7.9/
--rw-rw-rw-   0        0        0     9976 2024-05-20 12:23:03.710341 imsciences-0.5.7.9/PKG-INFO
--rw-rw-rw-   0        0        0     9471 2024-05-17 09:27:28.000000 imsciences-0.5.7.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 12:23:03.661793 imsciences-0.5.7.9/imsciences/
--rw-rw-rw-   0        0        0       78 2024-05-20 12:19:37.000000 imsciences-0.5.7.9/imsciences/__init__.py
--rw-rw-rw-   0        0        0    80090 2024-05-20 12:22:54.000000 imsciences-0.5.7.9/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-20 12:23:03.705340 imsciences-0.5.7.9/imsciences.egg-info/
--rw-rw-rw-   0        0        0     9976 2024-05-20 12:23:03.000000 imsciences-0.5.7.9/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-20 12:23:03.000000 imsciences-0.5.7.9/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 12:23:03.000000 imsciences-0.5.7.9/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-20 12:23:03.000000 imsciences-0.5.7.9/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-20 12:23:03.000000 imsciences-0.5.7.9/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 12:23:03.718337 imsciences-0.5.7.9/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-20 12:22:57.000000 imsciences-0.5.7.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:24:57.703160 imsciences-0.5.8.0/
+-rw-rw-rw-   0        0        0     9976 2024-05-20 12:24:57.698160 imsciences-0.5.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9471 2024-05-17 09:27:28.000000 imsciences-0.5.8.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 12:24:57.665553 imsciences-0.5.8.0/imsciences/
+-rw-rw-rw-   0        0        0       78 2024-05-20 12:19:37.000000 imsciences-0.5.8.0/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    80235 2024-05-20 12:24:50.000000 imsciences-0.5.8.0/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:24:57.695159 imsciences-0.5.8.0/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     9976 2024-05-20 12:24:57.000000 imsciences-0.5.8.0/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-20 12:24:57.000000 imsciences-0.5.8.0/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 12:24:57.000000 imsciences-0.5.8.0/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-20 12:24:57.000000 imsciences-0.5.8.0/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-20 12:24:57.000000 imsciences-0.5.8.0/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 12:24:57.704163 imsciences-0.5.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-20 12:24:34.000000 imsciences-0.5.8.0/setup.py
```

### Comparing `imsciences-0.5.7.9/PKG-INFO` & `imsciences-0.5.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.7.9
+Version: 0.5.8.0
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.7.9/README.md` & `imsciences-0.5.8.0/README.md`

 * *Files identical despite different names*

### Comparing `imsciences-0.5.7.9/imsciences/datafunctions.py` & `imsciences-0.5.8.0/imsciences/datafunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1223,15 +1223,16 @@
                 fred_series_df[base_col] = fred_series_df[col].combine_first(fred_series_df[base_col + '_y'])
                 fred_series_df.drop([col, base_col + '_y'], axis=1, inplace=True)
 
         # Ensure sum_columns are present in the DataFrame
         sum_columns = [series_names[series_id] for series_id in series_id_list if series_names[series_id] in fred_series_df.columns]
 
         # Aggregate results by week
-        fred_df_final = dataprocessing.aggregate_daily_to_wc_wide(df=fred_series_df, 
+        fred_df_final = dataprocessing.aggregate_daily_to_wc_wide(self,
+                                                                  df=fred_series_df, 
                                                     date_column="OBS", 
                                                     group_columns=[], 
                                                     sum_columns=sum_columns,
                                                     wc=week_commencing,
                                                     aggregation="average")
 
         # Remove anything after the instance of any ':' in the column names and rename, except for 'OBS'
@@ -1380,15 +1381,16 @@
         for col in value_columns:
             if col in daily_df.columns:
                 daily_df[col] = pd.to_numeric(daily_df[col], errors='coerce').fillna(0)
             else:
                 print(f"Column {col} not found in daily_df")
         
         # Aggregate results by week
-        ons_df_final = dataprocessing.aggregate_daily_to_wc_wide(df=daily_df, 
+        ons_df_final = dataprocessing.aggregate_daily_to_wc_wide(self,
+                                                                 df=daily_df, 
                                                     date_column="OBS", 
                                                     group_columns=[], 
                                                     sum_columns=value_columns,
                                                     wc=week_commencing,
                                                     aggregation="average")
         
         return ons_df_final
```

### Comparing `imsciences-0.5.7.9/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.8.0/imsciences.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.7.9
+Version: 0.5.8.0
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.7.9/setup.py` & `imsciences-0.5.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.7.9'
+VERSION = '0.5.8.0'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```


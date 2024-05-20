# Comparing `tmp/imsciences-0.5.7.1.tar.gz` & `tmp/imsciences-0.5.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.7.1.tar", last modified: Fri May 17 13:25:31 2024, max compression
+gzip compressed data, was "imsciences-0.5.7.2.tar", last modified: Mon May 20 08:54:59 2024, max compression
```

## Comparing `imsciences-0.5.7.1.tar` & `imsciences-0.5.7.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 13:25:31.874873 imsciences-0.5.7.1/
--rw-rw-rw-   0        0        0     9976 2024-05-17 13:25:31.868672 imsciences-0.5.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     9471 2024-05-17 09:27:28.000000 imsciences-0.5.7.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 13:25:31.812502 imsciences-0.5.7.1/imsciences/
--rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.7.1/imsciences/__init__.py
--rw-rw-rw-   0        0        0    80082 2024-05-17 13:25:03.000000 imsciences-0.5.7.1/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:25:31.864677 imsciences-0.5.7.1/imsciences.egg-info/
--rw-rw-rw-   0        0        0     9976 2024-05-17 13:25:31.000000 imsciences-0.5.7.1/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-17 13:25:31.000000 imsciences-0.5.7.1/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 13:25:31.000000 imsciences-0.5.7.1/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-17 13:25:31.000000 imsciences-0.5.7.1/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-17 13:25:31.000000 imsciences-0.5.7.1/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 13:25:31.875872 imsciences-0.5.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-17 13:24:37.000000 imsciences-0.5.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:54:59.552180 imsciences-0.5.7.2/
+-rw-rw-rw-   0        0        0     9976 2024-05-20 08:54:59.547178 imsciences-0.5.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9471 2024-05-17 09:27:28.000000 imsciences-0.5.7.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 08:54:59.401519 imsciences-0.5.7.2/imsciences/
+-rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.7.2/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    79911 2024-05-20 08:54:30.000000 imsciences-0.5.7.2/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:54:59.542181 imsciences-0.5.7.2/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     9976 2024-05-20 08:54:59.000000 imsciences-0.5.7.2/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-20 08:54:59.000000 imsciences-0.5.7.2/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 08:54:59.000000 imsciences-0.5.7.2/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-20 08:54:59.000000 imsciences-0.5.7.2/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-20 08:54:59.000000 imsciences-0.5.7.2/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 08:54:59.553180 imsciences-0.5.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-20 08:54:57.000000 imsciences-0.5.7.2/setup.py
```

### Comparing `imsciences-0.5.7.1/PKG-INFO` & `imsciences-0.5.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.7.1
+Version: 0.5.7.2
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.7.1/README.md` & `imsciences-0.5.7.2/README.md`

 * *Files identical despite different names*

### Comparing `imsciences-0.5.7.1/imsciences/datafunctions.py` & `imsciences-0.5.7.2/imsciences/datafunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,16 @@
         print("\n10. exclude_rows")
         print("    - Description: Removes rows from a DataFrame based on whether the values in a specified column are not in a provided list.")
         print("    - Usage: exclude_rows(df, col_to_filter, list_of_filters)")
         print("    - Example: exclude_rows(df, 'week', ['2022-W20', '2022-W21'])")
 
         print("\n11. rename_cols")
         print("    - Description: Renames columns in a pandas DataFrame.")
-        print("    - Usage: rename_cols(df, cols_to_rename)")
-        print("    - Example: rename_cols(df, {'old_col_name': 'new_col_name'})")
+        print("    - Usage: rename_cols(df, name)")
+        print("    - Example: rename_cols(df, 'ame_facebook'")
 
         print("\n12. merge_new_and_old")
         print("    - Description: Creates a new DataFrame with two columns: one for dates and one for merged numeric values.")
         print("    - Merges numeric values from specified columns in the old and new DataFrames based on a given cutoff date.")
         print("    - Usage: merge_new_and_old(old_df, old_col, new_df, new_col, cutoff_date, date_col_name='OBS')")
         print("    - Example: merge_new_and_old(df1, 'old_col', df2, 'new_col', '2023-01-15')")
 
@@ -443,30 +443,23 @@
         df['OBS'] = df[week_col].apply(lambda x: week_to_startdate(x, start_day)).dt.strftime('%d/%m/%Y')
         return df
     
     def exclude_rows(self, df, col_to_filter, list_of_filters):
         # This line filters the DataFrame based on whether the values in the specified column are not in the list_of_filters
         return df[~df[col_to_filter].isin(list_of_filters)]
     
-    def rename_cols(self, df, cols_to_rename):
-        """
-        Renames columns in a pandas DataFrame.
-
-        Parameters:
-        - df: pandas DataFrame
-            The DataFrame whose columns are to be renamed.
-        - cols_to_rename: dict
-            A dictionary where keys are the current column names and values are the new column names.
-
-        Returns:
-        - pandas DataFrame
-            The DataFrame with renamed columns.
-        """
-        
-        return df.rename(columns=cols_to_rename)
+    def rename_cols(self, df, name = 'ame_'):
+        new_columns = {}
+        for col in df.columns:
+            if col != 'OBS':
+                new_col_name = name + col.replace(" ", "_").lower()
+            else:
+                new_col_name = col
+            new_columns[col] = new_col_name
+        return df.rename(columns=new_columns)
     
     def merge_new_and_old(self, old_df, old_col, new_df, new_col, cutoff_date, date_col_name='OBS'):
         """
         Creates a new DataFrame with two columns: one for dates and one for merged numeric values.
         Merges numeric values from specified columns in the old and new DataFrames based on a given cutoff date.
 
         Parameters:
@@ -1211,15 +1204,15 @@
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
 
@@ -1237,16 +1230,16 @@
         fred_df_final = dataprocessing.aggregate_daily_to_wc_wide(df=fred_series_df, 
                                                     date_column="OBS", 
                                                     group_columns=[], 
                                                     sum_columns=sum_columns,
                                                     wc=week_commencing,
                                                     aggregation="average")
 
-        # Remove anything after the instance of any ':' in the column names and rename
-        fred_df_final.columns = ['macro_' + col.lower().split(':')[0].replace(' ', '_') for col in fred_df_final.columns]
+        # Remove anything after the instance of any ':' in the column names and rename, except for 'OBS'
+        fred_df_final.columns = ['OBS' if col == 'OBS' else 'macro_' + col.lower().split(':')[0].replace(' ', '_') for col in fred_df_final.columns]
 
         return fred_df_final
     
     def pull_boe_data(self, week_commencing="mon", max_retries=30, delay=5):
         """
         Fetch and process Bank of England interest rate data.
```

### Comparing `imsciences-0.5.7.1/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.7.2/imsciences.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.7.1
+Version: 0.5.7.2
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.7.1/setup.py` & `imsciences-0.5.7.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.7.1'
+VERSION = '0.5.7.2'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```


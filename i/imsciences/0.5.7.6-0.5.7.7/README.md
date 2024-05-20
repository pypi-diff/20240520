# Comparing `tmp/imsciences-0.5.7.6.tar.gz` & `tmp/imsciences-0.5.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.7.6.tar", last modified: Mon May 20 11:58:06 2024, max compression
+gzip compressed data, was "imsciences-0.5.7.7.tar", last modified: Mon May 20 12:03:20 2024, max compression
```

## Comparing `imsciences-0.5.7.6.tar` & `imsciences-0.5.7.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 11:58:06.148142 imsciences-0.5.7.6/
--rw-rw-rw-   0        0        0     9976 2024-05-20 11:58:06.143152 imsciences-0.5.7.6/PKG-INFO
--rw-rw-rw-   0        0        0     9471 2024-05-17 09:27:28.000000 imsciences-0.5.7.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 11:58:06.094948 imsciences-0.5.7.6/imsciences/
--rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.7.6/imsciences/__init__.py
--rw-rw-rw-   0        0        0    80097 2024-05-20 11:57:51.000000 imsciences-0.5.7.6/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-20 11:58:06.140132 imsciences-0.5.7.6/imsciences.egg-info/
--rw-rw-rw-   0        0        0     9976 2024-05-20 11:58:05.000000 imsciences-0.5.7.6/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-20 11:58:05.000000 imsciences-0.5.7.6/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 11:58:05.000000 imsciences-0.5.7.6/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-20 11:58:05.000000 imsciences-0.5.7.6/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-20 11:58:05.000000 imsciences-0.5.7.6/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 11:58:06.148142 imsciences-0.5.7.6/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-20 11:58:00.000000 imsciences-0.5.7.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:03:20.351593 imsciences-0.5.7.7/
+-rw-rw-rw-   0        0        0     9976 2024-05-20 12:03:20.343584 imsciences-0.5.7.7/PKG-INFO
+-rw-rw-rw-   0        0        0     9471 2024-05-17 09:27:28.000000 imsciences-0.5.7.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 12:03:20.297227 imsciences-0.5.7.7/imsciences/
+-rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.7.7/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    80100 2024-05-20 12:03:01.000000 imsciences-0.5.7.7/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:03:20.339586 imsciences-0.5.7.7/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     9976 2024-05-20 12:03:20.000000 imsciences-0.5.7.7/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-20 12:03:20.000000 imsciences-0.5.7.7/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 12:03:20.000000 imsciences-0.5.7.7/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-20 12:03:20.000000 imsciences-0.5.7.7/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-20 12:03:20.000000 imsciences-0.5.7.7/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 12:03:20.353000 imsciences-0.5.7.7/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-20 12:03:16.000000 imsciences-0.5.7.7/setup.py
```

### Comparing `imsciences-0.5.7.6/PKG-INFO` & `imsciences-0.5.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.7.6
+Version: 0.5.7.7
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.7.6/README.md` & `imsciences-0.5.7.7/README.md`

 * *Files identical despite different names*

### Comparing `imsciences-0.5.7.6/imsciences/datafunctions.py` & `imsciences-0.5.7.7/imsciences/datafunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1224,15 +1224,15 @@
                 fred_series_df[base_col] = fred_series_df[col].combine_first(fred_series_df[base_col + '_y'])
                 fred_series_df.drop([col, base_col + '_y'], axis=1, inplace=True)
 
         # Ensure sum_columns are present in the DataFrame
         sum_columns = [series_names[series_id] for series_id in series_id_list if series_names[series_id] in fred_series_df.columns]
 
         # Aggregate results by week
-        fred_df_final = dataprocessing.aggregate_daily_to_wc_wide(df=fred_series_df, 
+        fred_df_final = dataprocessing.aggregate_daily_to_wc_wide(self, df=fred_series_df, 
                                                     date_column="OBS", 
                                                     group_columns=[], 
                                                     sum_columns=sum_columns,
                                                     wc=week_commencing,
                                                     aggregation="average")
 
         # Remove anything after the instance of any ':' in the column names and rename, except for 'OBS'
@@ -1280,15 +1280,15 @@
         df.rename(columns={"Date Changed": "OBS", "Rate": "macro_boe_intr_rate"}, inplace=True)
         
         # Change date column to datetime and find the corresponding week to the date
         df["OBS"] = pd.to_datetime(df["OBS"], format="%d %b %y")
         df.sort_values("OBS", axis=0, inplace=True)
         
         # Create a daily date range and find the week commencing for that day
-        date_range = pd.date_range(df["OBS"].iloc[0], datetime.datetime.today(), freq="d")
+        date_range = pd.date_range(df["OBS"].iloc[0], datetime.today(), freq="d")
         df_daily = pd.DataFrame(date_range, columns=["OBS"])
         
         # Adjust each date to the specified week commencing day
         df_daily['Week_Commencing'] = df_daily["OBS"].apply(lambda x: x - pd.Timedelta(days=(x.weekday() - day_dict[week_commencing]) % 7))
         
         # Outer merge the daily date range on the boe dataframe and forward fill in the blanks
         df_final = df_daily.merge(df, on='OBS', how="left")
@@ -1381,15 +1381,15 @@
         for col in value_columns:
             if col in daily_df.columns:
                 daily_df[col] = pd.to_numeric(daily_df[col], errors='coerce').fillna(0)
             else:
                 print(f"Column {col} not found in daily_df")
         
         # Aggregate results by week
-        ons_df_final = dataprocessing.aggregate_daily_to_wc_wide(df=daily_df, 
+        ons_df_final = dataprocessing.aggregate_daily_to_wc_wide(self, df=daily_df, 
                                                     date_column="OBS", 
                                                     group_columns=[], 
                                                     sum_columns=value_columns,
                                                     wc=week_commencing,
                                                     aggregation="average")
         
         return ons_df_final
```

### Comparing `imsciences-0.5.7.6/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.7.7/imsciences.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.7.6
+Version: 0.5.7.7
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.7.6/setup.py` & `imsciences-0.5.7.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.7.6'
+VERSION = '0.5.7.7'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```


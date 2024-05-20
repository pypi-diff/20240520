# Comparing `tmp/imsciences-0.5.7.3.tar.gz` & `tmp/imsciences-0.5.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.7.3.tar", last modified: Mon May 20 09:09:06 2024, max compression
+gzip compressed data, was "imsciences-0.5.7.4.tar", last modified: Mon May 20 09:18:43 2024, max compression
```

## Comparing `imsciences-0.5.7.3.tar` & `imsciences-0.5.7.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 09:09:06.848592 imsciences-0.5.7.3/
--rw-rw-rw-   0        0        0     9976 2024-05-20 09:09:06.841265 imsciences-0.5.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     9471 2024-05-17 09:27:28.000000 imsciences-0.5.7.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 09:09:06.778569 imsciences-0.5.7.3/imsciences/
--rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.7.3/imsciences/__init__.py
--rw-rw-rw-   0        0        0    79906 2024-05-20 09:08:47.000000 imsciences-0.5.7.3/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-20 09:09:06.837275 imsciences-0.5.7.3/imsciences.egg-info/
--rw-rw-rw-   0        0        0     9976 2024-05-20 09:09:06.000000 imsciences-0.5.7.3/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-20 09:09:06.000000 imsciences-0.5.7.3/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 09:09:06.000000 imsciences-0.5.7.3/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-20 09:09:06.000000 imsciences-0.5.7.3/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-20 09:09:06.000000 imsciences-0.5.7.3/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 09:09:06.849539 imsciences-0.5.7.3/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-20 09:08:57.000000 imsciences-0.5.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:18:43.965733 imsciences-0.5.7.4/
+-rw-rw-rw-   0        0        0     9976 2024-05-20 09:18:43.960734 imsciences-0.5.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9471 2024-05-17 09:27:28.000000 imsciences-0.5.7.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 09:18:43.887386 imsciences-0.5.7.4/imsciences/
+-rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.7.4/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    80066 2024-05-20 09:18:20.000000 imsciences-0.5.7.4/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:18:43.954421 imsciences-0.5.7.4/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     9976 2024-05-20 09:18:43.000000 imsciences-0.5.7.4/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-20 09:18:43.000000 imsciences-0.5.7.4/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 09:18:43.000000 imsciences-0.5.7.4/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-20 09:18:43.000000 imsciences-0.5.7.4/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-20 09:18:43.000000 imsciences-0.5.7.4/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 09:18:43.966732 imsciences-0.5.7.4/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-20 09:18:40.000000 imsciences-0.5.7.4/setup.py
```

### Comparing `imsciences-0.5.7.3/PKG-INFO` & `imsciences-0.5.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.7.3
+Version: 0.5.7.4
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.7.3/README.md` & `imsciences-0.5.7.4/README.md`

 * *Files identical despite different names*

### Comparing `imsciences-0.5.7.3/imsciences/datafunctions.py` & `imsciences-0.5.7.4/imsciences/datafunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1242,15 +1242,15 @@
     def pull_boe_data(self, week_commencing="mon", max_retries=30, delay=5):
         """
         Fetch and process Bank of England interest rate data.
 
         Args:
             week_commencing (str): The starting day of the week for aggregation. 
                                 Options are "mon", "tue", "wed", "thur", "fri", "sat", "sun". 
-                                Default is "mon".
+                                Default is "sun".
             max_retries (int): Maximum number of retries to fetch data in case of failure. Default is 30.
             delay (int): Delay in seconds between retry attempts. Default is 5.
 
         Returns:
             pd.DataFrame: A DataFrame with weekly aggregated Bank of England interest rates. 
                         The 'OBS' column contains the week commencing dates in 'dd/mm/yyyy' format 
                         and 'macro_boe_intr_rate' contains the average interest rate for the week.
@@ -1282,25 +1282,26 @@
         df["OBS"] = pd.to_datetime(df["OBS"], format="%d %b %y")
         df.sort_values("OBS", axis=0, inplace=True)
         
         # Create a daily date range and find the week commencing for that day
         date_range = pd.date_range(df["OBS"].iloc[0], datetime.datetime.today(), freq="d")
         df_daily = pd.DataFrame(date_range, columns=["OBS"])
         
-        # Find the start of the week for each day
-        df_daily['OBS'] = df_daily["OBS"].apply(lambda x: x - pd.Timedelta(days=(x.weekday() - day_dict[week_commencing]) % 7))
+        # Adjust each date to the specified week commencing day
+        df_daily['Week_Commencing'] = df_daily["OBS"].apply(lambda x: x - pd.Timedelta(days=(x.weekday() - day_dict[week_commencing]) % 7))
         
         # Outer merge the daily date range on the boe dataframe and forward fill in the blanks
         df_final = df_daily.merge(df, on='OBS', how="left")
-        df_final.ffill(inplace=True)
+        df_final["macro_boe_intr_rate"].ffill(inplace=True)
         
         # Group by the week start date and get the mean of the interest rates for each week
-        df_final = df_final.groupby('OBS')['macro_boe_intr_rate'].mean().reset_index()
+        df_final = df_final.groupby('Week_Commencing')['macro_boe_intr_rate'].mean().reset_index()
         
-        df_final['OBS'] = df_final['OBS'].dt.strftime('%d/%m/%Y')
+        df_final['Week_Commencing'] = df_final['Week_Commencing'].dt.strftime('%d/%m/%Y')
+        df_final.rename(columns={'Week_Commencing': 'OBS'}, inplace=True)
         
         return df_final
 
     def pull_ons_data(self, series_list, week_commencing):
         """
         Fetch and process time series data from the ONS API.
```

### Comparing `imsciences-0.5.7.3/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.7.4/imsciences.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.7.3
+Version: 0.5.7.4
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.7.3/setup.py` & `imsciences-0.5.7.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.7.3'
+VERSION = '0.5.7.4'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```


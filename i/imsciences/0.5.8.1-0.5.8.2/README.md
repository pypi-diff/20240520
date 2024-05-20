# Comparing `tmp/imsciences-0.5.8.1.tar.gz` & `tmp/imsciences-0.5.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.8.1.tar", last modified: Mon May 20 12:29:34 2024, max compression
+gzip compressed data, was "imsciences-0.5.8.2.tar", last modified: Mon May 20 13:27:20 2024, max compression
```

## Comparing `imsciences-0.5.8.1.tar` & `imsciences-0.5.8.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 12:29:34.523401 imsciences-0.5.8.1/
--rw-rw-rw-   0        0        0     9976 2024-05-20 12:29:34.516400 imsciences-0.5.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     9471 2024-05-17 09:27:28.000000 imsciences-0.5.8.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 12:29:34.452379 imsciences-0.5.8.1/imsciences/
--rw-rw-rw-   0        0        0       78 2024-05-20 12:19:37.000000 imsciences-0.5.8.1/imsciences/__init__.py
--rw-rw-rw-   0        0        0    80113 2024-05-20 12:29:26.000000 imsciences-0.5.8.1/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-20 12:29:34.511385 imsciences-0.5.8.1/imsciences.egg-info/
--rw-rw-rw-   0        0        0     9976 2024-05-20 12:29:34.000000 imsciences-0.5.8.1/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-20 12:29:34.000000 imsciences-0.5.8.1/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 12:29:34.000000 imsciences-0.5.8.1/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-20 12:29:34.000000 imsciences-0.5.8.1/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-20 12:29:34.000000 imsciences-0.5.8.1/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 12:29:34.524403 imsciences-0.5.8.1/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-20 12:29:30.000000 imsciences-0.5.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 13:27:20.884457 imsciences-0.5.8.2/
+-rw-rw-rw-   0        0        0     9976 2024-05-20 13:27:20.875454 imsciences-0.5.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9471 2024-05-17 09:27:28.000000 imsciences-0.5.8.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 13:27:20.811446 imsciences-0.5.8.2/imsciences/
+-rw-rw-rw-   0        0        0       78 2024-05-20 13:24:02.000000 imsciences-0.5.8.2/imsciences/__init__.py
+-rw-rw-rw-   0        0        0   103192 2024-05-20 13:26:39.000000 imsciences-0.5.8.2/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-20 13:27:20.869445 imsciences-0.5.8.2/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     9976 2024-05-20 13:27:20.000000 imsciences-0.5.8.2/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-20 13:27:20.000000 imsciences-0.5.8.2/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 13:27:20.000000 imsciences-0.5.8.2/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-20 13:27:20.000000 imsciences-0.5.8.2/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-20 13:27:20.000000 imsciences-0.5.8.2/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 13:27:20.885967 imsciences-0.5.8.2/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-20 13:27:11.000000 imsciences-0.5.8.2/setup.py
```

### Comparing `imsciences-0.5.8.1/PKG-INFO` & `imsciences-0.5.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.8.1
+Version: 0.5.8.2
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.8.1/README.md` & `imsciences-0.5.8.2/README.md`

 * *Files identical despite different names*

### Comparing `imsciences-0.5.8.1/imsciences/datafunctions.py` & `imsciences-0.5.8.2/imsciences/datafunctions.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import datetime
 import re
 import pandas as pd
 from imsciences import *
 from fredapi import Fred
 import time
 from datetime import datetime
+from cif import cif
+from datetime import timedelta
 
 class dataprocessing:
     
     def help(self):
         print("This is the help section. The functions in the package are as follows:")
 
         print("\n1. get_wd_levels")
@@ -1313,14 +1315,22 @@
             week_commencing (str): The starting day of the week for aggregation. 
                                 Options are "mon", "tue", "wed", "thur", "fri", "sat", "sun".
 
         Returns:
             pd.DataFrame: A DataFrame with weekly aggregated ONS data. The 'OBS' column contains the week 
                         commencing dates and other columns contain the aggregated time series values.
         """ 
+        
+        def parse_quarter(date_str):
+            """Parses a string in 'YYYY Q#' format into a datetime object."""
+            year, quarter = date_str.split(' ')
+            quarter_number = int(quarter[1])
+            month = (quarter_number - 1) * 3 + 1
+            return pd.Timestamp(f"{year}-{month:02d}-01")
+
         # Generate a date range from 1950-01-01 to today
         date_range = pd.date_range(start="1950-01-01", end=datetime.today(), freq='D')
         daily_df = pd.DataFrame(date_range, columns=['OBS'])
         
         # Keep track of the renamed value columns
         value_columns = []
 
@@ -1358,15 +1368,15 @@
             
             # Create a DataFrame from the time series data
             df = pd.DataFrame(time_series_data)
             
             # Handle different frequencies in the data
             if 'date' in df.columns:
                 if any(df['date'].str.contains('Q')):  
-                    df['date'] = pd.PeriodIndex(df['date'], freq='Q').to_timestamp()
+                    df['date'] = df['date'].apply(parse_quarter)
                 else:  
                     df['date'] = pd.to_datetime(df['date'])
             
             df = df.rename(columns={'date': 'OBS', 'value': series_name})
             
             # Rename the value column
             new_col_name = 'macro_' + series_name.lower().replace(':', '').replace(' ', '_').replace('-', '_')
@@ -1391,14 +1401,401 @@
                                                     group_columns=[], 
                                                     sum_columns=value_columns,
                                                     wc=week_commencing,
                                                     aggregation="average")
         
         return ons_df_final
     
+    def pull_macro(self, country : str = "GBR", week_commencing : str = "mon"):
+        
+        # Change country input to list
+        countries_list = [country]
+        
+        # Check if the data wants to be inputted at any other week commencing date
+        day_dict = {"mon" : 0, "tue" : 1, "wed" : 2, "thur" : 3, "fri" : 4, "sat" : 5, "sun" : 6}
+        
+        # Two useful functions for quarterly data
+        # Define a function to get quarterly data
+        def get_quarter(p_date: datetime.date) -> int:
+            return (p_date.month - 1) // 3 + 1
+
+        # Define a function to get the last day of the quarter
+        def get_last_day_of_the_quarter(p_date: datetime.date):
+            quarter = get_quarter(p_date)
+            return datetime.datetime(p_date.year + 3 * quarter // 12, 3 * quarter % 12 + 1, 1) + datetime.timedelta(days=-1)
+        
+        # For the monthly data
+        data_M, subjects_M, measures_M = cif.createDataFrameFromOECD(countries = countries_list, dsname = 'MEI',subject = ['LCEAMN01',
+                                                                                                                    'LCEAPR',
+                                                                                                                    'CSCICP03',
+                                                                                                                    'CPALTT01',
+                                                                                                                    'LRHUTTTT',
+                                                                                                                    'LORSGPRT',
+                                                                                                                    'IR3TIB01',     
+                                                                                                                    'PRINTO01'],
+                                                                measure = ['IXOBSA','IXNSA','IXNB','STSA','ST','GPSA','GY'],
+                                                                    frequency = 'M', startDate = '2015-01')
+        data_M = data_M.stack(level=[0,-1,-2]).reset_index()
+
+        data_Q, subjects_Q, measures_Q = cif.createDataFrameFromOECD(countries = countries_list, dsname = 'MEI',subject = ['LCEAMN01',
+                                                                                                                    'LCEAPR',
+                                                                                                                    'CSCICP03',
+                                                                                                                    'CPALTT01',
+                                                                                                                    'LRHUTTTT',
+                                                                                                                    'LORSGPRT',
+                                                                                                                    'IR3TIB01',
+                                                                                                                    'PRINTO01'],
+                                                                measure = ['IXOBSA','IXNSA','IXNB','STSA','ST','GPSA','GY'], frequency = 'Q',startDate = '2015-01')
+
+        data_Q=data_Q.stack(level=[0,-1,-2]).reset_index()
+
+        # create a data frame dictionary to store your monthly data frames
+        DataFrameDict_M = {elem : pd.DataFrame() for elem in countries_list}
+        for key in DataFrameDict_M.keys():
+            DataFrameDict_M[key] = data_M[:][data_M.country == key]
+
+        # create a data frame dictionary to store your quarterly data frames
+        DataFrameDict_Q = {elem : pd.DataFrame() for elem in countries_list}
+        for key in DataFrameDict_Q.keys():
+            DataFrameDict_Q[key] = data_Q[:][data_Q.country == key]
+
+        # Create a monthly list of the dataframes to iterate through
+        countries_df_list_M = []
+        for i in countries_list:
+            df = pd.DataFrame(DataFrameDict_M[i])
+            df.rename(columns={0:'Values'},inplace=True)
+            df = pd.pivot_table(data=df,index='time',values='Values',columns=['subject','measure'])
+            countries_df_list_M.append(df)
+
+        # Create a quarterly list of the dataframes to iterate through
+        countries_df_list_Q = []
+        for i in countries_list:
+            df = pd.DataFrame(DataFrameDict_Q[i])
+            df.rename(columns={0:'Values'},inplace=True)
+            df = pd.pivot_table(data=df,index='time',values='Values',columns=['subject','measure'])
+            countries_df_list_Q.append(df)
+
+        combined_countries_df_list = list(zip(countries_df_list_M,countries_df_list_Q))
+
+        # Loop through and create dataframes for every country
+        for index, data in enumerate(combined_countries_df_list):
+
+            # Find country being extracted
+            country = countries_list[index]  
+            print(country)
+
+            # For consumer confidence
+            # For countries with no data
+            if country in ['CAN','IND','NOR']:
+                Consumer_Confidence_Index_df_M = pd.DataFrame()
+                Consumer_Confidence_Index_df_Q = pd.DataFrame()
+            # For countries with quarterly data   
+            elif country in []:
+                Consumer_Confidence_Index_df_Q = data[1]['CSCICP03']['IXNSA']
+                Consumer_Confidence_Index_df_Q.rename('consumer_confidence_index',inplace=True)
+                Consumer_Confidence_Index_df_M = pd.DataFrame()
+            # For countries with monthly data
+            else:
+                Consumer_Confidence_Index_df_M = data[0]['CSCICP03']['IXNSA']
+                Consumer_Confidence_Index_df_M.rename('consumer_confidence_index',inplace=True)
+                Consumer_Confidence_Index_df_Q = pd.DataFrame()
+
+            # For consumer prices for COST OF LIVING
+            # For countries with no data
+            if country in []:
+                Consumer_Price_Index_Cost_Of_Living_df_M = pd.DataFrame()
+                Consumer_Price_Index_Cost_Of_Living_df_Q = pd.DataFrame()
+            # For countries with quarterly data
+            elif country in ['AUS','NZL']:
+                Consumer_Price_Index_Cost_Of_Living_df_Q = data[1]['CPALTT01']['IXNB']
+                Consumer_Price_Index_Cost_Of_Living_df_Q.rename('consumer_price_index_cost_of_living',inplace=True)
+                Consumer_Price_Index_Cost_Of_Living_df_M = pd.DataFrame()
+            # For countries with monthly data
+            else:
+                Consumer_Price_Index_Cost_Of_Living_df_M = data[0]['CPALTT01']['IXNB']
+                Consumer_Price_Index_Cost_Of_Living_df_M.rename('consumer_price_index_cost_of_living',inplace=True)
+                Consumer_Price_Index_Cost_Of_Living_df_Q = pd.DataFrame()
+
+            # For consumer prices FOR INFLATION
+            # For countries with no data
+            if country in []:
+                Consumer_Price_Index_Inflation_df_M = pd.DataFrame()
+                Consumer_Price_Index_Inflation_df_Q = pd.DataFrame()
+            # For countries with quarterly data
+            elif country in ['AUS','NZL']:
+                Consumer_Price_Index_Inflation_df_Q = data[1]['CPALTT01']['GY']
+                Consumer_Price_Index_Inflation_df_Q.rename('consumer_price_index_inflation',inplace=True)
+                Consumer_Price_Index_Inflation_df_M = pd.DataFrame()
+            # For countries with monthly data
+            else:
+                Consumer_Price_Index_Inflation_df_M = data[0]['CPALTT01']['GY']
+                Consumer_Price_Index_Inflation_df_M.rename('consumer_price_index_inflation',inplace=True)
+                Consumer_Price_Index_Inflation_df_Q = pd.DataFrame()
+
+            # For GDP Index Smoothed 
+            # For countries with no data
+            if country in ['NLD','CHE','NZL','SWE','NOR']:
+                GDP_Index_Smoothed_df_M = pd.DataFrame()
+                GDP_Index_Smoothed_df_Q = pd.DataFrame()
+            # For countries with quarterly data
+            elif country in []:
+                GDP_Index_Smoothed_df_Q = data[1]['LORSGPRT']['STSA']
+                GDP_Index_Smoothed_df_Q.rename('gdp_index_smoothed',inplace=True)
+                GDP_Index_Smoothed_df_M = pd.DataFrame()
+            # For countries with monthly data
+            else:
+                GDP_Index_Smoothed_df_M = data[0]['LORSGPRT']['STSA']
+                GDP_Index_Smoothed_df_M.rename('gdp_index_smoothed',inplace=True)
+                GDP_Index_Smoothed_df_Q = pd.DataFrame()
+
+            # For Harmonised Unemployment Index
+            # For countries with no data
+            if country in ['IND','CHE','ZAF','CHN']:
+                Harmonised_Unemployment_Index_df_M = pd.DataFrame()
+                Harmonised_Unemployment_Index_df_Q = pd.DataFrame()
+            # For countries with quarterly data
+            elif country in ['NZL']:
+                Harmonised_Unemployment_Index_df_Q = data[1]['LRHUTTTT']['STSA']
+                Harmonised_Unemployment_Index_df_Q.rename('harmonised_unemployment_index',inplace=True)  
+                Harmonised_Unemployment_Index_df_M = pd.DataFrame()
+            # For countries with monthly data
+            else:     
+                Harmonised_Unemployment_Index_df_M = data[0]['LRHUTTTT']['STSA']
+                Harmonised_Unemployment_Index_df_M.rename('harmonised_unemployment_index',inplace=True)  
+                Harmonised_Unemployment_Index_df_Q = pd.DataFrame()
+
+            # For hourly earnings index manufacturing 
+            # For countries with no data
+            if country in ['IND','CHE','ZAF','CHN']:
+                Hourly_Earnings_Index_Manufacturing_df_M = pd.DataFrame()
+                Hourly_Earnings_Index_Manufacturing_df_Q = pd.DataFrame()
+            # For countries with quarterly data
+            elif country in ['FRA','DEU','ESP','AUS','NZL','KOR','NOR']:
+                Hourly_Earnings_Index_Manufacturing_df_Q = data[1]['LCEAMN01']['IXOBSA']
+                Hourly_Earnings_Index_Manufacturing_df_Q.rename('hourly_earnings_index_manufacturing',inplace=True)
+                Hourly_Earnings_Index_Manufacturing_df_M = pd.DataFrame()
+            # For countries with monthly data
+            else:
+                Hourly_Earnings_Index_Manufacturing_df_M = data[0]['LCEAMN01']['IXOBSA']
+                Hourly_Earnings_Index_Manufacturing_df_M.rename('hourly_earnings_index_manufacturing',inplace=True)
+                Hourly_Earnings_Index_Manufacturing_df_Q = pd.DataFrame()
+
+            # For hourly earnings index private
+            # Hourly_Earnings_Index_Private_df = data['GBR']['LCEAPR']['IXOBSA']
+            # Hourly_Earnings_Index_Private_df.rename('Hourly Earnings Index Private',inplace=True)
+
+            # For Short Term Interest Rate
+            # For countries with no data
+            if country in []:
+                Short_Term_Interest_Rate_df_M = pd.DataFrame()
+                Short_Term_Interest_Rate_df_Q = pd.DataFrame()
+            # For countries with quarterly data    
+            elif country in []:
+                Short_Term_Interest_Rate_df_Q = data[1]['IR3TIB01']['ST']
+                Short_Term_Interest_Rate_df_Q.rename('short_term_interest_rate',inplace=True)
+                Short_Term_Interest_Rate_df_M = pd.DataFrame()
+            # For countries with monthly data
+            else:
+                Short_Term_Interest_Rate_df_M = data[0]['IR3TIB01']['ST']
+                Short_Term_Interest_Rate_df_M.rename('short_term_interest_rate',inplace=True)
+                Short_Term_Interest_Rate_df_Q = pd.DataFrame()
+
+            # For Industrial Product Growth on Previous Period
+            # For countries with no data
+            if country in ['ZAF','CHN']:
+                Industrial_Product_Growth_on_Previous_Period_df_M = pd.DataFrame()
+                Industrial_Product_Growth_on_Previous_Period_df_Q = pd.DataFrame()
+            # For countries with quarterly data
+            elif country in ['AUS','NZL']:
+                Industrial_Product_Growth_on_Previous_Period_df_Q = data[1]['PRINTO01']['GPSA']
+                Industrial_Product_Growth_on_Previous_Period_df_Q.rename('industrial_product_growth_on_previous_period',inplace=True)
+                Industrial_Product_Growth_on_Previous_Period_df_M = pd.DataFrame()
+            # For countries with monthly data
+            else:
+                Industrial_Product_Growth_on_Previous_Period_df_M = data[0]['PRINTO01']['GPSA']
+                Industrial_Product_Growth_on_Previous_Period_df_M.rename('industrial_product_growth_on_previous_period',inplace=True)
+                Industrial_Product_Growth_on_Previous_Period_df_Q = pd.DataFrame()
+
+            # For Industrial Production Index
+            # For countries with no data
+            if country in ['ZAF','CHN']:
+                Industrial_Production_Index_df_M = pd.DataFrame()
+                Industrial_Production_Index_df_Q = pd.DataFrame()
+            # For countries with quarterly data
+            elif country in ['AUS','NZL']:
+                Industrial_Production_Index_df_Q = data[1]['PRINTO01']['IXOBSA']
+                Industrial_Production_Index_df_Q.rename('industrial_production_index',inplace=True) 
+                Industrial_Production_Index_df_M = pd.DataFrame()
+            # For countries with monthly data
+            else:
+                Industrial_Production_Index_df_M = data[0]['PRINTO01']['IXOBSA']
+                Industrial_Production_Index_df_M.rename('industrial_production_index',inplace=True)
+                Industrial_Production_Index_df_Q = pd.DataFrame()
+
+            # For USD GBP Exchange Rate
+            # USD_GBP_Exchange_Rate_df = data['GBR']['PRINTO01']['IXOBSA']
+            # USD_GBP_Exchange_Rate_df.rename('Industrial Production Index',inplace=True)
+            
+        
+
+        
+        
+            # Create monthly macroeconomic dataframe 
+            all_dfs_list_M = [Consumer_Confidence_Index_df_M,
+                            Consumer_Price_Index_Cost_Of_Living_df_M,
+                            Consumer_Price_Index_Inflation_df_M,
+                            GDP_Index_Smoothed_df_M,
+                            Harmonised_Unemployment_Index_df_M,
+                            Hourly_Earnings_Index_Manufacturing_df_M,
+                            Short_Term_Interest_Rate_df_M,
+                            Industrial_Product_Growth_on_Previous_Period_df_M,
+                            Industrial_Production_Index_df_M]
+
+            # Check if any dataframes are empty and if there are remove them 
+            all_dfs_list_M = [df for df in all_dfs_list_M if not df.empty]    
+            cif_Macroeconomic_df_M = pd.concat(all_dfs_list_M,axis=1)
+
+            # Create quarterly macroeconomic dataframe 
+            all_dfs_list_Q = [Consumer_Confidence_Index_df_Q,
+                            Consumer_Price_Index_Cost_Of_Living_df_Q,
+                            Consumer_Price_Index_Inflation_df_Q,
+                            GDP_Index_Smoothed_df_Q,
+                            Harmonised_Unemployment_Index_df_Q,
+                            Hourly_Earnings_Index_Manufacturing_df_Q,
+                            Short_Term_Interest_Rate_df_Q,
+                            Industrial_Product_Growth_on_Previous_Period_df_Q,
+                            Industrial_Production_Index_df_Q]
+
+            # Check if any dataframes are empty and if there are remove them 
+            all_dfs_list_Q = [df for df in all_dfs_list_Q if not df.empty]   
+            if all_dfs_list_Q != []:
+                macroeconomic_monthly_df_Q = pd.concat(all_dfs_list_Q,axis=1)
+            else: 
+                macroeconomic_monthly_df_Q  = []
+
+            # For USD GBP Exchange Rate
+            # If it's the UK add this series else don't
+            if countries_list[index] == 'GBR':
+                USD_GBP_Exchange_Rate_df = pd.read_csv('https://stats.oecd.org/SDMX-JSON/data/MEI_FIN/CCUS.' + countries_list[index] + '.M/OECD?contentType=csv')
+                USD_GBP_Exchange_Rate_df.head()
+                USD_GBP_Exchange_Rate_df_pivot = pd.pivot_table(USD_GBP_Exchange_Rate_df,values='Value',index='TIME',columns='Subject')
+                USD_GBP_Exchange_Rate_df_pivot_final = USD_GBP_Exchange_Rate_df_pivot.loc["2015-01":]
+                USD_GBP_Exchange_Rate_df_pivot_final.rename(columns={'Currency exchange rates, monthly average':'usd_gbp_exchange_rate'},inplace=True)
+
+                # Create final monthly dataframe
+                macroeconomic_monthly_df_M = pd.concat([cif_Macroeconomic_df_M,USD_GBP_Exchange_Rate_df_pivot_final],axis=1)
+            else:
+                # Create final monthly dataframe
+                macroeconomic_monthly_df_M = cif_Macroeconomic_df_M
+
+                
+                
+
+            # Create the final W/C Sunday dataframe 
+            # For monthly data
+            macroeconomic_monthly_df_M['Date']=macroeconomic_monthly_df_M.index
+            df_M = macroeconomic_monthly_df_M.set_index(pd.to_datetime(macroeconomic_monthly_df_M['Date'])).drop(columns='Date')
+            df_M.fillna(method="ffill",inplace=True)
+            df_M.reset_index(inplace=True)
+            
+            daily_records = []
+            # Iterate over each row in the DataFrame
+            for _, row in df_M.iterrows():
+                # Calculate the number of days in the month
+                num_days = calendar.monthrange(row["Date"].year, row["Date"].month)[1]
+                # Create a new record for each day of the month
+                for day in range(1, num_days + 1):
+                    daily_row = row.copy()
+                    daily_row["Date"] = row["Date"].replace(day=day)
+                    daily_records.append(daily_row)
+
+            # Convert the list of daily records into a DataFrame
+            daily_df = pd.DataFrame(daily_records)
+            
+            # Extend dataframe to include the current data if needed        
+            datelist = pd.date_range(daily_df["Date"].iloc[-1]+pd.Timedelta(days=1),datetime.date.today()).tolist()
+            extended_data =  np.repeat([list(daily_df.iloc[-1,1:].values)],len(datelist),axis=0)
+            q = pd.Series(datelist,name="Date")
+            s = pd.DataFrame(extended_data,columns=list(df_M.columns[1:]))
+            extended_daily_df = pd.concat([q,s],axis=1)
+            extended_daily_df = daily_df.append(extended_daily_df, ignore_index=False)
+            
+            # Create a week commencing column
+            extended_daily_df["Date"] = pd.to_datetime(extended_daily_df["Date"], format='%d %b %Y') 
+            extended_daily_df['week_start'] = extended_daily_df["Date"].apply(lambda x: x - pd.Timedelta(days=(x.weekday() - day_dict[week_commencing]) % 7))
+            extended_daily_df.drop("Date",axis=1,inplace=True)
+            extended_daily_df.rename(columns={'week_start':"Date"},inplace=True)
+            
+            # Take a weekly average
+            macroeconomic_weekly_df_M = extended_daily_df.groupby('Date').mean()
+            
+
+
+
+
+
+
+
+            # For quarterly data
+            # If there are quarterly datasets
+            if all_dfs_list_Q != []:
+                macroeconomic_monthly_df_Q['Date']=macroeconomic_monthly_df_Q.index
+                df_Q = macroeconomic_monthly_df_Q.set_index(pd.to_datetime(macroeconomic_monthly_df_Q['Date'])).drop(columns='Date')
+                df_Q.fillna(method="ffill",inplace=True)
+                df_Q.reset_index(inplace=True)
+
+                daily_records = []
+                for _, row in df_Q.iterrows():
+                    year = row["Date"].year
+                    month = row["Date"].month
+                    day = row["Date"].day
+                    last_date = get_last_day_of_the_quarter(datetime.datetime(year,month,day).date())
+                    all_days = pd.date_range(row["Date"],last_date,freq="D")
+
+                    # Create a new record for each day of the quarter
+                    for day in all_days:
+                        daily_row = row.copy()
+                        daily_row["Date"] = row["Date"].replace(day=day.day,month=day.month)
+                        daily_records.append(daily_row)
+
+                # Convert the list of daily records into a DataFrame
+                daily_df = pd.DataFrame(daily_records)
+                
+                # Extend dataframe to include data up to today
+                datelist = pd.date_range(daily_df["Date"].iloc[-1]+pd.Timedelta(days=1),datetime.date.today()).tolist()
+                extended_data =  np.repeat([list(daily_df.iloc[-1,1:].values)],len(datelist),axis=0)
+                q = pd.Series(datelist,name="Date")
+                s = pd.DataFrame(extended_data,columns=list(df_Q.columns[1:]))
+                extended_daily_df = pd.concat([q,s],axis=1)
+                extended_daily_df = daily_df.append(extended_daily_df, ignore_index=False)
+                
+                # Create a week commencing column
+                extended_daily_df["Date"] = pd.to_datetime(extended_daily_df["Date"], format='%d %b %Y') 
+                extended_daily_df['week_start'] = extended_daily_df["Date"].apply(lambda x: x - pd.Timedelta(days=(x.weekday() - day_dict[week_commencing]) % 7))
+                extended_daily_df.drop("Date",axis=1,inplace=True)
+                extended_daily_df.rename(columns={'week_start':"Date"},inplace=True)
+            
+                # Take a weekly average
+                macroeconomic_weekly_df_Q = extended_daily_df.groupby('Date').mean()
+
+            # Merge the two datasets together
+            if all_dfs_list_Q != []:
+                macroeconomic_weekly_df = macroeconomic_weekly_df_M.merge(macroeconomic_weekly_df_Q,left_index=True, right_index=True)
+            # If there are no quarterly datasets
+            else:
+                macroeconomic_weekly_df = macroeconomic_weekly_df_M
+            
+            # Change datime format
+            macroeconomic_weekly_df.index = macroeconomic_weekly_df.index.strftime('%d/%m/%Y') 
+            
+        macroeconomic_weekly_df.reset_index()
+            
+        return macroeconomic_weekly_df
+        
+        
     ###############################################################  Seasonality  ##########################################################################
 
     def pull_combined_dummies(self, week_commencing):
         # Week commencing dictionary
         day_dict = {"mon": 0, "tue": 1, "wed": 2, "thur": 3, "fri": 4, "sat": 5, "sun": 6}
         
         # Create daily date range dataframe
```

### Comparing `imsciences-0.5.8.1/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.8.2/imsciences.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.8.1
+Version: 0.5.8.2
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.8.1/setup.py` & `imsciences-0.5.8.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.8.1'
+VERSION = '0.5.8.2'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```


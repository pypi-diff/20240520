# Comparing `tmp/aecdata-0.0.3.tar.gz` & `tmp/aecdata-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aecdata-0.0.3.tar", last modified: Wed Apr 24 13:48:10 2024, max compression
+gzip compressed data, was "aecdata-0.0.4.tar", last modified: Mon May 20 13:35:42 2024, max compression
```

## Comparing `aecdata-0.0.3.tar` & `aecdata-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-24 13:48:10.149800 aecdata-0.0.3/
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      554 2024-04-04 08:44:04.000000 aecdata-0.0.3/LICENSE
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    16348 2024-04-24 13:48:10.149489 aecdata-0.0.3/PKG-INFO
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    15745 2024-04-22 09:51:42.000000 aecdata-0.0.3/README.md
-drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-24 13:48:10.147967 aecdata-0.0.3/aecdata/
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      104 2024-04-03 12:58:03.000000 aecdata-0.0.3/aecdata/__init__.py
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)     2402 2024-04-03 12:58:03.000000 aecdata-0.0.3/aecdata/auth.py
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)     9211 2024-04-05 12:23:40.000000 aecdata-0.0.3/aecdata/client.py
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    40613 2024-04-24 13:34:47.000000 aecdata-0.0.3/aecdata/productdata.py
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    20904 2024-04-12 08:29:30.000000 aecdata-0.0.3/aecdata/utils.py
-drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-24 13:48:10.149125 aecdata-0.0.3/aecdata.egg-info/
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    16348 2024-04-24 13:48:10.000000 aecdata-0.0.3/aecdata.egg-info/PKG-INFO
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      313 2024-04-24 13:48:10.000000 aecdata-0.0.3/aecdata.egg-info/SOURCES.txt
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        1 2024-04-24 13:48:10.000000 aecdata-0.0.3/aecdata.egg-info/dependency_links.txt
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       41 2024-04-24 13:48:10.000000 aecdata-0.0.3/aecdata.egg-info/requires.txt
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       14 2024-04-24 13:48:10.000000 aecdata-0.0.3/aecdata.egg-info/top_level.txt
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       38 2024-04-24 13:48:10.149846 aecdata-0.0.3/setup.cfg
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      771 2024-04-24 13:46:29.000000 aecdata-0.0.3/setup.py
-drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-24 13:48:10.148975 aecdata-0.0.3/tests/
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-03 12:58:03.000000 aecdata-0.0.3/tests/__init__.py
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-03 12:58:03.000000 aecdata-0.0.3/tests/test_client.py
+drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-05-20 13:35:42.526330 aecdata-0.0.4/
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      554 2024-04-04 08:44:04.000000 aecdata-0.0.4/LICENSE
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    17644 2024-05-20 13:35:42.526056 aecdata-0.0.4/PKG-INFO
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    17067 2024-05-20 13:30:58.000000 aecdata-0.0.4/README.md
+drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-05-20 13:35:42.524232 aecdata-0.0.4/aecdata/
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      104 2024-04-03 12:58:03.000000 aecdata-0.0.4/aecdata/__init__.py
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)     2445 2024-04-26 12:04:05.000000 aecdata-0.0.4/aecdata/auth.py
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)     9197 2024-04-26 12:04:05.000000 aecdata-0.0.4/aecdata/client.py
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    39206 2024-05-20 13:00:48.000000 aecdata-0.0.4/aecdata/productdata.py
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    20910 2024-04-26 12:04:05.000000 aecdata-0.0.4/aecdata/utils.py
+drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-05-20 13:35:42.525798 aecdata-0.0.4/aecdata.egg-info/
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    17644 2024-05-20 13:35:42.000000 aecdata-0.0.4/aecdata.egg-info/PKG-INFO
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      313 2024-05-20 13:35:42.000000 aecdata-0.0.4/aecdata.egg-info/SOURCES.txt
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        1 2024-05-20 13:35:42.000000 aecdata-0.0.4/aecdata.egg-info/dependency_links.txt
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       30 2024-05-20 13:35:42.000000 aecdata-0.0.4/aecdata.egg-info/requires.txt
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       14 2024-05-20 13:35:42.000000 aecdata-0.0.4/aecdata.egg-info/top_level.txt
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       38 2024-05-20 13:35:42.526378 aecdata-0.0.4/setup.cfg
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      749 2024-05-20 13:34:21.000000 aecdata-0.0.4/setup.py
+drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-05-20 13:35:42.525642 aecdata-0.0.4/tests/
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-03 12:58:03.000000 aecdata-0.0.4/tests/__init__.py
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-03 12:58:03.000000 aecdata-0.0.4/tests/test_client.py
```

### Comparing `aecdata-0.0.3/LICENSE` & `aecdata-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aecdata-0.0.3/PKG-INFO` & `aecdata-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: aecdata
-Version: 0.0.3
-Summary: A Python library designed to simplify access to the 2050-materials API
-Home-page: https://github.com/2050-Materials/aecdata
-Author: 2050 Materials
-Author-email: nicodemos@2050-materials.com
-License: Apache License 2.0
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: matplotlib
-Requires-Dist: pyarrow
-
 # AECData
 
 AECData is a Python library designed to facilitate seamless interaction with the 2050-materials platform API (see documentation [here](https://docs.2050-materials.com/getting-started-with-2050-materials/using-the-api)). By abstracting the complexities of authentication and data retrieval, this library empowers developers to focus on analyzing and utilizing environmental data about construction materials effectively.
 
 ## Key Features
 
 - **Simplified Authentication**: Manages API tokens automatically, streamlining the authentication process.
@@ -59,17 +40,17 @@
 
 ## `Authenticator` Class
 
 The `Authenticator` class is designed to handle the authentication process for accessing the API. It is used internally to manage both API tokens and to ensure continued access.
 
 ### Initialization
 
--   `__init__(self, developer_token, base_api_url)`: Initializes the `Authenticator` instance.
+-   `__init__(self, developer_token, base_api_url = 'https://app.2050-materials.com/')`: Initializes the `Authenticator` instance.
     -   `developer_token`: The developer token provided for API access.
-    -   `base_api_url`: The base URL for the API endpoints.
+    -   `base_api_url` (optional): The base URL for the API endpoints.
 
 ### Methods
 
 -   `get_token(self)`: Retrieves the API token using the developer token. This method is ideal for operations that only require a single API token without the need for a refresh token.
 -   `get_api_and_refresh_token(self)`: Retrieves both the API token and a refresh token. This is useful for long-running applications that may need to refresh the API token.
 -   `refresh_api_token(self)`: Refreshes the API token using the refresh token. This method should be used when the API token has expired and a new one is needed without re-authenticating using the developer token.
 
@@ -172,15 +153,15 @@
 
 - `get_available_units(self)`: Extracts and returns a set of available units for scaling based on the data's 'material_facts.scaling_factors' entries.
 - `convert_df_to_unit(self, df, unit='declared_unit', amount=1)`: Scales the DataFrame's numerical fields to the specified unit and amount.
 - `scale_products_by_unit_and_amount(self, products_info)`: Scales product data based on a dictionary mapping product UUIDs to units and amounts, facilitating comparisons and aggregations.
 
 #### Plotting and Visualization
 
-- `plot_product_contributions(self, products_info, field_name)`: Generates a pie chart illustrating the contributions of each product to the specified field (e.g., CO2 emissions).
+- `get_product_contributions(self, products_info, field_name)`: Generates a pie chart illustrating the contributions of each product to the specified field (e.g., CO2 emissions).
 
 #### Data Transformation for EPDx Format
 
 - `to_epdx(self)`: Converts the data into the EPDx format, suitable for environmental product declarations.
 
 
 ## Usage Example
@@ -195,18 +176,29 @@
 # Create a custom project with specified products, units and amounts
 products_info = {
     '6aa6d32c-f8cf-11ed-9c01-0242ac120004' : {'amount': 0.2}, 
     'c0800dc0-f8cc-11ed-9c01-0242ac120004' : {'amount': 0.30}, 
     '6ab16fb2-f8cf-11ed-9c01-0242ac120004' : {'unit':'m2'},
     '6aab7152-f8cf-11ed-9c01-0242ac120004' : {'unit':'m2', 'amount': 1},
 }
+
+import matplotlib.pyplot as plt
+
 scale_df = product_data.scale_products_by_unit_and_amount(products_info)
 
-# Vizualise the contributions from each product for a specific LCA field
-product_data.plot_product_contributions(products_info, 'material_facts.manufacturing')
+field_name =  'material_facts.manufacturing'
+contributions = product_data.get_product_contributions(products_info, 'material_facts.manufacturing')
+contributions
+
+# Plotting pie chart
+plt.figure(figsize=(10, 8))
+contributions.plot(kind='pie', autopct='%1.1f%%', startangle=90, counterclock=False, labels=contributions.index)
+plt.title(f'Contribution of Each Product by {field_name}')
+plt.ylabel('')  # Hide y-axis label for clarity
+plt.show()
 
 # Convert to EPDx format
 epdx_products = product_data.to_epdx()
 ```
 
 ## `ProductStatistics` Class
 
@@ -235,41 +227,64 @@
 
 #### Data Filtering and Transformation
 
 - `remove_outliers_from_df(self, filtered_df, field, method, sqrt_tranf)`: Removes outliers from the DataFrame based on the specified field and method, optionally applying a square root transformation for variance stabilization.
 - `filter_dataframe_based_on_field(self, field, filters=None, include_estimated_values=False, remove_outliers=True, method='IQR', sqrt_tranf=True)`: Filters the DataFrame based on specified criteria, including the treatment of estimated values and outliers.
 
 #### Plotting and Visualization
-
-- `plot_histogram(self, df, field)`: Generates a histogram for the specified field, visualizing the distribution of values.
-- `get_field_distribution(self, field, filters=None, include_estimated_values=False, remove_outliers=True, method='IQR', sqrt_tranf=True)`: Filters the DataFrame and plots the distribution of the specified field, offering insights into the data's structure.
-- `plot_distribution_boxplot(self, df, field, group_by_field)`: Creates a boxplot for the specified field, grouped by another field, highlighting the variance and distribution within the data.
+- `get_product_contributions(products_info, 'material_facts.manufacturing')`: Takes a dictionary with product ids as keys and values a dictionary with unit and amount and for an LCA field calculates the percentage contribution of carbon emissions.
+- `get_field_distribution(self, field, filters=None, include_estimated_values=False, remove_outliers=True, method='IQR', sqrt_tranf=True)`: Filters the DataFrame and returns the distribution of the specified field, offering insights into the data's structure.
 - `get_field_distribution_boxplot(self, field, group_by_field, filters=None, include_estimated_values=False, remove_outliers=True, method='IQR', sqrt_tranf=True)`: Filters the DataFrame and generates a boxplot for the specified field, providing a visual representation of statistical distributions.
 
 ## Usage Example
 
 ```
-# Create ProductStatistics (extension of ProductData)
-stats_obj = ProductStatistics(product_data.dataframe, unit='m2')
+import matplotlib.pyplot as plt
 
-# Choose fields to group by
-group_by = [
-    'country',
-    'manufacturing_continent',
-]
+def plot_histogram(df, field):
+    bin_count = min(len(df[field].unique()), 50)  # Limit the number of bins to a maximum of 50
+    plt.figure(figsize=(10, 6))
+    n, bins, patches = plt.hist(df[field], bins=bin_count, color='#2ab0ff', alpha=0.7, rwidth=0.85)
+    plt.grid(axis='y', alpha=0.75)
+    plt.xlabel('Value', fontsize=15)
+    plt.ylabel('Frequency', fontsize=15)
+    plt.xticks(fontsize=12)
+    plt.yticks(fontsize=12)
+    plt.title(f'Distribution of {field}', fontsize=15)
+    plt.axvline(x=df[field].mean(), color='r', linestyle='-', label=f'Mean: {df[field].mean():.4f}')
+    plt.axvline(x=df[field].median(), color='m', linestyle='-', label=f'Median: {df[field].median():.4f}')
+    plt.legend(loc='upper right')
+    plt.show()
 
-# Get all available fields
-all_available_fields  = stats_obj.get_available_fields()
-
-# Calculate statistics dataframe
-stat_df = stats_obj.get_statistics(group_by=group_by, fields=all_available_fields, statistical_metrics=['count', 'mean', 'median'], include_estimated_values=False, remove_outliers=True, method='IQR', sqrt_tranf=True, min_count=3)
-
-# Apply further filters and get field distribution
 filters = {
     'material_type':'Ceramic',
+    # 'elements_nrm_1':'3.1 - Wall finishes'
 }
-stats_obj.get_field_distribution(field='material_facts.manufacturing', filters=filters, include_estimated_values=True, remove_outliers=False, method='IQR', sqrt_tranf=True)
+field = 'material_facts.manufacturing'
+df = stats_obj.get_field_distribution(field=field, filters=filters, include_estimated_values=True, remove_outliers=False, method='IQR', sqrt_tranf=True)
+
+plot_histogram(df, field)
 
-# Get field distribution boxplot for all product types
-stats_obj.get_field_distribution_boxplot(field='material_facts.manufacturing', group_by_field='product_type', filters=None, include_estimated_values=True, remove_outliers=True, method='IQR', sqrt_tranf=True)
+# With removing outliers
+field = 'material_facts.manufacturing'
+df = stats_obj.get_field_distribution(field=field, filters=filters, include_estimated_values=True, remove_outliers=True, method='IQR', sqrt_tranf=True)
+
+plot_histogram(df, field)
+
+# Field distribution boxplot
+field='material_facts.manufacturing'
+group_by_field = 'product_type'
+# Get a dict with keys product types and values dataframe series 
+grouped_data_dict = stats_obj.get_field_distribution_boxplot(field=field, group_by_field=group_by_field, filters=None, include_estimated_values=True, remove_outliers=True, method='IQR', sqrt_tranf=True)
+
+# Box-plotting
+plt.figure(figsize=(10, 6))
+plt.boxplot(grouped_data_dict.values(), patch_artist=True, labels=grouped_data_dict.keys())
+plt.grid(axis='y', alpha=0.75)
+plt.xlabel(group_by_field, fontsize=15)
+plt.ylabel('Value', fontsize=15)
+plt.xticks(fontsize=12, rotation=45)  # Rotate labels if there are many groups
+plt.yticks(fontsize=12)
+plt.title(f'Distribution of {field} by {group_by_field}', fontsize=15)
+plt.show()
 ```
```

### Comparing `aecdata-0.0.3/README.md` & `aecdata-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: aecdata
+Version: 0.0.4
+Summary: A Python library designed to simplify access to the 2050-materials API
+Home-page: https://github.com/2050-Materials/aecdata
+Author: 2050 Materials
+Author-email: nicodemos@2050-materials.com
+License: Apache License 2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: pyarrow
+
 # AECData
 
 AECData is a Python library designed to facilitate seamless interaction with the 2050-materials platform API (see documentation [here](https://docs.2050-materials.com/getting-started-with-2050-materials/using-the-api)). By abstracting the complexities of authentication and data retrieval, this library empowers developers to focus on analyzing and utilizing environmental data about construction materials effectively.
 
 ## Key Features
 
 - **Simplified Authentication**: Manages API tokens automatically, streamlining the authentication process.
@@ -40,17 +58,17 @@
 
 ## `Authenticator` Class
 
 The `Authenticator` class is designed to handle the authentication process for accessing the API. It is used internally to manage both API tokens and to ensure continued access.
 
 ### Initialization
 
--   `__init__(self, developer_token, base_api_url)`: Initializes the `Authenticator` instance.
+-   `__init__(self, developer_token, base_api_url = 'https://app.2050-materials.com/')`: Initializes the `Authenticator` instance.
     -   `developer_token`: The developer token provided for API access.
-    -   `base_api_url`: The base URL for the API endpoints.
+    -   `base_api_url` (optional): The base URL for the API endpoints.
 
 ### Methods
 
 -   `get_token(self)`: Retrieves the API token using the developer token. This method is ideal for operations that only require a single API token without the need for a refresh token.
 -   `get_api_and_refresh_token(self)`: Retrieves both the API token and a refresh token. This is useful for long-running applications that may need to refresh the API token.
 -   `refresh_api_token(self)`: Refreshes the API token using the refresh token. This method should be used when the API token has expired and a new one is needed without re-authenticating using the developer token.
 
@@ -153,15 +171,15 @@
 
 - `get_available_units(self)`: Extracts and returns a set of available units for scaling based on the data's 'material_facts.scaling_factors' entries.
 - `convert_df_to_unit(self, df, unit='declared_unit', amount=1)`: Scales the DataFrame's numerical fields to the specified unit and amount.
 - `scale_products_by_unit_and_amount(self, products_info)`: Scales product data based on a dictionary mapping product UUIDs to units and amounts, facilitating comparisons and aggregations.
 
 #### Plotting and Visualization
 
-- `plot_product_contributions(self, products_info, field_name)`: Generates a pie chart illustrating the contributions of each product to the specified field (e.g., CO2 emissions).
+- `get_product_contributions(self, products_info, field_name)`: Generates a pie chart illustrating the contributions of each product to the specified field (e.g., CO2 emissions).
 
 #### Data Transformation for EPDx Format
 
 - `to_epdx(self)`: Converts the data into the EPDx format, suitable for environmental product declarations.
 
 
 ## Usage Example
@@ -176,18 +194,29 @@
 # Create a custom project with specified products, units and amounts
 products_info = {
     '6aa6d32c-f8cf-11ed-9c01-0242ac120004' : {'amount': 0.2}, 
     'c0800dc0-f8cc-11ed-9c01-0242ac120004' : {'amount': 0.30}, 
     '6ab16fb2-f8cf-11ed-9c01-0242ac120004' : {'unit':'m2'},
     '6aab7152-f8cf-11ed-9c01-0242ac120004' : {'unit':'m2', 'amount': 1},
 }
+
+import matplotlib.pyplot as plt
+
 scale_df = product_data.scale_products_by_unit_and_amount(products_info)
 
-# Vizualise the contributions from each product for a specific LCA field
-product_data.plot_product_contributions(products_info, 'material_facts.manufacturing')
+field_name =  'material_facts.manufacturing'
+contributions = product_data.get_product_contributions(products_info, 'material_facts.manufacturing')
+contributions
+
+# Plotting pie chart
+plt.figure(figsize=(10, 8))
+contributions.plot(kind='pie', autopct='%1.1f%%', startangle=90, counterclock=False, labels=contributions.index)
+plt.title(f'Contribution of Each Product by {field_name}')
+plt.ylabel('')  # Hide y-axis label for clarity
+plt.show()
 
 # Convert to EPDx format
 epdx_products = product_data.to_epdx()
 ```
 
 ## `ProductStatistics` Class
 
@@ -216,41 +245,64 @@
 
 #### Data Filtering and Transformation
 
 - `remove_outliers_from_df(self, filtered_df, field, method, sqrt_tranf)`: Removes outliers from the DataFrame based on the specified field and method, optionally applying a square root transformation for variance stabilization.
 - `filter_dataframe_based_on_field(self, field, filters=None, include_estimated_values=False, remove_outliers=True, method='IQR', sqrt_tranf=True)`: Filters the DataFrame based on specified criteria, including the treatment of estimated values and outliers.
 
 #### Plotting and Visualization
-
-- `plot_histogram(self, df, field)`: Generates a histogram for the specified field, visualizing the distribution of values.
-- `get_field_distribution(self, field, filters=None, include_estimated_values=False, remove_outliers=True, method='IQR', sqrt_tranf=True)`: Filters the DataFrame and plots the distribution of the specified field, offering insights into the data's structure.
-- `plot_distribution_boxplot(self, df, field, group_by_field)`: Creates a boxplot for the specified field, grouped by another field, highlighting the variance and distribution within the data.
+- `get_product_contributions(products_info, 'material_facts.manufacturing')`: Takes a dictionary with product ids as keys and values a dictionary with unit and amount and for an LCA field calculates the percentage contribution of carbon emissions.
+- `get_field_distribution(self, field, filters=None, include_estimated_values=False, remove_outliers=True, method='IQR', sqrt_tranf=True)`: Filters the DataFrame and returns the distribution of the specified field, offering insights into the data's structure.
 - `get_field_distribution_boxplot(self, field, group_by_field, filters=None, include_estimated_values=False, remove_outliers=True, method='IQR', sqrt_tranf=True)`: Filters the DataFrame and generates a boxplot for the specified field, providing a visual representation of statistical distributions.
 
 ## Usage Example
 
 ```
-# Create ProductStatistics (extension of ProductData)
-stats_obj = ProductStatistics(product_data.dataframe, unit='m2')
+import matplotlib.pyplot as plt
 
-# Choose fields to group by
-group_by = [
-    'country',
-    'manufacturing_continent',
-]
+def plot_histogram(df, field):
+    bin_count = min(len(df[field].unique()), 50)  # Limit the number of bins to a maximum of 50
+    plt.figure(figsize=(10, 6))
+    n, bins, patches = plt.hist(df[field], bins=bin_count, color='#2ab0ff', alpha=0.7, rwidth=0.85)
+    plt.grid(axis='y', alpha=0.75)
+    plt.xlabel('Value', fontsize=15)
+    plt.ylabel('Frequency', fontsize=15)
+    plt.xticks(fontsize=12)
+    plt.yticks(fontsize=12)
+    plt.title(f'Distribution of {field}', fontsize=15)
+    plt.axvline(x=df[field].mean(), color='r', linestyle='-', label=f'Mean: {df[field].mean():.4f}')
+    plt.axvline(x=df[field].median(), color='m', linestyle='-', label=f'Median: {df[field].median():.4f}')
+    plt.legend(loc='upper right')
+    plt.show()
 
-# Get all available fields
-all_available_fields  = stats_obj.get_available_fields()
-
-# Calculate statistics dataframe
-stat_df = stats_obj.get_statistics(group_by=group_by, fields=all_available_fields, statistical_metrics=['count', 'mean', 'median'], include_estimated_values=False, remove_outliers=True, method='IQR', sqrt_tranf=True, min_count=3)
-
-# Apply further filters and get field distribution
 filters = {
     'material_type':'Ceramic',
+    # 'elements_nrm_1':'3.1 - Wall finishes'
 }
-stats_obj.get_field_distribution(field='material_facts.manufacturing', filters=filters, include_estimated_values=True, remove_outliers=False, method='IQR', sqrt_tranf=True)
+field = 'material_facts.manufacturing'
+df = stats_obj.get_field_distribution(field=field, filters=filters, include_estimated_values=True, remove_outliers=False, method='IQR', sqrt_tranf=True)
+
+plot_histogram(df, field)
 
-# Get field distribution boxplot for all product types
-stats_obj.get_field_distribution_boxplot(field='material_facts.manufacturing', group_by_field='product_type', filters=None, include_estimated_values=True, remove_outliers=True, method='IQR', sqrt_tranf=True)
+# With removing outliers
+field = 'material_facts.manufacturing'
+df = stats_obj.get_field_distribution(field=field, filters=filters, include_estimated_values=True, remove_outliers=True, method='IQR', sqrt_tranf=True)
+
+plot_histogram(df, field)
+
+# Field distribution boxplot
+field='material_facts.manufacturing'
+group_by_field = 'product_type'
+# Get a dict with keys product types and values dataframe series 
+grouped_data_dict = stats_obj.get_field_distribution_boxplot(field=field, group_by_field=group_by_field, filters=None, include_estimated_values=True, remove_outliers=True, method='IQR', sqrt_tranf=True)
+
+# Box-plotting
+plt.figure(figsize=(10, 6))
+plt.boxplot(grouped_data_dict.values(), patch_artist=True, labels=grouped_data_dict.keys())
+plt.grid(axis='y', alpha=0.75)
+plt.xlabel(group_by_field, fontsize=15)
+plt.ylabel('Value', fontsize=15)
+plt.xticks(fontsize=12, rotation=45)  # Rotate labels if there are many groups
+plt.yticks(fontsize=12)
+plt.title(f'Distribution of {field} by {group_by_field}', fontsize=15)
+plt.show()
 ```
```

### Comparing `aecdata-0.0.3/aecdata/auth.py` & `aecdata-0.0.4/aecdata/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
+from .utils import *
 
 class Authenticator:
-    def __init__(self, developer_token, base_api_url):
+    def __init__(self, developer_token, base_api_url = production_base_url):
         self.base_api_url = base_api_url
         self.developer_token = developer_token
         self.api_token = None
         self.refresh_token = None
 
     def get_token(self):
         base_token_url = f'{self.base_api_url}developer/api/token/getapitoken/'
```

### Comparing `aecdata-0.0.3/aecdata/client.py` & `aecdata-0.0.4/aecdata/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .auth import Authenticator
 from .utils import *
 
 # Ensure all instances of this specific warning are always shown
 warnings.simplefilter('always', UserWarning)
 
 class User:
-    def __init__(self, developer_token, base_api_url = "https://app.2050-materials.com/"):
+    def __init__(self, developer_token, base_api_url = production_base_url):
         self.base_api_url = base_api_url
         self.authenticator = Authenticator(developer_token, base_api_url)
         self.api_token, self.refresh_token = self.authenticator.get_api_and_refresh_token()
         self._filters = None
         self._field_description = None
 
     @property
```

### Comparing `aecdata-0.0.3/aecdata/productdata.py` & `aecdata-0.0.4/aecdata/productdata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import pandas as pd
 import numpy as np
 import json
 import warnings
 from itertools import product
 from datetime import datetime
-import matplotlib.pyplot as plt
 from .utils import *
 
 # Ensure all instances of this specific warning are always shown
 warnings.simplefilter('always', UserWarning)
 
 class ProductData:
     def __init__(self, data):
@@ -231,15 +230,15 @@
                     print(f"Scaling to unit '{unit}' failed for product {uuid}.")
             else:
                 print(f"Product UUID '{uuid}' not found in DataFrame.")
 
         return scaled_products_df.reset_index(drop=True)
 
 
-    def plot_product_contributions(self, products_info, field_name):
+    def get_product_contributions(self, products_info, field_name):
         # Use the existing method to scale the DataFrame
         scaled_df = self.scale_products_by_unit_and_amount(products_info)
 
         # Ensure the DataFrame is ready for operations
         scaled_df = scaled_df.infer_objects()
 
         # Check if the specified field and required columns are available
@@ -254,20 +253,16 @@
         scaled_df['label'] = scaled_df['name'] + '\n(' + scaled_df['unique_product_uuid_v2'] + ')'
 
         scaled_df.replace([np.inf, -np.inf], np.nan, inplace=True)
 
         # Aggregate the data by summing the specified field, grouped by the new 'label' attribute
         contributions = scaled_df.groupby('label')[field_name].sum()
 
-        # Plotting
-        plt.figure(figsize=(10, 8))
-        contributions.plot(kind='pie', autopct='%1.1f%%', startangle=90, counterclock=False, labels=contributions.index)
-        plt.title(f'Contribution of Each Product by {field_name}')
-        plt.ylabel('')  # Hide y-axis label for clarity
-        plt.show()
+        return contributions
+
 
     def to_epdx(self):
         def create_epdx_dict_from_row(row, modules_to_epdx, lca_field_to_epdx):
             # Initialize the dictionary to hold the EPDx structured data
             epdx_dict = {}
 
             # Iterate through the LCA fields to EPDx abbreviations mapping
@@ -853,55 +848,33 @@
         df = df.dropna(subset=[field])
 
         if remove_outliers:
             df = self.remove_outliers_from_df(df, field, method, sqrt_tranf)
 
         return df.reset_index(drop=True)
 
-    def plot_histogram(self, df, field):
-        bin_count = min(len(df[field].unique()), 50)  # Limit the number of bins to a maximum of 50
-        plt.figure(figsize=(10, 6))
-        n, bins, patches = plt.hist(df[field], bins=bin_count, color='#2ab0ff', alpha=0.7, rwidth=0.85)
-        plt.grid(axis='y', alpha=0.75)
-        plt.xlabel('Value', fontsize=15)
-        plt.ylabel('Frequency', fontsize=15)
-        plt.xticks(fontsize=12)
-        plt.yticks(fontsize=12)
-        plt.title(f'Distribution of {field}', fontsize=15)
-        plt.axvline(x=df[field].mean(), color='r', linestyle='-', label=f'Mean: {df[field].mean():.4f}')
-        plt.axvline(x=df[field].median(), color='m', linestyle='-', label=f'Median: {df[field].median():.4f}')
-        plt.legend(loc='upper right')
-        plt.show()
-
     def get_field_distribution(self, field, filters=None, include_estimated_values=False, remove_outliers=True, method='IQR', sqrt_tranf=True):
         df = self.filter_dataframe_based_on_field(field, filters, include_estimated_values, remove_outliers, method, sqrt_tranf)
+        return df
+        # self.plot_histogram(df, field)
 
-        self.plot_histogram(df, field)
-
-    def plot_distribution_boxplot(self, df, field, group_by_field):
+    def get_grouped_data(self, df, field, group_by_field):
         # Ensure the group_by_field is in the DataFrame
         if group_by_field not in df.columns:
             raise ValueError(f"{group_by_field} column is not available in the DataFrame.")
 
         # Get unique values for the group_by_field column
         group_by_dict = self.get_group_by_dict(df, [group_by_field])
 
-        # Plotting
-        plt.figure(figsize=(10, 6))
-
         # Create a boxplot for each unique value in the group_by_field column
-        grouped_data = [df[df[group_by_field] == value][field] for value in group_by_dict[group_by_field]]
-        plt.boxplot(grouped_data, patch_artist=True, labels=group_by_dict[group_by_field])
+        # grouped_data = [df[df[group_by_field] == value][field] for value in group_by_dict[group_by_field]]
+        grouped_data_dict = {value: df[df[group_by_field] == value][field] for value in group_by_dict[group_by_field]}
+
+        return grouped_data_dict
 
-        plt.grid(axis='y', alpha=0.75)
-        plt.xlabel(group_by_field, fontsize=15)
-        plt.ylabel('Value', fontsize=15)
-        plt.xticks(fontsize=12, rotation=45)  # Rotate labels if there are many groups
-        plt.yticks(fontsize=12)
-        plt.title(f'Distribution of {field} by {group_by_field}', fontsize=15)
-        plt.show()
 
     def get_field_distribution_boxplot(self, field, group_by_field, filters=None, include_estimated_values=False, remove_outliers=True, method='IQR', sqrt_tranf=True):
         df = self.filter_dataframe_based_on_field(field, filters, include_estimated_values, remove_outliers, method, sqrt_tranf)
         # After preparing and filtering the DataFrame, plot it
-        self.plot_distribution_boxplot(df, field, group_by_field)
+        grouped_data_dict = self.get_grouped_data(df, field, group_by_field)
+        return grouped_data_dict
```

### Comparing `aecdata-0.0.3/aecdata/utils.py` & `aecdata-0.0.4/aecdata/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,8 @@
-
-
-# lca_fields = ['net_fresh_water_use', 'non_renewable_primary_energy','non_renewable_primary_energy_raw_materials','non_renewable_secondary_fuels','renewable_primary_energy',
-#     'renewable_primary_energy_raw_materials','renewable_secondary_fuels','secondary_material_use','total_non_renewable_primary_energy','total_renewable_primary_energy','components_for_reuse',
-#     'exported_electrical_energy','exported_thermal_energy','hazardous_waste_disposed','materials_for_energy_recovery','materials_for_recycling','non_hazardous_waste_disposed',
-#     'radioactive_waste_disposed','abiotic_depletion_potential_fossil','abiotic_depletion_potential_non_fossil','acidification_potential','ozone_depletion_potential','eutrophication_potential',
-#     'formation_potential_of_tropospheric_ozone','global_warming_potential_fossil','global_warming_potential_biogenic','global_warming_potential_luluc','water_deprivation_potential'
-#               ]
-#
-# lca_modules = ['A1', 'A2', 'A3', 'A1A2A3', 'A4', 'A5', 'B1', 'B2', 'B3', 'B4', 'B5', 'B6', 'B7', 'C1', 'C2', 'C3', 'C4', 'D']
+production_base_url = "https://app.2050-materials.com/"
 
 unit_to_field_mapping = {
     ('kg', 'm3'): 'density',
     ('kg', 'm2'): 'grammage',
     ('kg', 'm'): 'linear_density',
     ('kg', 'piece'): 'mass_per_piece',
     ('m3', 'm2'): 'thickness',
@@ -145,18 +136,27 @@
     'global_warming_potential_luluc': None,  # Not directly mapped, may need a custom field or consider 'gwp'
     'water_deprivation_potential': None,  # Not directly mapped, may need a custom field or consider 'fw'
 }
 
 field_description = {}
 
 field_description['filters_template']  = {
-    'sort_by': "Sort By (Available options are - carbon_sorting, latest, recycled_content, recyclable_content)",
+    'sort_by': "Sort By (Available options are - carbon_sorting, latest, recycled_content, recyclable_content, update & created)",
     'group_by': "Products are grouped by (Available options are - company_name, product_type, material, manufacturing_location, continent, price_range, building_applications, building_types, certification_types)",
+    'unique_product_uuid_v2': "Search a specific product with UUID (2050 Materials unique id) (e.g. unique_product_uuid_v2=ac22f2a4-f960-11ed-92ea-0242ac120004)",
+    'product_url': "Search a specific product with product url (e.g. product_url='https://app.2050-materials.com/product/details_designer/isolconfort-srl-eps-eco-espanso-k120/')",
+    "compliances": "compliances (e.g. compliances=EN 15804)",
+    "updated_after": "Products updated after a date (e.g. updated_after=2022-12-31)",
+    "updated_before": "Products updated before a date (e.g. updated_before=2022-12-31)",
+    "created_after": "Products created after a date (e.g. created_after=2022-12-31)",
+    "created_before": "Products created before a date (e.g. created_before=2022-12-31)",
+    "created_between": "Products created during date range (e.g. created_between=2022-12-31,2023-12-31)",
+    "updated_between": "Products updated during date range (e.g. updated_between=2022-12-31,2023-12-31)",
     'mf_unit': "Include dictionary with material facts in specified units. Accepts a single value or multiple values. Use 'all' to include all units. For example, to express material facts in square meters and square feet, use mf_unit='m2'&mf_unit='ft2'.",
-    'name': "Search with the name of the product",
+    'name': "Search with the name of the product (e.g. name='Mycelium Insulation Panel')",
     'product_type': "Product Type Ids (e.g. product_type=2 or [2,3])",
     'product_type_family': "Product Type Family Ids (e.g. product_type_family=3 or [2,3])",
     'material_types': "Material Types Ids (e.g. material_types=4 or [2,3])",
     'material_types_family': "Material Types Family Ids (e.g. material_types_family=3 or [2,3])",
     'building_applications': "Building Applications Ids (e.g. building_applications=4 or [2,3])",
     'company': "Company Ids (e.g. company=4 or [22,23])",
     'building_types': "Building Types Ids (e.g. building_types=4 or [1,2,3,4])",
```

### Comparing `aecdata-0.0.3/aecdata.egg-info/PKG-INFO` & `aecdata-0.0.4/aecdata.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: aecdata
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python library designed to simplify access to the 2050-materials API
 Home-page: https://github.com/2050-Materials/aecdata
 Author: 2050 Materials
 Author-email: nicodemos@2050-materials.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: matplotlib
 Requires-Dist: pyarrow
 
 # AECData
 
 AECData is a Python library designed to facilitate seamless interaction with the 2050-materials platform API (see documentation [here](https://docs.2050-materials.com/getting-started-with-2050-materials/using-the-api)). By abstracting the complexities of authentication and data retrieval, this library empowers developers to focus on analyzing and utilizing environmental data about construction materials effectively.
 
 ## Key Features
@@ -59,17 +58,17 @@
 
 ## `Authenticator` Class
 
 The `Authenticator` class is designed to handle the authentication process for accessing the API. It is used internally to manage both API tokens and to ensure continued access.
 
 ### Initialization
 
--   `__init__(self, developer_token, base_api_url)`: Initializes the `Authenticator` instance.
+-   `__init__(self, developer_token, base_api_url = 'https://app.2050-materials.com/')`: Initializes the `Authenticator` instance.
     -   `developer_token`: The developer token provided for API access.
-    -   `base_api_url`: The base URL for the API endpoints.
+    -   `base_api_url` (optional): The base URL for the API endpoints.
 
 ### Methods
 
 -   `get_token(self)`: Retrieves the API token using the developer token. This method is ideal for operations that only require a single API token without the need for a refresh token.
 -   `get_api_and_refresh_token(self)`: Retrieves both the API token and a refresh token. This is useful for long-running applications that may need to refresh the API token.
 -   `refresh_api_token(self)`: Refreshes the API token using the refresh token. This method should be used when the API token has expired and a new one is needed without re-authenticating using the developer token.
 
@@ -172,15 +171,15 @@
 
 - `get_available_units(self)`: Extracts and returns a set of available units for scaling based on the data's 'material_facts.scaling_factors' entries.
 - `convert_df_to_unit(self, df, unit='declared_unit', amount=1)`: Scales the DataFrame's numerical fields to the specified unit and amount.
 - `scale_products_by_unit_and_amount(self, products_info)`: Scales product data based on a dictionary mapping product UUIDs to units and amounts, facilitating comparisons and aggregations.
 
 #### Plotting and Visualization
 
-- `plot_product_contributions(self, products_info, field_name)`: Generates a pie chart illustrating the contributions of each product to the specified field (e.g., CO2 emissions).
+- `get_product_contributions(self, products_info, field_name)`: Generates a pie chart illustrating the contributions of each product to the specified field (e.g., CO2 emissions).
 
 #### Data Transformation for EPDx Format
 
 - `to_epdx(self)`: Converts the data into the EPDx format, suitable for environmental product declarations.
 
 
 ## Usage Example
@@ -195,18 +194,29 @@
 # Create a custom project with specified products, units and amounts
 products_info = {
     '6aa6d32c-f8cf-11ed-9c01-0242ac120004' : {'amount': 0.2}, 
     'c0800dc0-f8cc-11ed-9c01-0242ac120004' : {'amount': 0.30}, 
     '6ab16fb2-f8cf-11ed-9c01-0242ac120004' : {'unit':'m2'},
     '6aab7152-f8cf-11ed-9c01-0242ac120004' : {'unit':'m2', 'amount': 1},
 }
+
+import matplotlib.pyplot as plt
+
 scale_df = product_data.scale_products_by_unit_and_amount(products_info)
 
-# Vizualise the contributions from each product for a specific LCA field
-product_data.plot_product_contributions(products_info, 'material_facts.manufacturing')
+field_name =  'material_facts.manufacturing'
+contributions = product_data.get_product_contributions(products_info, 'material_facts.manufacturing')
+contributions
+
+# Plotting pie chart
+plt.figure(figsize=(10, 8))
+contributions.plot(kind='pie', autopct='%1.1f%%', startangle=90, counterclock=False, labels=contributions.index)
+plt.title(f'Contribution of Each Product by {field_name}')
+plt.ylabel('')  # Hide y-axis label for clarity
+plt.show()
 
 # Convert to EPDx format
 epdx_products = product_data.to_epdx()
 ```
 
 ## `ProductStatistics` Class
 
@@ -235,41 +245,64 @@
 
 #### Data Filtering and Transformation
 
 - `remove_outliers_from_df(self, filtered_df, field, method, sqrt_tranf)`: Removes outliers from the DataFrame based on the specified field and method, optionally applying a square root transformation for variance stabilization.
 - `filter_dataframe_based_on_field(self, field, filters=None, include_estimated_values=False, remove_outliers=True, method='IQR', sqrt_tranf=True)`: Filters the DataFrame based on specified criteria, including the treatment of estimated values and outliers.
 
 #### Plotting and Visualization
-
-- `plot_histogram(self, df, field)`: Generates a histogram for the specified field, visualizing the distribution of values.
-- `get_field_distribution(self, field, filters=None, include_estimated_values=False, remove_outliers=True, method='IQR', sqrt_tranf=True)`: Filters the DataFrame and plots the distribution of the specified field, offering insights into the data's structure.
-- `plot_distribution_boxplot(self, df, field, group_by_field)`: Creates a boxplot for the specified field, grouped by another field, highlighting the variance and distribution within the data.
+- `get_product_contributions(products_info, 'material_facts.manufacturing')`: Takes a dictionary with product ids as keys and values a dictionary with unit and amount and for an LCA field calculates the percentage contribution of carbon emissions.
+- `get_field_distribution(self, field, filters=None, include_estimated_values=False, remove_outliers=True, method='IQR', sqrt_tranf=True)`: Filters the DataFrame and returns the distribution of the specified field, offering insights into the data's structure.
 - `get_field_distribution_boxplot(self, field, group_by_field, filters=None, include_estimated_values=False, remove_outliers=True, method='IQR', sqrt_tranf=True)`: Filters the DataFrame and generates a boxplot for the specified field, providing a visual representation of statistical distributions.
 
 ## Usage Example
 
 ```
-# Create ProductStatistics (extension of ProductData)
-stats_obj = ProductStatistics(product_data.dataframe, unit='m2')
+import matplotlib.pyplot as plt
 
-# Choose fields to group by
-group_by = [
-    'country',
-    'manufacturing_continent',
-]
+def plot_histogram(df, field):
+    bin_count = min(len(df[field].unique()), 50)  # Limit the number of bins to a maximum of 50
+    plt.figure(figsize=(10, 6))
+    n, bins, patches = plt.hist(df[field], bins=bin_count, color='#2ab0ff', alpha=0.7, rwidth=0.85)
+    plt.grid(axis='y', alpha=0.75)
+    plt.xlabel('Value', fontsize=15)
+    plt.ylabel('Frequency', fontsize=15)
+    plt.xticks(fontsize=12)
+    plt.yticks(fontsize=12)
+    plt.title(f'Distribution of {field}', fontsize=15)
+    plt.axvline(x=df[field].mean(), color='r', linestyle='-', label=f'Mean: {df[field].mean():.4f}')
+    plt.axvline(x=df[field].median(), color='m', linestyle='-', label=f'Median: {df[field].median():.4f}')
+    plt.legend(loc='upper right')
+    plt.show()
 
-# Get all available fields
-all_available_fields  = stats_obj.get_available_fields()
-
-# Calculate statistics dataframe
-stat_df = stats_obj.get_statistics(group_by=group_by, fields=all_available_fields, statistical_metrics=['count', 'mean', 'median'], include_estimated_values=False, remove_outliers=True, method='IQR', sqrt_tranf=True, min_count=3)
-
-# Apply further filters and get field distribution
 filters = {
     'material_type':'Ceramic',
+    # 'elements_nrm_1':'3.1 - Wall finishes'
 }
-stats_obj.get_field_distribution(field='material_facts.manufacturing', filters=filters, include_estimated_values=True, remove_outliers=False, method='IQR', sqrt_tranf=True)
+field = 'material_facts.manufacturing'
+df = stats_obj.get_field_distribution(field=field, filters=filters, include_estimated_values=True, remove_outliers=False, method='IQR', sqrt_tranf=True)
+
+plot_histogram(df, field)
 
-# Get field distribution boxplot for all product types
-stats_obj.get_field_distribution_boxplot(field='material_facts.manufacturing', group_by_field='product_type', filters=None, include_estimated_values=True, remove_outliers=True, method='IQR', sqrt_tranf=True)
+# With removing outliers
+field = 'material_facts.manufacturing'
+df = stats_obj.get_field_distribution(field=field, filters=filters, include_estimated_values=True, remove_outliers=True, method='IQR', sqrt_tranf=True)
+
+plot_histogram(df, field)
+
+# Field distribution boxplot
+field='material_facts.manufacturing'
+group_by_field = 'product_type'
+# Get a dict with keys product types and values dataframe series 
+grouped_data_dict = stats_obj.get_field_distribution_boxplot(field=field, group_by_field=group_by_field, filters=None, include_estimated_values=True, remove_outliers=True, method='IQR', sqrt_tranf=True)
+
+# Box-plotting
+plt.figure(figsize=(10, 6))
+plt.boxplot(grouped_data_dict.values(), patch_artist=True, labels=grouped_data_dict.keys())
+plt.grid(axis='y', alpha=0.75)
+plt.xlabel(group_by_field, fontsize=15)
+plt.ylabel('Value', fontsize=15)
+plt.xticks(fontsize=12, rotation=45)  # Rotate labels if there are many groups
+plt.yticks(fontsize=12)
+plt.title(f'Distribution of {field} by {group_by_field}', fontsize=15)
+plt.show()
 ```
```

### Comparing `aecdata-0.0.3/setup.py` & `aecdata-0.0.4/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="aecdata",
-    version="0.0.3",
+    version="0.0.4",
     author="2050 Materials",
     license="Apache License 2.0",
     author_email="nicodemos@2050-materials.com",
     description="A Python library designed to simplify access to the 2050-materials API",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/2050-Materials/aecdata",
@@ -16,11 +16,10 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "requests",
         "numpy",
         "pandas",
-        "matplotlib",
         "pyarrow",
     ]
 )
```


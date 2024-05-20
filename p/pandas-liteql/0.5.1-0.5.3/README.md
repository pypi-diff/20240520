# Comparing `tmp/pandas-liteql-0.5.1.tar.gz` & `tmp/pandas_liteql-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\GitHub\pandas-liteql\dist\.tmp-p3aoimi4\pandas-liteql-0.5.1.tar", last modified: Mon Oct 16 04:04:22 2023, max compression
+gzip compressed data, was "pandas_liteql-0.5.3.tar", last modified: Mon May 20 04:56:22 2024, max compression
```

## Comparing `pandas-liteql-0.5.1.tar` & `pandas_liteql-0.5.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-10-16 04:04:22.000000 pandas-liteql-0.5.1/
--rw-rw-rw-   0        0        0     1092 2023-09-06 00:50:38.000000 pandas-liteql-0.5.1/LICENSE
--rw-rw-rw-   0        0        0     5950 2023-10-16 04:04:22.000000 pandas-liteql-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     4901 2023-10-16 04:03:37.000000 pandas-liteql-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-10-16 04:04:22.000000 pandas-liteql-0.5.1/pandas_liteql/
--rw-rw-rw-   0        0        0       23 2023-10-15 03:43:37.000000 pandas-liteql-0.5.1/pandas_liteql/__init__.py
--rw-rw-rw-   0        0        0     3527 2023-10-16 03:32:38.000000 pandas-liteql-0.5.1/pandas_liteql/liteql.py
-drwxrwxrwx   0        0        0        0 2023-10-16 04:04:22.000000 pandas-liteql-0.5.1/pandas_liteql.egg-info/
--rw-rw-rw-   0        0        0     5950 2023-10-16 04:04:22.000000 pandas-liteql-0.5.1/pandas_liteql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-10-16 04:04:22.000000 pandas-liteql-0.5.1/pandas_liteql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-16 04:04:22.000000 pandas-liteql-0.5.1/pandas_liteql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-10-16 04:04:22.000000 pandas-liteql-0.5.1/pandas_liteql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-10-16 04:04:22.000000 pandas-liteql-0.5.1/pandas_liteql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-16 04:04:22.000000 pandas-liteql-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1723 2023-10-16 03:59:43.000000 pandas-liteql-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 04:56:22.748590 pandas_liteql-0.5.3/
+-rw-rw-rw-   0        0        0     1092 2023-09-06 00:50:38.000000 pandas_liteql-0.5.3/LICENSE
+-rw-rw-rw-   0        0        0     6194 2024-05-20 04:56:22.748590 pandas_liteql-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4711 2024-05-20 04:43:24.000000 pandas_liteql-0.5.3/README.md
+-rw-rw-rw-   0        0        0     1817 2024-05-20 04:51:28.000000 pandas_liteql-0.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 04:56:22.748590 pandas_liteql-0.5.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 04:56:22.738591 pandas_liteql-0.5.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-20 04:56:22.741591 pandas_liteql-0.5.3/src/pandas_liteql/
+-rw-rw-rw-   0        0        0       23 2023-10-15 03:43:37.000000 pandas_liteql-0.5.3/src/pandas_liteql/__init__.py
+-rw-rw-rw-   0        0        0     3915 2023-10-17 00:07:14.000000 pandas_liteql-0.5.3/src/pandas_liteql/liteql.py
+drwxrwxrwx   0        0        0        0 2024-05-20 04:56:22.747590 pandas_liteql-0.5.3/src/pandas_liteql.egg-info/
+-rw-rw-rw-   0        0        0     6194 2024-05-20 04:56:22.000000 pandas_liteql-0.5.3/src/pandas_liteql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2024-05-20 04:56:22.000000 pandas_liteql-0.5.3/src/pandas_liteql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 04:56:22.000000 pandas_liteql-0.5.3/src/pandas_liteql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-20 04:56:22.000000 pandas_liteql-0.5.3/src/pandas_liteql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-20 04:56:22.000000 pandas_liteql-0.5.3/src/pandas_liteql.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pandas-liteql-0.5.1/LICENSE` & `pandas_liteql-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-liteql-0.5.1/PKG-INFO` & `pandas_liteql-0.5.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 Metadata-Version: 2.1
 Name: pandas-liteql
-Version: 0.5.1
-Summary: A simple pandas extension that enables users to execute SQL statements against DataFrames using 
-Home-page: https://github.com/forgineer/pandas-liteql
-Author: forgineer
+Version: 0.5.3
+Summary: A simple pandas extension that enables users to execute SQL statements against DataFrames using in-memory SQLite.
+Author-email: forgineer <blake.phillips86@gmail.com>
 License: MIT License
+Project-URL: Homepage, https://github.com/forgineer/pandas-liteql
+Project-URL: Documentation, https://github.com/forgineer/pandas-liteql
+Project-URL: Repository, https://github.com/forgineer/pandas-liteql
+Project-URL: Issues, https://github.com/forgineer/pandas-liteql/issues
 Keywords: dataframe,pandas,sql,sqlite
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 7 - Inactive
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: pypi_deployment
 License-File: LICENSE
+Requires-Dist: pandas>=1.3.5
+Requires-Dist: sqlalchemy>=1.4.36
+Provides-Extra: pypi-deploy
+Requires-Dist: build; extra == "pypi-deploy"
+Requires-Dist: twine; extra == "pypi-deploy"
 
 <div align="center">
-    <img src="https://forgineer.pythonanywhere.com/static/pandas_liteql/pandas-liteql-logo.png" alt="pandas-liteql-logo.png"><br>
+    <img src="https://forgineer.pythonanywhere.com/static/pandas_liteql/pandas-liteql-feather-logo-large.png" alt="pandas-liteql-logo.png"><br>
 </div>
 
 ---
 
 # What is pandas-liteql?
 **pandas-liteql** is a simple [pandas](https://pandas.pydata.org/) extension that enables users to execute SQL statements against DataFrames using in-memory [SQLite](https://www.sqlite.org/index.html). It is meant to streamline data manipulation and analysis tasks. For more detailed information and examples on **pandas-liteql**, visit the [documentation pages](https://forgineer.pythonanywhere.com/pandas-liteql).
 
@@ -46,22 +53,22 @@
 Assuming these prerequisites are already installed, adding **pandas-liteql** is as simple as...
 
 ```
 pip install pandas-liteql
 ```
 
 # Examples
-Below are some usage examples to load, query, and drop data from the in-memory SQLite sessions established with **pandas-liteql** and pandas DataFrame integration. For more in-depth information and examples visit the [documentation pages](https://forgineer.pythonanywhere.com/pandas-liteql).
+Below are some usage examples to load, query, and drop data from the in-memory SQLite sessions established with **pandas-liteql** and pandas DataFrame integration.
 
 ## Loading
 Start by loading your DataFrame with the `load` function. When **pandas-liteql** is imported, an in-memory SQLite session is created where data can be loaded to.
 
 ```python
 import pandas as pd
-import pandas_liteql as lql
+from src import pandas_liteql as lql
 
 # Data set creation
 person_data = {
     'name': ['Bill', 'Ted', 'Abraham', 'Genghis', 'Napoleon'],
     'age': [25, 24, 56, 64, 51],
     'email': ['bill@excellent.com', 'ted@excellent.com',
               'lincoln@excellent.com', 'khan@excellent.com',
@@ -141,8 +148,8 @@
    index  name  age               email
 0      0  Bill   25  bill@excellent.com
 1      1   Ted   24   ted@excellent.com
 ```
 
 
 # Contributing
-Contributions are welcome via pull request from a fork. Log issues if any bugs are found or if you have some good ideas of how this project could be expanded on. Depending on interest, other contributors could be added to meet the demand in features.
+Currently, **pandas-liteql** will not be receiving any additional updates. Contributions will not be accepted here, but feel free to fork this project if you desire.
```

### Comparing `pandas-liteql-0.5.1/README.md` & `pandas_liteql-0.5.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <div align="center">
-    <img src="https://forgineer.pythonanywhere.com/static/pandas_liteql/pandas-liteql-logo.png" alt="pandas-liteql-logo.png"><br>
+    <img src="https://forgineer.pythonanywhere.com/static/pandas_liteql/pandas-liteql-feather-logo-large.png" alt="pandas-liteql-logo.png"><br>
 </div>
 
 ---
 
 # What is pandas-liteql?
 **pandas-liteql** is a simple [pandas](https://pandas.pydata.org/) extension that enables users to execute SQL statements against DataFrames using in-memory [SQLite](https://www.sqlite.org/index.html). It is meant to streamline data manipulation and analysis tasks. For more detailed information and examples on **pandas-liteql**, visit the [documentation pages](https://forgineer.pythonanywhere.com/pandas-liteql).
 
@@ -21,22 +21,22 @@
 Assuming these prerequisites are already installed, adding **pandas-liteql** is as simple as...
 
 ```
 pip install pandas-liteql
 ```
 
 # Examples
-Below are some usage examples to load, query, and drop data from the in-memory SQLite sessions established with **pandas-liteql** and pandas DataFrame integration. For more in-depth information and examples visit the [documentation pages](https://forgineer.pythonanywhere.com/pandas-liteql).
+Below are some usage examples to load, query, and drop data from the in-memory SQLite sessions established with **pandas-liteql** and pandas DataFrame integration.
 
 ## Loading
 Start by loading your DataFrame with the `load` function. When **pandas-liteql** is imported, an in-memory SQLite session is created where data can be loaded to.
 
 ```python
 import pandas as pd
-import pandas_liteql as lql
+from src import pandas_liteql as lql
 
 # Data set creation
 person_data = {
     'name': ['Bill', 'Ted', 'Abraham', 'Genghis', 'Napoleon'],
     'age': [25, 24, 56, 64, 51],
     'email': ['bill@excellent.com', 'ted@excellent.com',
               'lincoln@excellent.com', 'khan@excellent.com',
@@ -116,8 +116,8 @@
    index  name  age               email
 0      0  Bill   25  bill@excellent.com
 1      1   Ted   24   ted@excellent.com
 ```
 
 
 # Contributing
-Contributions are welcome via pull request from a fork. Log issues if any bugs are found or if you have some good ideas of how this project could be expanded on. Depending on interest, other contributors could be added to meet the demand in features.
+Currently, **pandas-liteql** will not be receiving any additional updates. Contributions will not be accepted here, but feel free to fork this project if you desire.
```

### Comparing `pandas-liteql-0.5.1/pandas_liteql/liteql.py` & `pandas_liteql-0.5.3/src/pandas_liteql/liteql.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     def __init__(self, table_name: str):
         self.name = table_name
 
         liteql_inspect = sqlalchemy.inspect(LITEQL_ENGINE)
         columns_table = liteql_inspect.get_columns(table_name)
 
-        self.schema = pandas.DataFrame.from_dict(columns_table)
+        self.schema = pandas.DataFrame(columns_table)
 
     def log_schema(self):
         schema_str = self.schema.to_string()
 
         for schema_line in schema_str.splitlines():
             logging.debug(schema_line)
 
@@ -68,23 +68,29 @@
 def drop(table_name: str) -> None:
     """
     Drops the table from the SQLite in-memory session (if exists).
 
     :param table_name: The name of the loaded SQLite table.
     :return: None.
     """
-    LITEQL_ENGINE.execute(f'DROP TABLE IF EXISTS {table_name}')
+    if int(sqlalchemy.__version__[:1]) < 2:
+        LITEQL_ENGINE.execute(f'DROP TABLE IF EXISTS {table_name}')
+    else:
+        with LITEQL_ENGINE.connect() as connection:
+            connection.execute(sqlalchemy.text(f'DROP TABLE IF EXISTS {table_name}'))
 
 
 @liteql_logger
 def query(sql: str, *drop_tables, **pandas_args) -> pandas.DataFrame:
     """
     Queries the SQLite in-memory session.
 
     :param sql: An SQLite compatible SQL string.
+    :param *drop_tables: A list of tables (as args) to be dropped after the query has completed.
+    :param **pandas_args: Additional pandas keyword arguments related to the pandas.to_sql method.
     :return: A pandas DataFrame containing the queried data.
     """
     # Remove the 'sql' or 'con' arguments if somehow included in 'pandas_args'
     pandas_args.pop('sql', None)
     pandas_args.pop('con', None)
 
     data = pandas.read_sql(sql=sql, con=LITEQL_ENGINE, **pandas_args)
```

### Comparing `pandas-liteql-0.5.1/pandas_liteql.egg-info/PKG-INFO` & `pandas_liteql-0.5.3/src/pandas_liteql.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 Metadata-Version: 2.1
 Name: pandas-liteql
-Version: 0.5.1
-Summary: A simple pandas extension that enables users to execute SQL statements against DataFrames using 
-Home-page: https://github.com/forgineer/pandas-liteql
-Author: forgineer
+Version: 0.5.3
+Summary: A simple pandas extension that enables users to execute SQL statements against DataFrames using in-memory SQLite.
+Author-email: forgineer <blake.phillips86@gmail.com>
 License: MIT License
+Project-URL: Homepage, https://github.com/forgineer/pandas-liteql
+Project-URL: Documentation, https://github.com/forgineer/pandas-liteql
+Project-URL: Repository, https://github.com/forgineer/pandas-liteql
+Project-URL: Issues, https://github.com/forgineer/pandas-liteql/issues
 Keywords: dataframe,pandas,sql,sqlite
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 7 - Inactive
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: pypi_deployment
 License-File: LICENSE
+Requires-Dist: pandas>=1.3.5
+Requires-Dist: sqlalchemy>=1.4.36
+Provides-Extra: pypi-deploy
+Requires-Dist: build; extra == "pypi-deploy"
+Requires-Dist: twine; extra == "pypi-deploy"
 
 <div align="center">
-    <img src="https://forgineer.pythonanywhere.com/static/pandas_liteql/pandas-liteql-logo.png" alt="pandas-liteql-logo.png"><br>
+    <img src="https://forgineer.pythonanywhere.com/static/pandas_liteql/pandas-liteql-feather-logo-large.png" alt="pandas-liteql-logo.png"><br>
 </div>
 
 ---
 
 # What is pandas-liteql?
 **pandas-liteql** is a simple [pandas](https://pandas.pydata.org/) extension that enables users to execute SQL statements against DataFrames using in-memory [SQLite](https://www.sqlite.org/index.html). It is meant to streamline data manipulation and analysis tasks. For more detailed information and examples on **pandas-liteql**, visit the [documentation pages](https://forgineer.pythonanywhere.com/pandas-liteql).
 
@@ -46,22 +53,22 @@
 Assuming these prerequisites are already installed, adding **pandas-liteql** is as simple as...
 
 ```
 pip install pandas-liteql
 ```
 
 # Examples
-Below are some usage examples to load, query, and drop data from the in-memory SQLite sessions established with **pandas-liteql** and pandas DataFrame integration. For more in-depth information and examples visit the [documentation pages](https://forgineer.pythonanywhere.com/pandas-liteql).
+Below are some usage examples to load, query, and drop data from the in-memory SQLite sessions established with **pandas-liteql** and pandas DataFrame integration.
 
 ## Loading
 Start by loading your DataFrame with the `load` function. When **pandas-liteql** is imported, an in-memory SQLite session is created where data can be loaded to.
 
 ```python
 import pandas as pd
-import pandas_liteql as lql
+from src import pandas_liteql as lql
 
 # Data set creation
 person_data = {
     'name': ['Bill', 'Ted', 'Abraham', 'Genghis', 'Napoleon'],
     'age': [25, 24, 56, 64, 51],
     'email': ['bill@excellent.com', 'ted@excellent.com',
               'lincoln@excellent.com', 'khan@excellent.com',
@@ -141,8 +148,8 @@
    index  name  age               email
 0      0  Bill   25  bill@excellent.com
 1      1   Ted   24   ted@excellent.com
 ```
 
 
 # Contributing
-Contributions are welcome via pull request from a fork. Log issues if any bugs are found or if you have some good ideas of how this project could be expanded on. Depending on interest, other contributors could be added to meet the demand in features.
+Currently, **pandas-liteql** will not be receiving any additional updates. Contributions will not be accepted here, but feel free to fork this project if you desire.
```


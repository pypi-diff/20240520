# Comparing `tmp/portfolio_tracker-0.2.0.1.tar.gz` & `tmp/portfolio_tracker-0.2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portfolio_tracker-0.2.0.1.tar", last modified: Mon May 20 16:33:33 2024, max compression
+gzip compressed data, was "portfolio_tracker-0.2.0.2.tar", last modified: Mon May 20 16:35:48 2024, max compression
```

## Comparing `portfolio_tracker-0.2.0.1.tar` & `portfolio_tracker-0.2.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 16:33:33.221045 portfolio_tracker-0.2.0.1/
--rw-rw-rw-   0        0        0     3357 2024-05-20 16:33:33.219046 portfolio_tracker-0.2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2892 2024-05-12 11:24:33.000000 portfolio_tracker-0.2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 16:33:33.208045 portfolio_tracker-0.2.0.1/portfolio_tracker/
--rw-rw-rw-   0        0        0      131 2024-05-20 16:33:24.000000 portfolio_tracker-0.2.0.1/portfolio_tracker/__init__.py
--rw-rw-rw-   0        0        0    17732 2024-05-20 16:31:04.000000 portfolio_tracker-0.2.0.1/portfolio_tracker/manager.py
--rw-rw-rw-   0        0        0     4655 2024-05-12 09:13:01.000000 portfolio_tracker-0.2.0.1/portfolio_tracker/price_repo.py
--rw-rw-rw-   0        0        0     4118 2024-05-12 09:07:54.000000 portfolio_tracker-0.2.0.1/portfolio_tracker/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:33:33.218047 portfolio_tracker-0.2.0.1/portfolio_tracker.egg-info/
--rw-rw-rw-   0        0        0     3357 2024-05-20 16:33:32.000000 portfolio_tracker-0.2.0.1/portfolio_tracker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2024-05-20 16:33:33.000000 portfolio_tracker-0.2.0.1/portfolio_tracker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 16:33:32.000000 portfolio_tracker-0.2.0.1/portfolio_tracker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-20 16:33:32.000000 portfolio_tracker-0.2.0.1/portfolio_tracker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-20 16:33:32.000000 portfolio_tracker-0.2.0.1/portfolio_tracker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 16:33:33.221045 portfolio_tracker-0.2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      898 2024-05-20 16:33:24.000000 portfolio_tracker-0.2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:35:48.599992 portfolio_tracker-0.2.0.2/
+-rw-rw-rw-   0        0        0     3397 2024-05-20 16:35:48.597991 portfolio_tracker-0.2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2931 2024-05-20 16:35:40.000000 portfolio_tracker-0.2.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 16:35:48.589991 portfolio_tracker-0.2.0.2/portfolio_tracker/
+-rw-rw-rw-   0        0        0      131 2024-05-20 16:35:41.000000 portfolio_tracker-0.2.0.2/portfolio_tracker/__init__.py
+-rw-rw-rw-   0        0        0    17732 2024-05-20 16:31:04.000000 portfolio_tracker-0.2.0.2/portfolio_tracker/manager.py
+-rw-rw-rw-   0        0        0     4655 2024-05-12 09:13:01.000000 portfolio_tracker-0.2.0.2/portfolio_tracker/price_repo.py
+-rw-rw-rw-   0        0        0     4118 2024-05-12 09:07:54.000000 portfolio_tracker-0.2.0.2/portfolio_tracker/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:35:48.595993 portfolio_tracker-0.2.0.2/portfolio_tracker.egg-info/
+-rw-rw-rw-   0        0        0     3397 2024-05-20 16:35:48.000000 portfolio_tracker-0.2.0.2/portfolio_tracker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2024-05-20 16:35:48.000000 portfolio_tracker-0.2.0.2/portfolio_tracker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 16:35:48.000000 portfolio_tracker-0.2.0.2/portfolio_tracker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-20 16:35:48.000000 portfolio_tracker-0.2.0.2/portfolio_tracker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-20 16:35:48.000000 portfolio_tracker-0.2.0.2/portfolio_tracker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 16:35:48.599992 portfolio_tracker-0.2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      898 2024-05-20 16:35:40.000000 portfolio_tracker-0.2.0.2/setup.py
```

### Comparing `portfolio_tracker-0.2.0.1/PKG-INFO` & `portfolio_tracker-0.2.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolio_tracker
-Version: 0.2.0.1
+Version: 0.2.0.2
 Summary: A portfolio tracker library, that allows to track a portfolio of stocks and their performance.
 Author: Poli Luca
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: yfinance
 Requires-Dist: numpy
@@ -65,16 +65,17 @@
 # Rebalance the portfolio
 portfolio_path2 = os.path.join(PORTFOLIOS_PATH, "portfolio_01_2024.xlsx")
 portfolio.rebalancing_from_file(portfolio_path2)
 
 # We can roll again the portfolio forward
 portfolio.roll_forward(20)
 
-# Print the weights and returns
-print(portfolio.get_weights(normalize=True))
+# Print the weights, assets values and returns
+print(portfolio.get_weights())
+print(portfolio.get_assets_values())
 print(portfolio.get_returns(weighted=True))
 ```
 
 For more examples, check the `example.ipynb` notebook.
 
 
 ## Development
```

### Comparing `portfolio_tracker-0.2.0.1/README.md` & `portfolio_tracker-0.2.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,17 @@
 # Rebalance the portfolio
 portfolio_path2 = os.path.join(PORTFOLIOS_PATH, "portfolio_01_2024.xlsx")
 portfolio.rebalancing_from_file(portfolio_path2)
 
 # We can roll again the portfolio forward
 portfolio.roll_forward(20)
 
-# Print the weights and returns
-print(portfolio.get_weights(normalize=True))
+# Print the weights, assets values and returns
+print(portfolio.get_weights())
+print(portfolio.get_assets_values())
 print(portfolio.get_returns(weighted=True))
 ```
 
 For more examples, check the `example.ipynb` notebook.
 
 
 ## Development
```

### Comparing `portfolio_tracker-0.2.0.1/portfolio_tracker/manager.py` & `portfolio_tracker-0.2.0.2/portfolio_tracker/manager.py`

 * *Files identical despite different names*

### Comparing `portfolio_tracker-0.2.0.1/portfolio_tracker/price_repo.py` & `portfolio_tracker-0.2.0.2/portfolio_tracker/price_repo.py`

 * *Files identical despite different names*

### Comparing `portfolio_tracker-0.2.0.1/portfolio_tracker/utils.py` & `portfolio_tracker-0.2.0.2/portfolio_tracker/utils.py`

 * *Files identical despite different names*

### Comparing `portfolio_tracker-0.2.0.1/portfolio_tracker.egg-info/PKG-INFO` & `portfolio_tracker-0.2.0.2/portfolio_tracker.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolio-tracker
-Version: 0.2.0.1
+Version: 0.2.0.2
 Summary: A portfolio tracker library, that allows to track a portfolio of stocks and their performance.
 Author: Poli Luca
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: yfinance
 Requires-Dist: numpy
@@ -65,16 +65,17 @@
 # Rebalance the portfolio
 portfolio_path2 = os.path.join(PORTFOLIOS_PATH, "portfolio_01_2024.xlsx")
 portfolio.rebalancing_from_file(portfolio_path2)
 
 # We can roll again the portfolio forward
 portfolio.roll_forward(20)
 
-# Print the weights and returns
-print(portfolio.get_weights(normalize=True))
+# Print the weights, assets values and returns
+print(portfolio.get_weights())
+print(portfolio.get_assets_values())
 print(portfolio.get_returns(weighted=True))
 ```
 
 For more examples, check the `example.ipynb` notebook.
 
 
 ## Development
```

### Comparing `portfolio_tracker-0.2.0.1/setup.py` & `portfolio_tracker-0.2.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 import codecs
 
 # version = '{{VERSION_PLACEHOLDER}}'
-version = '0.2.0.1'
+version = '0.2.0.2'
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='portfolio_tracker',
```


# Comparing `tmp/mercapy-0.1.0.tar.gz` & `tmp/mercapy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercapy-0.1.0.tar", last modified: Sat May 18 21:48:41 2024, max compression
+gzip compressed data, was "mercapy-0.2.0.tar", last modified: Mon May 20 21:21:05 2024, max compression
```

## Comparing `mercapy-0.1.0.tar` & `mercapy-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:48:41.885901 mercapy-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-18 21:48:36.000000 mercapy-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-18 21:48:41.885901 mercapy-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-18 21:48:36.000000 mercapy-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:48:41.881901 mercapy-0.1.0/mercapy/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-18 21:48:36.000000 mercapy-0.1.0/mercapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-18 21:48:36.000000 mercapy-0.1.0/mercapy/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:48:41.881901 mercapy-0.1.0/mercapy/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 21:48:36.000000 mercapy-0.1.0/mercapy/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-18 21:48:36.000000 mercapy-0.1.0/mercapy/exceptions/product.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-18 21:48:36.000000 mercapy-0.1.0/mercapy/merca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:48:41.881901 mercapy-0.1.0/mercapy/product/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-18 21:48:36.000000 mercapy-0.1.0/mercapy/product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-18 21:48:36.000000 mercapy-0.1.0/mercapy/product/photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-18 21:48:36.000000 mercapy-0.1.0/mercapy/product/product.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:48:41.881901 mercapy-0.1.0/mercapy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 21:48:36.000000 mercapy-0.1.0/mercapy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-18 21:48:36.000000 mercapy-0.1.0/mercapy/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-18 21:48:36.000000 mercapy-0.1.0/mercapy/utils/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:48:41.885901 mercapy-0.1.0/mercapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-18 21:48:41.000000 mercapy-0.1.0/mercapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-18 21:48:41.000000 mercapy-0.1.0/mercapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 21:48:41.000000 mercapy-0.1.0/mercapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-18 21:48:41.000000 mercapy-0.1.0/mercapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-18 21:48:41.000000 mercapy-0.1.0/mercapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 21:48:41.885901 mercapy-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-18 21:48:36.000000 mercapy-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:21:05.793660 mercapy-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-20 21:21:00.000000 mercapy-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-20 21:21:05.793660 mercapy-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-20 21:21:00.000000 mercapy-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:21:05.789661 mercapy-0.2.0/mercapy/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:21:05.789661 mercapy-0.2.0/mercapy/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/elements/photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/elements/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/elements/season.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/merca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:21:05.793660 mercapy-0.2.0/mercapy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/utils/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/utils/warehouses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:21:05.793660 mercapy-0.2.0/mercapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-20 21:21:05.000000 mercapy-0.2.0/mercapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-20 21:21:05.000000 mercapy-0.2.0/mercapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:21:05.000000 mercapy-0.2.0/mercapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 21:21:05.000000 mercapy-0.2.0/mercapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 21:21:05.000000 mercapy-0.2.0/mercapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 21:21:05.793660 mercapy-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-20 21:21:00.000000 mercapy-0.2.0/setup.py
```

### Comparing `mercapy-0.1.0/LICENSE` & `mercapy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mercapy-0.1.0/PKG-INFO` & `mercapy-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mercapy
-Version: 0.1.0
-Summary: A Mercadona SDK for Python to track product prices, amounts, and more.
+Version: 0.2.0
+Summary: A Mercadona interface for Python to track product prices, amounts, and more.
 Author: Joel Taylor
 Author-email: contact@joeltaylor.business
 License: MIT
 Keywords: mercadona,api,sdk,data science,prices,information
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.12
@@ -18,15 +18,15 @@
   <br>
   <img src="https://github.com/jtayped/mercapy/blob/main/images/logo.png?raw=true" alt="mercapy" width="200">
   <br>
   🛍️ mercapy
   <br>
 </h1>
 
-<h4 align="center">A Mercadona SDK for Python to track product prices, amounts, and more.</h4>
+<h4 align="center">A Mercadona interface for Python to track product prices, amounts, and more.</h4>
 
 <div align="center">
   <a href="https://pypi.org/project/mercapy/">
     <img src="https://img.shields.io/pypi/v/mercapy?style=for-the-badge">
   </a>
   <a href="https://github.com/jtayped/mercapy/blob/main/LICENSE">
     <img src="https://img.shields.io/github/license/jtayped/mercapy?style=for-the-badge" alt="License">
@@ -40,40 +40,65 @@
 </div>
 
 <div align="center">
   <a href="#how-to-use">How to use it</a> •
   <a href="#related">Related</a>
 </div>
 
-
 ## 🔧 How to use it
 
 First of all, install the package using:
 
 ```bash
 pip install mercapy
 ```
 
-Now you can start tracking multiple product's prices, availability, weight, etc.
+By initializing the mercadona class, you can search products, recommendations, and new arrivals:
+
+```python
+from mercapy import Mercadona
+
+mercadona = Mercadona()
+
+mercadona.search("galletas")
+mercadona.get_new_arrivals()
+mercadona.get_home_recommendations()
+```
+
+Each product has statistics such as:
+
 ```python
 from mercapy import Product
 
-water = Product("27335")
-print(water.ean)
-print(water.price)
-print(water.origin)
+# Find product by ID
+prod = Product("12345")
+
+prod.name               # Beer
+prod.unit_price         # 1.25€
+prod.previos_price      # 1.95€
+prod.is_discounted      # True
+prod.bulk_price         # 7.5€
+prod.is_pack            # True
+prod.weight             # 0.5kg
+prod.age_check          # True
+prod.alcohol_by_volume  # 3.2%
+prod.iva                # 21%
 ```
 
-And you can also get other recommended products:
+You can also interact with product photos:
+
 ```python
-# Get recommended product's prices
-recommeded = water.get_recommended()
-for product in recommeded:
-    print(product.price)
+from mercapy import Product
+
+# Find product by ID
+prod = Product("12345")
+prod.images[0].save("product.png", width=1920, height=1080)
 ```
 
+More docs coming soon...
+
 <div id="related"></div>
 
 ## 🙋‍♂️ You may also like...
 
-- [📷📱 pygramcore](https://github.com/jtayped/pygramcore) - A simple-to-use Instagram SDK for Python using Selenium.
+- [📷📱 pygramcore](https://github.com/jtayped/pygramcore) - A simple-to-use Instagram interface for Python using Selenium.
 - [🧑‍💼My Portfolio](https://joeltaylor.business) - Check out my front-end and SEO skills on my Portfolio!
```

#### html2text {}

```diff
@@ -1,27 +1,34 @@
-Metadata-Version: 2.1 Name: mercapy Version: 0.1.0 Summary: A Mercadona SDK for
-Python to track product prices, amounts, and more. Author: Joel Taylor Author-
-email: contact@joeltaylor.business License: MIT Keywords:
+Metadata-Version: 2.1 Name: mercapy Version: 0.2.0 Summary: A Mercadona
+interface for Python to track product prices, amounts, and more. Author: Joel
+Taylor Author-email: contact@joeltaylor.business License: MIT Keywords:
 mercadona,api,sdk,data science,prices,information Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.12 Classifier: Programming Language ::
 Python :: Implementation :: CPython Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: requests
                                     ************
                                    [[mmeerrccaappyy]]
                                 ?ð????ï?¸? mmeerrccaappyy
                                      ************
-****** AA MMeerrccaaddoonnaa SSDDKK ffoorr PPyytthhoonn ttoo ttrraacckk pprroodduucctt pprriicceess,, aammoouunnttss,, aanndd mmoorree.. ******
+  ****** AA MMeerrccaaddoonnaa iinntteerrffaaccee ffoorr PPyytthhoonn ttoo ttrraacckk pprroodduucctt pprriicceess,, aammoouunnttss,, aanndd
+                                   mmoorree.. ******
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_m_e_r_c_a_p_y_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_L_i_c_e_n_s_e_]_[_L_i_c_e_n_s_e_]
                                   _[_L_i_n_k_e_d_I_n_]
                            _H_o_w_ _t_o_ _u_s_e_ _i_t â¢ _R_e_l_a_t_e_d
 ## ð§ How to use it First of all, install the package using: ```bash pip
-install mercapy ``` Now you can start tracking multiple product's prices,
-availability, weight, etc. ```python from mercapy import Product water =
-Product("27335") print(water.ean) print(water.price) print(water.origin) ```
-And you can also get other recommended products: ```python # Get recommended
-product's prices recommeded = water.get_recommended() for product in
-recommeded: print(product.price) ```
+install mercapy ``` By initializing the mercadona class, you can search
+products, recommendations, and new arrivals: ```python from mercapy import
+Mercadona mercadona = Mercadona() mercadona.search("galletas")
+mercadona.get_new_arrivals() mercadona.get_home_recommendations() ``` Each
+product has statistics such as: ```python from mercapy import Product # Find
+product by ID prod = Product("12345") prod.name # Beer prod.unit_price #
+1.25â¬ prod.previos_price # 1.95â¬ prod.is_discounted # True prod.bulk_price
+# 7.5â¬ prod.is_pack # True prod.weight # 0.5kg prod.age_check # True
+prod.alcohol_by_volume # 3.2% prod.iva # 21% ``` You can also interact with
+product photos: ```python from mercapy import Product # Find product by ID prod
+= Product("12345") prod.images[0].save("product.png", width=1920, height=1080)
+``` More docs coming soon...
 ## ðââï¸ You may also like... - [ð·ð± pygramcore](https://
-github.com/jtayped/pygramcore) - A simple-to-use Instagram SDK for Python using
-Selenium. - [ð§âð¼My Portfolio](https://joeltaylor.business) - Check out
-my front-end and SEO skills on my Portfolio!
+github.com/jtayped/pygramcore) - A simple-to-use Instagram interface for Python
+using Selenium. - [ð§âð¼My Portfolio](https://joeltaylor.business) -
+Check out my front-end and SEO skills on my Portfolio!
```

### Comparing `mercapy-0.1.0/README.md` & `mercapy-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   <br>
   <img src="https://github.com/jtayped/mercapy/blob/main/images/logo.png?raw=true" alt="mercapy" width="200">
   <br>
   🛍️ mercapy
   <br>
 </h1>
 
-<h4 align="center">A Mercadona SDK for Python to track product prices, amounts, and more.</h4>
+<h4 align="center">A Mercadona interface for Python to track product prices, amounts, and more.</h4>
 
 <div align="center">
   <a href="https://pypi.org/project/mercapy/">
     <img src="https://img.shields.io/pypi/v/mercapy?style=for-the-badge">
   </a>
   <a href="https://github.com/jtayped/mercapy/blob/main/LICENSE">
     <img src="https://img.shields.io/github/license/jtayped/mercapy?style=for-the-badge" alt="License">
@@ -24,40 +24,65 @@
 </div>
 
 <div align="center">
   <a href="#how-to-use">How to use it</a> •
   <a href="#related">Related</a>
 </div>
 
-
 ## 🔧 How to use it
 
 First of all, install the package using:
 
 ```bash
 pip install mercapy
 ```
 
-Now you can start tracking multiple product's prices, availability, weight, etc.
+By initializing the mercadona class, you can search products, recommendations, and new arrivals:
+
+```python
+from mercapy import Mercadona
+
+mercadona = Mercadona()
+
+mercadona.search("galletas")
+mercadona.get_new_arrivals()
+mercadona.get_home_recommendations()
+```
+
+Each product has statistics such as:
+
 ```python
 from mercapy import Product
 
-water = Product("27335")
-print(water.ean)
-print(water.price)
-print(water.origin)
+# Find product by ID
+prod = Product("12345")
+
+prod.name               # Beer
+prod.unit_price         # 1.25€
+prod.previos_price      # 1.95€
+prod.is_discounted      # True
+prod.bulk_price         # 7.5€
+prod.is_pack            # True
+prod.weight             # 0.5kg
+prod.age_check          # True
+prod.alcohol_by_volume  # 3.2%
+prod.iva                # 21%
 ```
 
-And you can also get other recommended products:
+You can also interact with product photos:
+
 ```python
-# Get recommended product's prices
-recommeded = water.get_recommended()
-for product in recommeded:
-    print(product.price)
+from mercapy import Product
+
+# Find product by ID
+prod = Product("12345")
+prod.images[0].save("product.png", width=1920, height=1080)
 ```
 
+More docs coming soon...
+
 <div id="related"></div>
 
 ## 🙋‍♂️ You may also like...
 
-- [📷📱 pygramcore](https://github.com/jtayped/pygramcore) - A simple-to-use Instagram SDK for Python using Selenium.
+- [📷📱 pygramcore](https://github.com/jtayped/pygramcore) - A simple-to-use Instagram interface for Python using Selenium.
 - [🧑‍💼My Portfolio](https://joeltaylor.business) - Check out my front-end and SEO skills on my Portfolio!
```

#### html2text {}

```diff
@@ -1,19 +1,26 @@
                                     ************
                                    [[mmeerrccaappyy]]
                                 ?ð????ï?¸? mmeerrccaappyy
                                      ************
-****** AA MMeerrccaaddoonnaa SSDDKK ffoorr PPyytthhoonn ttoo ttrraacckk pprroodduucctt pprriicceess,, aammoouunnttss,, aanndd mmoorree.. ******
+  ****** AA MMeerrccaaddoonnaa iinntteerrffaaccee ffoorr PPyytthhoonn ttoo ttrraacckk pprroodduucctt pprriicceess,, aammoouunnttss,, aanndd
+                                   mmoorree.. ******
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_m_e_r_c_a_p_y_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_L_i_c_e_n_s_e_]_[_L_i_c_e_n_s_e_]
                                   _[_L_i_n_k_e_d_I_n_]
                            _H_o_w_ _t_o_ _u_s_e_ _i_t â¢ _R_e_l_a_t_e_d
 ## ð§ How to use it First of all, install the package using: ```bash pip
-install mercapy ``` Now you can start tracking multiple product's prices,
-availability, weight, etc. ```python from mercapy import Product water =
-Product("27335") print(water.ean) print(water.price) print(water.origin) ```
-And you can also get other recommended products: ```python # Get recommended
-product's prices recommeded = water.get_recommended() for product in
-recommeded: print(product.price) ```
+install mercapy ``` By initializing the mercadona class, you can search
+products, recommendations, and new arrivals: ```python from mercapy import
+Mercadona mercadona = Mercadona() mercadona.search("galletas")
+mercadona.get_new_arrivals() mercadona.get_home_recommendations() ``` Each
+product has statistics such as: ```python from mercapy import Product # Find
+product by ID prod = Product("12345") prod.name # Beer prod.unit_price #
+1.25â¬ prod.previos_price # 1.95â¬ prod.is_discounted # True prod.bulk_price
+# 7.5â¬ prod.is_pack # True prod.weight # 0.5kg prod.age_check # True
+prod.alcohol_by_volume # 3.2% prod.iva # 21% ``` You can also interact with
+product photos: ```python from mercapy import Product # Find product by ID prod
+= Product("12345") prod.images[0].save("product.png", width=1920, height=1080)
+``` More docs coming soon...
 ## ðââï¸ You may also like... - [ð·ð± pygramcore](https://
-github.com/jtayped/pygramcore) - A simple-to-use Instagram SDK for Python using
-Selenium. - [ð§âð¼My Portfolio](https://joeltaylor.business) - Check out
-my front-end and SEO skills on my Portfolio!
+github.com/jtayped/pygramcore) - A simple-to-use Instagram interface for Python
+using Selenium. - [ð§âð¼My Portfolio](https://joeltaylor.business) -
+Check out my front-end and SEO skills on my Portfolio!
```

### Comparing `mercapy-0.1.0/mercapy.egg-info/PKG-INFO` & `mercapy-0.2.0/mercapy.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mercapy
-Version: 0.1.0
-Summary: A Mercadona SDK for Python to track product prices, amounts, and more.
+Version: 0.2.0
+Summary: A Mercadona interface for Python to track product prices, amounts, and more.
 Author: Joel Taylor
 Author-email: contact@joeltaylor.business
 License: MIT
 Keywords: mercadona,api,sdk,data science,prices,information
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.12
@@ -18,15 +18,15 @@
   <br>
   <img src="https://github.com/jtayped/mercapy/blob/main/images/logo.png?raw=true" alt="mercapy" width="200">
   <br>
   🛍️ mercapy
   <br>
 </h1>
 
-<h4 align="center">A Mercadona SDK for Python to track product prices, amounts, and more.</h4>
+<h4 align="center">A Mercadona interface for Python to track product prices, amounts, and more.</h4>
 
 <div align="center">
   <a href="https://pypi.org/project/mercapy/">
     <img src="https://img.shields.io/pypi/v/mercapy?style=for-the-badge">
   </a>
   <a href="https://github.com/jtayped/mercapy/blob/main/LICENSE">
     <img src="https://img.shields.io/github/license/jtayped/mercapy?style=for-the-badge" alt="License">
@@ -40,40 +40,65 @@
 </div>
 
 <div align="center">
   <a href="#how-to-use">How to use it</a> •
   <a href="#related">Related</a>
 </div>
 
-
 ## 🔧 How to use it
 
 First of all, install the package using:
 
 ```bash
 pip install mercapy
 ```
 
-Now you can start tracking multiple product's prices, availability, weight, etc.
+By initializing the mercadona class, you can search products, recommendations, and new arrivals:
+
+```python
+from mercapy import Mercadona
+
+mercadona = Mercadona()
+
+mercadona.search("galletas")
+mercadona.get_new_arrivals()
+mercadona.get_home_recommendations()
+```
+
+Each product has statistics such as:
+
 ```python
 from mercapy import Product
 
-water = Product("27335")
-print(water.ean)
-print(water.price)
-print(water.origin)
+# Find product by ID
+prod = Product("12345")
+
+prod.name               # Beer
+prod.unit_price         # 1.25€
+prod.previos_price      # 1.95€
+prod.is_discounted      # True
+prod.bulk_price         # 7.5€
+prod.is_pack            # True
+prod.weight             # 0.5kg
+prod.age_check          # True
+prod.alcohol_by_volume  # 3.2%
+prod.iva                # 21%
 ```
 
-And you can also get other recommended products:
+You can also interact with product photos:
+
 ```python
-# Get recommended product's prices
-recommeded = water.get_recommended()
-for product in recommeded:
-    print(product.price)
+from mercapy import Product
+
+# Find product by ID
+prod = Product("12345")
+prod.images[0].save("product.png", width=1920, height=1080)
 ```
 
+More docs coming soon...
+
 <div id="related"></div>
 
 ## 🙋‍♂️ You may also like...
 
-- [📷📱 pygramcore](https://github.com/jtayped/pygramcore) - A simple-to-use Instagram SDK for Python using Selenium.
+- [📷📱 pygramcore](https://github.com/jtayped/pygramcore) - A simple-to-use Instagram interface for Python using Selenium.
 - [🧑‍💼My Portfolio](https://joeltaylor.business) - Check out my front-end and SEO skills on my Portfolio!
```

#### html2text {}

```diff
@@ -1,27 +1,34 @@
-Metadata-Version: 2.1 Name: mercapy Version: 0.1.0 Summary: A Mercadona SDK for
-Python to track product prices, amounts, and more. Author: Joel Taylor Author-
-email: contact@joeltaylor.business License: MIT Keywords:
+Metadata-Version: 2.1 Name: mercapy Version: 0.2.0 Summary: A Mercadona
+interface for Python to track product prices, amounts, and more. Author: Joel
+Taylor Author-email: contact@joeltaylor.business License: MIT Keywords:
 mercadona,api,sdk,data science,prices,information Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.12 Classifier: Programming Language ::
 Python :: Implementation :: CPython Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: requests
                                     ************
                                    [[mmeerrccaappyy]]
                                 ?ð????ï?¸? mmeerrccaappyy
                                      ************
-****** AA MMeerrccaaddoonnaa SSDDKK ffoorr PPyytthhoonn ttoo ttrraacckk pprroodduucctt pprriicceess,, aammoouunnttss,, aanndd mmoorree.. ******
+  ****** AA MMeerrccaaddoonnaa iinntteerrffaaccee ffoorr PPyytthhoonn ttoo ttrraacckk pprroodduucctt pprriicceess,, aammoouunnttss,, aanndd
+                                   mmoorree.. ******
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_m_e_r_c_a_p_y_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_L_i_c_e_n_s_e_]_[_L_i_c_e_n_s_e_]
                                   _[_L_i_n_k_e_d_I_n_]
                            _H_o_w_ _t_o_ _u_s_e_ _i_t â¢ _R_e_l_a_t_e_d
 ## ð§ How to use it First of all, install the package using: ```bash pip
-install mercapy ``` Now you can start tracking multiple product's prices,
-availability, weight, etc. ```python from mercapy import Product water =
-Product("27335") print(water.ean) print(water.price) print(water.origin) ```
-And you can also get other recommended products: ```python # Get recommended
-product's prices recommeded = water.get_recommended() for product in
-recommeded: print(product.price) ```
+install mercapy ``` By initializing the mercadona class, you can search
+products, recommendations, and new arrivals: ```python from mercapy import
+Mercadona mercadona = Mercadona() mercadona.search("galletas")
+mercadona.get_new_arrivals() mercadona.get_home_recommendations() ``` Each
+product has statistics such as: ```python from mercapy import Product # Find
+product by ID prod = Product("12345") prod.name # Beer prod.unit_price #
+1.25â¬ prod.previos_price # 1.95â¬ prod.is_discounted # True prod.bulk_price
+# 7.5â¬ prod.is_pack # True prod.weight # 0.5kg prod.age_check # True
+prod.alcohol_by_volume # 3.2% prod.iva # 21% ``` You can also interact with
+product photos: ```python from mercapy import Product # Find product by ID prod
+= Product("12345") prod.images[0].save("product.png", width=1920, height=1080)
+``` More docs coming soon...
 ## ðââï¸ You may also like... - [ð·ð± pygramcore](https://
-github.com/jtayped/pygramcore) - A simple-to-use Instagram SDK for Python using
-Selenium. - [ð§âð¼My Portfolio](https://joeltaylor.business) - Check out
-my front-end and SEO skills on my Portfolio!
+github.com/jtayped/pygramcore) - A simple-to-use Instagram interface for Python
+using Selenium. - [ð§âð¼My Portfolio](https://joeltaylor.business) -
+Check out my front-end and SEO skills on my Portfolio!
```

### Comparing `mercapy-0.1.0/setup.py` & `mercapy-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
 # Read version from VERSION file
 here = path.abspath(path.dirname(__file__))
 
-VERSION = "0.1.0"
-DESCRIPTION = "A Mercadona SDK for Python to track product prices, amounts, and more."
+VERSION = "0.2.0"
+DESCRIPTION = "A Mercadona interface for Python to track product prices, amounts, and more."
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="mercapy",
```


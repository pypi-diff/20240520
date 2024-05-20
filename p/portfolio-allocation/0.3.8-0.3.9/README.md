# Comparing `tmp/portfolio_allocation-0.3.8.tar.gz` & `tmp/portfolio_allocation-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portfolio_allocation-0.3.8.tar", max compression
+gzip compressed data, was "portfolio_allocation-0.3.9.tar", max compression
```

## Comparing `portfolio_allocation-0.3.8.tar` & `portfolio_allocation-0.3.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35149 2024-02-27 04:42:56.872238 portfolio_allocation-0.3.8/LICENSE
--rw-r--r--   0        0        0     1197 2024-02-27 04:42:56.872238 portfolio_allocation-0.3.8/README.md
--rw-r--r--   0        0        0       47 2024-02-27 04:42:56.872238 portfolio_allocation-0.3.8/portfolio_allocation/__init__.py
--rw-r--r--   0        0        0      229 2024-02-27 04:42:56.872238 portfolio_allocation-0.3.8/portfolio_allocation/cache.py
--rw-r--r--   0        0        0     2410 2024-02-27 04:42:56.872238 portfolio_allocation-0.3.8/portfolio_allocation/cli.py
--rw-r--r--   0        0        0     2220 2024-02-27 04:42:56.872238 portfolio_allocation-0.3.8/portfolio_allocation/gnucash.py
--rw-r--r--   0        0        0       34 2024-02-27 04:42:56.872238 portfolio_allocation-0.3.8/portfolio_allocation/instruments/__init__.py
--rw-r--r--   0        0        0      737 2024-02-27 04:42:56.872238 portfolio_allocation-0.3.8/portfolio_allocation/instruments/instruments.py
--rw-r--r--   0        0        0      337 2024-02-27 04:42:56.872238 portfolio_allocation-0.3.8/portfolio_allocation/instruments/model.py
--rw-r--r--   0        0        0        0 2024-02-27 04:42:56.872238 portfolio_allocation-0.3.8/portfolio_allocation/instruments/sources/__init__.py
--rw-r--r--   0        0        0     1073 2024-02-27 04:42:56.872238 portfolio_allocation-0.3.8/portfolio_allocation/instruments/sources/currencies.py
--rw-r--r--   0        0        0     1434 2024-02-27 04:42:56.872238 portfolio_allocation-0.3.8/portfolio_allocation/instruments/sources/custom.py
--rw-r--r--   0        0        0     4286 2024-02-27 04:42:56.876238 portfolio_allocation-0.3.8/portfolio_allocation/instruments/sources/funds.py
--rw-r--r--   0        0        0     1898 2024-02-27 04:42:56.876238 portfolio_allocation-0.3.8/portfolio_allocation/instruments/sources/securities.py
--rw-r--r--   0        0        0       29 2024-02-27 04:42:56.876238 portfolio_allocation-0.3.8/portfolio_allocation/report/__init__.py
--rw-r--r--   0        0        0     2207 2024-02-27 04:42:56.876238 portfolio_allocation-0.3.8/portfolio_allocation/report/report.py
--rw-r--r--   0        0        0        0 2024-02-27 04:42:56.876238 portfolio_allocation-0.3.8/portfolio_allocation/report/resources/__init__.py
--rw-r--r--   0        0        0      537 2024-02-27 04:42:56.876238 portfolio_allocation-0.3.8/portfolio_allocation/report/resources/main.css
--rw-r--r--   0        0        0     7189 2024-02-27 04:42:56.876238 portfolio_allocation-0.3.8/portfolio_allocation/report/resources/main.js
--rw-r--r--   0        0        0      509 2024-02-27 04:42:56.876238 portfolio_allocation-0.3.8/portfolio_allocation/report/resources/report_template.html
--rw-r--r--   0        0        0     1240 2024-02-27 04:42:56.876238 portfolio_allocation-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 portfolio_allocation-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-28 04:53:30.396218 portfolio_allocation-0.3.9/LICENSE
+-rw-r--r--   0        0        0     1197 2024-04-28 04:53:30.396218 portfolio_allocation-0.3.9/README.md
+-rw-r--r--   0        0        0       47 2024-04-28 04:53:30.396218 portfolio_allocation-0.3.9/portfolio_allocation/__init__.py
+-rw-r--r--   0        0        0      229 2024-04-28 04:53:30.396218 portfolio_allocation-0.3.9/portfolio_allocation/cache.py
+-rw-r--r--   0        0        0     2410 2024-04-28 04:53:30.396218 portfolio_allocation-0.3.9/portfolio_allocation/cli.py
+-rw-r--r--   0        0        0     2220 2024-04-28 04:53:30.396218 portfolio_allocation-0.3.9/portfolio_allocation/gnucash.py
+-rw-r--r--   0        0        0       34 2024-04-28 04:53:30.396218 portfolio_allocation-0.3.9/portfolio_allocation/instruments/__init__.py
+-rw-r--r--   0        0        0      737 2024-04-28 04:53:30.396218 portfolio_allocation-0.3.9/portfolio_allocation/instruments/instruments.py
+-rw-r--r--   0        0        0      337 2024-04-28 04:53:30.396218 portfolio_allocation-0.3.9/portfolio_allocation/instruments/model.py
+-rw-r--r--   0        0        0        0 2024-04-28 04:53:30.396218 portfolio_allocation-0.3.9/portfolio_allocation/instruments/sources/__init__.py
+-rw-r--r--   0        0        0     1073 2024-04-28 04:53:30.396218 portfolio_allocation-0.3.9/portfolio_allocation/instruments/sources/currencies.py
+-rw-r--r--   0        0        0     1434 2024-04-28 04:53:30.396218 portfolio_allocation-0.3.9/portfolio_allocation/instruments/sources/custom.py
+-rw-r--r--   0        0        0     4286 2024-04-28 04:53:30.396218 portfolio_allocation-0.3.9/portfolio_allocation/instruments/sources/funds.py
+-rw-r--r--   0        0        0     1898 2024-04-28 04:53:30.396218 portfolio_allocation-0.3.9/portfolio_allocation/instruments/sources/securities.py
+-rw-r--r--   0        0        0       29 2024-04-28 04:53:30.396218 portfolio_allocation-0.3.9/portfolio_allocation/report/__init__.py
+-rw-r--r--   0        0        0     2207 2024-04-28 04:53:30.396218 portfolio_allocation-0.3.9/portfolio_allocation/report/report.py
+-rw-r--r--   0        0        0        0 2024-04-28 04:53:30.396218 portfolio_allocation-0.3.9/portfolio_allocation/report/resources/__init__.py
+-rw-r--r--   0        0        0      537 2024-04-28 04:53:30.396218 portfolio_allocation-0.3.9/portfolio_allocation/report/resources/main.css
+-rw-r--r--   0        0        0     7189 2024-04-28 04:53:30.396218 portfolio_allocation-0.3.9/portfolio_allocation/report/resources/main.js
+-rw-r--r--   0        0        0      509 2024-04-28 04:53:30.400218 portfolio_allocation-0.3.9/portfolio_allocation/report/resources/report_template.html
+-rw-r--r--   0        0        0     1240 2024-04-28 04:53:30.400218 portfolio_allocation-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 portfolio_allocation-0.3.9/PKG-INFO
```

### Comparing `portfolio_allocation-0.3.8/LICENSE` & `portfolio_allocation-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.3.8/README.md` & `portfolio_allocation-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.3.8/portfolio_allocation/cli.py` & `portfolio_allocation-0.3.9/portfolio_allocation/cli.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.3.8/portfolio_allocation/gnucash.py` & `portfolio_allocation-0.3.9/portfolio_allocation/gnucash.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.3.8/portfolio_allocation/instruments/instruments.py` & `portfolio_allocation-0.3.9/portfolio_allocation/instruments/instruments.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.3.8/portfolio_allocation/instruments/sources/currencies.py` & `portfolio_allocation-0.3.9/portfolio_allocation/instruments/sources/currencies.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.3.8/portfolio_allocation/instruments/sources/custom.py` & `portfolio_allocation-0.3.9/portfolio_allocation/instruments/sources/custom.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.3.8/portfolio_allocation/instruments/sources/funds.py` & `portfolio_allocation-0.3.9/portfolio_allocation/instruments/sources/funds.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.3.8/portfolio_allocation/instruments/sources/securities.py` & `portfolio_allocation-0.3.9/portfolio_allocation/instruments/sources/securities.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.3.8/portfolio_allocation/report/report.py` & `portfolio_allocation-0.3.9/portfolio_allocation/report/report.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.3.8/portfolio_allocation/report/resources/main.css` & `portfolio_allocation-0.3.9/portfolio_allocation/report/resources/main.css`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.3.8/portfolio_allocation/report/resources/main.js` & `portfolio_allocation-0.3.9/portfolio_allocation/report/resources/main.js`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.3.8/pyproject.toml` & `portfolio_allocation-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "portfolio-allocation"
-version = "0.3.8"
+version = "0.3.9"
 description = "Calculates currency, country and industry allocations for portfolio of ETFs and mutual funds"
 authors = ["Kirill Fertikov <kirill.fertikov@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 homepage = "https://pypi.org/project/portfolio-allocation/"
 repository = "https://github.com/fertkir/portfolio-allocation"
 keywords = ["etf", "allocation", "moex", "tinkoff", "finex", "gnucash"]
```

### Comparing `portfolio_allocation-0.3.8/PKG-INFO` & `portfolio_allocation-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolio-allocation
-Version: 0.3.8
+Version: 0.3.9
 Summary: Calculates currency, country and industry allocations for portfolio of ETFs and mutual funds
 Home-page: https://pypi.org/project/portfolio-allocation/
 License: GPL-3.0-or-later
 Keywords: etf,allocation,moex,tinkoff,finex,gnucash
 Author: Kirill Fertikov
 Author-email: kirill.fertikov@gmail.com
 Requires-Python: >=3.12,<4.0
```


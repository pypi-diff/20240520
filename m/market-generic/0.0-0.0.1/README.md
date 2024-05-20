# Comparing `tmp/market_generic-0.0.tar.gz` & `tmp/market_generic-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market_generic-0.0.tar", last modified: Mon May 13 14:30:00 2024, max compression
+gzip compressed data, was "market_generic-0.0.1.tar", last modified: Mon May 20 18:36:00 2024, max compression
```

## Comparing `market_generic-0.0.tar` & `market_generic-0.0.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:30:00.044591 market_generic-0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-13 14:30:00.044591 market_generic-0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-13 14:29:50.000000 market_generic-0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:30:00.044591 market_generic-0.0/market_generic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-13 14:29:59.000000 market_generic-0.0/market_generic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-13 14:30:00.000000 market_generic-0.0/market_generic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:29:59.000000 market_generic-0.0/market_generic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-13 14:29:59.000000 market_generic-0.0/market_generic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 14:29:59.000000 market_generic-0.0/market_generic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-13 14:29:50.000000 market_generic-0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:30:00.044591 market_generic-0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-13 14:29:50.000000 market_generic-0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:30:00.040591 market_generic-0.0/trade/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:29:50.000000 market_generic-0.0/trade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:30:00.040591 market_generic-0.0/trade/calendar/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-13 14:29:50.000000 market_generic-0.0/trade/calendar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10783 2024-05-13 14:29:50.000000 market_generic-0.0/trade/calendar/calendar_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-13 14:29:50.000000 market_generic-0.0/trade/calendar/calendar_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:30:00.044591 market_generic-0.0/trade/ticker/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-13 14:29:50.000000 market_generic-0.0/trade/ticker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-13 14:29:50.000000 market_generic-0.0/trade/ticker/api_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-13 14:29:50.000000 market_generic-0.0/trade/ticker/market.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-13 14:29:50.000000 market_generic-0.0/trade/ticker/yf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:30:00.044591 market_generic-0.0/trade/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-13 14:29:50.000000 market_generic-0.0/trade/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-13 14:29:50.000000 market_generic-0.0/trade/utils/df_market_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-13 14:29:50.000000 market_generic-0.0/trade/utils/gsheet_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-13 14:29:50.000000 market_generic-0.0/trade/utils/log_configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:30:00.044591 market_generic-0.0/trade/utils/meta_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-13 14:29:50.000000 market_generic-0.0/trade/utils/meta_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-13 14:29:50.000000 market_generic-0.0/trade/utils/meta_utils/master_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-13 14:29:50.000000 market_generic-0.0/trade/utils/meta_utils/singleton_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-13 14:29:50.000000 market_generic-0.0/trade/utils/network_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-13 14:29:50.000000 market_generic-0.0/trade/utils/op_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-13 14:29:50.000000 market_generic-0.0/trade/utils/telegram_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:36:00.751809 market_generic-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-20 18:36:00.751809 market_generic-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-20 18:35:46.000000 market_generic-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:36:00.751809 market_generic-0.0.1/market_generic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-20 18:36:00.000000 market_generic-0.0.1/market_generic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-20 18:36:00.000000 market_generic-0.0.1/market_generic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:36:00.000000 market_generic-0.0.1/market_generic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 18:36:00.000000 market_generic-0.0.1/market_generic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 18:36:00.000000 market_generic-0.0.1/market_generic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-20 18:35:46.000000 market_generic-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 18:36:00.751809 market_generic-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-20 18:35:46.000000 market_generic-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:36:00.747809 market_generic-0.0.1/trade/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:36:00.747809 market_generic-0.0.1/trade/calendar/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/calendar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/calendar/calendar_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/calendar/calendar_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:36:00.751809 market_generic-0.0.1/trade/nse/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/nse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/nse/nse_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/nse/nse_stock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:36:00.751809 market_generic-0.0.1/trade/ticker/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/ticker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/ticker/api_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/ticker/market.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/ticker/stock_generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/ticker/yf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:36:00.751809 market_generic-0.0.1/trade/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/utils/df_market_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/utils/gsheet_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/utils/log_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/utils/network_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/utils/op_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/utils/telegram_api.py
```

### Comparing `market_generic-0.0/README.md` & `market_generic-0.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,70 @@
-# Trade - A Generic Python Package for Stock Market Analysis and Trading
+# market-generic - A Generic Python Package for Stock Market Analysis and Trading
 
 ### Overview
 
-Trade is a powerful and flexible Python library designed to simplify the process of working with stock market data. It provides a comprehensive set of tools and utilities to handle, analyze, and visualize stock data, enabling developers and analysts to build dynamic stock scanners, trading strategies, and other financial applications with ease.
+`market-generic` is a powerful and flexible Python library designed to simplify the process of working with stock market data. It provides a comprehensive set of tools and utilities to handle, analyze, and visualize stock data, enabling developers and analysts to build dynamic stock scanners, trading strategies, and other financial applications with ease.
 
 
 ### Key Features
 - <b>Data Handling</b>: Seamless integration with popular data sources (e.g., Yahoo Finance, NSE APIs) to fetch and manage stock data.
 - <b>Technical Indicators</b>: A wide range of technical indicators (e.g., Moving Averages, Pivot Points, RSI, MACD) for in-depth market analysis.
 - <b>Generic Strategy Abstractions</b>: Tools to dynamically create trading strategies on the fly based on user-defined parameters.
 - <b>Extensibility</b>: Modular design allows for easy integration with other Python libraries and frameworks.
 
 
 ### Installation
 To install the AlgoTrade package, use pip:
 
-```
-pip install trade
+```commandline
+pip install market-generic
 ```
 
 ### Usage
 
 Here's a simple example of how to use the Trade package to fetch and analyze stock data:
 python
 
+```python 
+>>from trade.nse import NSEStock
+>>stock = NSEStock("RELIANCE", "17-May-2024")
+>>stock.symbol == "RELIANCE"
+True 
+>>stock.curr_ohlc 
+# Will Display Reliance's latest Bhav 
+{
+"open": 2860.7,
+"low": ...,
+"high":...,
+ "close": ...,
+ "volume": ...
+ "pct_change": ...
+}
 ```
-from trade.data import StockDataFetcher
-from trade.indicators import MovingAverage
 
-# Fetch stock data for Apple (AAPL)
-fetcher = StockDataFetcher()
-data = fetcher.get_stock_data('AAPL')
-
-# Calculate the 20-day simple moving average
-sma_20 = MovingAverage(data, window=20, type='simple')
-
-# Plot the stock price and the moving average
-data.plot(y='Close', label='Price')
-sma_20.plot(label='SMA-20')
+`AllNSEStocks` uses `NSEStock` module underneath to utilize stock functions.
+
+```python
+>>from trade.nse import AllNSEStocks
+>>all_stocks = AllNSEStocks("17-May-2024", ["RELIANCE", "SBIN"])
+>>all_stocks.symbols[0] == "RELIANCE"
+True
+>>all_stocks.symbols[1] == "SBIN"
+True 
+>>all_stocks.symbols[0].curr_ohlc
+# Will Display Reliance's latest Bhav 
+{
+"open": 2860.7,
+"low": ...,
+"high":...,
+ "close": ...,
+ "volume": ...
+ "pct_change": ...
+}
 ```
 
+
 ### Documentation
 
-For detailed documentation, examples, and API reference, please visit the [Trade GitHub repository](https://github.com/sharmasourab93/Trade).
+For detailed documentation, examples, and API reference, please visit the 
+[market-generic 
+GitHub repository](https://github.com/sharmasourab93/market-generic).
```

### Comparing `market_generic-0.0/market_generic.egg-info/SOURCES.txt` & `market_generic-0.0.1/market_generic.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 market_generic.egg-info/dependency_links.txt
 market_generic.egg-info/requires.txt
 market_generic.egg-info/top_level.txt
 trade/__init__.py
 trade/calendar/__init__.py
 trade/calendar/calendar_data.py
 trade/calendar/calendar_tool.py
+trade/nse/__init__.py
+trade/nse/nse_config.py
+trade/nse/nse_stock.py
 trade/ticker/__init__.py
 trade/ticker/api_config.py
 trade/ticker/market.py
+trade/ticker/stock_generics.py
 trade/ticker/yf.py
 trade/utils/__init__.py
 trade/utils/df_market_utils.py
 trade/utils/gsheet_util.py
 trade/utils/log_configurator.py
 trade/utils/network_tools.py
 trade/utils/op_utils.py
-trade/utils/telegram_api.py
-trade/utils/meta_utils/__init__.py
-trade/utils/meta_utils/master_meta.py
-trade/utils/meta_utils/singleton_meta.py
+trade/utils/telegram_api.py
```

### Comparing `market_generic-0.0/setup.py` & `market_generic-0.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import find_packages, setup
 
 NAME = "market-generic"
-VERSION = "0.0"
+__version__ = "0.0.1"
 DESCRITPION = "A Generic Python Package for Stock Market Analysis and Trading"
-URL = "https://github.com/sharmasourab93/market-gen"
+URL = "https://github.com/sharmasourab93/market-generic"
 AUTHOR = "Sourab S Sharma"
 EMAIL = "sharmasourab93@gmail.com"
 
 with open("README.md", "r") as f:
     LONG_DESCRIPTION = f.read()
 
 with open("requirements.txt", "r") as file:
     INSTALL_REQUIRES = [line.strip() for line in file.readlines()]
 
 KEYWORDS = ["Market", "Trade", "Analysis"]
 
 setup(
     name=NAME,
-    version=VERSION,
+    version=__version__,
     author=AUTHOR,
     author_email=EMAIL,
     description=DESCRITPION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url=URL,
     packages=find_packages(exclude=["tests", ".github"]),
```

### Comparing `market_generic-0.0/trade/calendar/calendar_data.py` & `market_generic-0.0.1/trade/calendar/calendar_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,33 +52,51 @@
         self._formatted_date = datetime.strptime(self.raw_date, self.date_fmt).date()
 
     @property
     def as_date(self) -> datetime:
         return self._formatted_date
 
     @property
+    def day(self) -> int:
+        return self._formatted_date.day
+
+    @property
+    def month(self) -> str:
+        return self._formatted_date.strftime("%b")
+
+    @property
+    def year(self) -> str:
+        return self._formatted_date.year
+
+    @property
     def as_str(self) -> str:
         return self.as_date.strftime(self.date_fmt)
 
     @property
     def as_weekday(self):
         return self.as_date.strftime("%A")
 
     @property
     def as_weekday_iso(self) -> int:
         return WEEKDAY_TO_ISO[self.as_weekday]
 
     def __str__(self):
         return self.as_str
 
-    def __add__(self, date_diff: Union[timedelta, BDay]) -> "DateObj":
+    def __add__(self, date_diff: Union[timedelta, BDay, int]) -> "DateObj":
+        if isinstance(date_diff, int):
+            date_diff = timedelta(date_diff)
+
         new_date = self.as_date + date_diff
         return DateObj(new_date.strftime(self.date_fmt), date_fmt=self.date_fmt)
 
-    def __sub__(self, date_diff: Union[timedelta, BDay]) -> "DateObj":
+    def __sub__(self, date_diff: Union[timedelta, BDay, int]) -> "DateObj":
+        if isinstance(date_diff, int):
+            date_diff = timedelta(date_diff)
+
         new_date = self.as_date - date_diff
         return DateObj(new_date.strftime(self.date_fmt), date_fmt=self.date_fmt)
 
     def __eq__(self, another_date: Union["DateObj", date, datetime]):
 
         if isinstance(another_date, date) or isinstance(another_date, datetime):
             another_date = DateObj(
@@ -272,15 +290,16 @@
 
             if tomorrow < date_ and date_ > yesterday:
                 return date_ - BDay()
 
         return date_
 
     def __post_init__(self):
-        self.market_timings = MarketTimings(**self.market_timings)
+        if not isinstance(self.market_timings, MarketTimings):
+            self.market_timings = MarketTimings(**self.market_timings)
 
         if self.today is None:
             self.today = datetime.now(tz=self.market_timings.tz).today().date()
 
         now = datetime.now(tz=self.market_timings.tz).time()
 
         if (
```

### Comparing `market_generic-0.0/trade/calendar/calendar_tool.py` & `market_generic-0.0.1/trade/calendar/calendar_tool.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.0/trade/ticker/api_config.py` & `market_generic-0.0.1/trade/ticker/api_config.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.0/trade/ticker/market.py` & `market_generic-0.0.1/trade/ticker/market.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,60 +1,52 @@
+from dataclasses import dataclass, field
 from pathlib import Path
-from typing import Dict, Optional, Union
+from typing import Callable, Dict, List, Optional, Union
 
 from trade.calendar import MarketCalendar, MarketHolidayType, MarketTimingType
 from trade.ticker.api_config import APIConfig
 from trade.ticker.yf import YFinance
-from trade.utils import DownloadTools, Logger, LoggingType, Utilities
+from trade.utils import DownloadTools, Logger, LoggingType
 
 
-class Exchange(APIConfig, YFinance, MarketCalendar, DownloadTools):
-
-    def __init__(
-        self,
-        today,
-        date_fmt,
-        config,
-        market,
-        country,
-        market_holidays,
-        market_timings,
-        ticker_mod,
-    ):
-        super().__init__(config)
-        YFinance.__init__(
-            self, market, country, date_fmt, ticker_modifications=ticker_mod
-        )
-        MarketCalendar.__init__(self, today, date_fmt, market_holidays, market_timings)
+@dataclass
+class ExchangeArgs:
+    today: str
+    date_fmt: str
+    config: str
+    market: str
+    country: str
+    market_holidays: List[MarketHolidayType]
+    market_timings: List[MarketTimingType]
+    ticker_mod: Optional[Dict[str, str]] = None
+    log_config: Optional[LoggingType] = None
 
 
-class CombinedMeta(type(Exchange), type(Utilities)):
-    pass
-
-
-class Market(Exchange):
+class Exchange(APIConfig, YFinance, MarketCalendar, DownloadTools):
 
     def __init__(
         self,
         today: str,
         date_fmt: str,
-        market_config: Union[Path, str],
+        config: str,
         market: str,
         country: str,
-        market_holiday: MarketHolidayType,
-        market_timing: MarketTimingType,
+        market_holidays: Union[List[MarketHolidayType], Callable],
+        market_timings: List[MarketTimingType],
         ticker_mod: Optional[Dict[str, str]] = None,
         logging_config: Optional[LoggingType] = None,
-        **kwargs,
     ):
-
-        super().__init__(
-            today=today,
-            date_fmt=date_fmt,
-            market=market,
-            country=country,
-            config=market_config,
-            market_holidays=market_holiday,
-            market_timings=market_timing,
-            ticker_mod=ticker_mod,
-            **kwargs,
+        super().__init__(config)
+        YFinance.__init__(
+            self, market, country, date_fmt, ticker_modifications=ticker_mod
+        )
+        market_holidays = (
+            market_holidays if isinstance(market_holidays, list) else market_holidays()
         )
+        MarketCalendar.__init__(self, today, date_fmt, market_holidays, market_timings)
+
+        # TODO: Identify a way to make use of metaclasses to enable, logging,
+        #  telegram & compute execution time methods.
+        # This is just for the time being.
+        if logging_config is not None:
+            Logger.setup_logging(**logging_config)
+            self.logger = Logger.get_logger(__name__)
```

### Comparing `market_generic-0.0/trade/ticker/yf.py` & `market_generic-0.0.1/trade/ticker/yf.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from calendar import monthrange
 from datetime import date, datetime
 from typing import Dict, List, Optional, Tuple
 
 import numpy as np
 import pandas as pd
 import yfinance as yf
+
 from trade.utils import Logger, MarketDFUtils
 
 SYMBOL_ERROR = "Error Incurred for symbol: {0}"
 YFIN_TICKER_BY_COUNTRY = {
     "INDIA": {"BSE": ".BO", "NSE": ".NS"},
     # TODO: Populate this country to extend to all the countries.
 }
@@ -26,15 +27,15 @@
     ):
         self.market = market
         self.country = country
         self.date_fmt = date_fmt
         self.ticker_modifications = ticker_modifications
         self.yf = yf
 
-    def adjust_yfin_ticker_by_market(self, symbol: str, index: bool) -> str:
+    def adjust_yfin_ticker_by_market(self, symbol: str, index: bool = False) -> str:
 
         if not index:
             if self.country in YFIN_TICKER_BY_COUNTRY.keys():
                 suffix = YFIN_TICKER_BY_COUNTRY[self.country].get(self.market, "")
 
             if suffix != str():
                 return symbol.upper() + suffix
@@ -46,31 +47,40 @@
             self.logger.error(message)
 
     def get_period_data(
         self,
         symbol: str,
         period: str = "1mo",
         interval: str = "1d",
+        start: date = None,
+        end: date = None,
         rounding: bool = True,
         index: bool = False,
         ascending: bool = False,
         auto_adjust: bool = True,
         progress: bool = False,
         **kwargs,
     ) -> pd.DataFrame:
 
-        symbol = self.adjust_yfin_ticker_by_market(symbol, index)
-
-        data = self.yf.download(
-            symbol,
-            period=period,
+        download_params = dict(
             interval=interval,
             rounding=rounding,
             auto_adjust=auto_adjust,
             progress=progress,
+        )
+        symbol = self.adjust_yfin_ticker_by_market(symbol, index)
+
+        if start is None and end is None:
+            download_params.update({"period": period})
+        else:
+            download_params.update({"start": start, "end": end})
+
+        data = self.yf.download(
+            symbol,
+            **download_params,
             **kwargs,
         )
 
         if 0 in data.shape:
             message = SYMBOL_ERROR.format(symbol)
             self.log_method(message)
```

### Comparing `market_generic-0.0/trade/utils/gsheet_util.py` & `market_generic-0.0.1/trade/utils/gsheet_util.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.0/trade/utils/log_configurator.py` & `market_generic-0.0.1/trade/utils/log_configurator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
+from dataclasses import dataclass
 from datetime import datetime
 from logging import config as log_conf
 from os import mkdir, path
 from pathlib import Path
-from typing import Any, TypedDict
+from typing import Any, Literal
 
 LOG_MAP = {
     "version": 1,
     "disable_existing_loggers": True,
     "formatters": {
         "simple": {
             "format": "%(asctime)s:[%(levelname)s]: %(name)s: %(message)s",
@@ -28,19 +29,20 @@
             "encoding": "utf8",
         },
     },
     "root": {"level": "INFO", "handlers": ["console", "file_handler"]},
 }
 
 
-class LoggingType(TypedDict):
+@dataclass
+class LoggingType:
     date_fmt: str
     log_path: str
     config_path: str
-    level: Any
+    level: Literal[0, 10, 20, 30, 40, 50]
     to_log: bool = True
     to_console: bool = True
 
 
 class LogConfig:
     """
     LogConfig Module to Configure logger.
```

### Comparing `market_generic-0.0/trade/utils/network_tools.py` & `market_generic-0.0.1/trade/utils/network_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,44 @@
 import csv
 import os
 from abc import ABC
 from io import BytesIO
 from typing import Optional
+from urllib.error import HTTPError
 from urllib.parse import urlparse
 from zipfile import ZipFile
 
 import requests
 from pandas import DataFrame, read_csv, read_excel
 from requests import Session
 from requests.exceptions import ConnectionError, InvalidURL, ReadTimeout
 
 CHUNK_SIZE = 1024
 INVALID_URL = "URL: {0}, Status Code:{1}"
+RECEIVED_STATUS = "Status Code Received: {0}"
+
+
+def match_http(result, status_code: int, url: Optional[str] = None):
+    msg = ""
+    match status_code:
+        case 200:
+            return result
+
+        case 404:
+            raise InvalidURL(INVALID_URL.format(url, result.status_code))
+
+        case 403:
+            msg = RECEIVED_STATUS.format(status_code)
+            if url is not None:
+                msg += ". For url: {0}".format(url)
+
+            raise Exception(msg)
+
+        case _:
+            raise Exception(RECEIVED_STATUS.format(status_code))
 
 
 class DownloadTools(ABC):
     def get_cookies(self, base_url: str, headers: dict, timeout: int = 5) -> dict:
 
         url = self.extract_domain(base_url)
 
@@ -32,42 +54,37 @@
 
     def get_request_api(
         self, url: str, headers: dict, cookies: Optional[dict] = None, **kwargs
     ):
 
         cookies = self.get_cookies(url, headers)
         result = requests.get(url, headers=headers, cookies=cookies, **kwargs)
-
-        if result.status_code == 200:
-            return result
-
-        elif result.status_code == 404:
-            raise InvalidURL(INVALID_URL.format(url, result.status_code))
-
-        return self.get_request_api(url, headers, cookies)
+        return match_http(result, result.status_code, url)
 
     def extract_domain(self, url: str) -> str:
         parsed_url = urlparse(url)
         domain = parsed_url.netloc
 
         return "https://" + domain
 
-    def download_data(self, url: str, headers: str) -> BytesIO:
+    def get_headers(self, url):
+
+        return requests.head(url)
+
+    def download_data(self, url: str, headers: Optional[str] = None) -> DataFrame:
         """
         For a given url and file name
         download data to the provided filename/path.
         """
         domain = self.extract_domain(url)
         cookies = self.get_cookies(domain, headers)
         response = self.get_request_api(url, headers, cookies)
 
         bytes_obj = BytesIO(response.content)
 
-        self.logger.debug("Response received.")
-
         if self.is_zip(bytes_obj):
             bytes_obj = self.unzip(bytes_obj)
 
         result = self.read_from_buffer(bytes_obj)
 
         return result
```

### Comparing `market_generic-0.0/trade/utils/telegram_api.py` & `market_generic-0.0.1/trade/utils/telegram_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 import asyncio
 from datetime import datetime
 from functools import cache
 from os import getenv
 
 import telegram
-from trade.utils.meta_utils.singleton_meta import SingletonMeta
 
 TELEGRAM_SIGNATURE = "\n Generated on {0}."
 
 
+class SingletonMeta(type):
+    _instances = {}
+
+    def __call__(cls, *args, **kwargs):
+        if cls not in cls._instances:
+            cls._instances[cls] = super().__call__(*args, **kwargs)
+
+        return cls._instances[cls]
+
+
 class TelegramBot(metaclass=SingletonMeta):
     """
     TelegramBot method is built on the Singleton Pattern
     wherein at any given point we do not replicate creation of
     TelegramBot objects. This helps in using the same object
     over and over again in an optimized manner.
     """
```


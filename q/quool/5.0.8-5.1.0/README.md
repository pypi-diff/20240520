# Comparing `tmp/quool-5.0.8.tar.gz` & `tmp/quool-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quool-5.0.8.tar", last modified: Tue Apr  9 05:38:09 2024, max compression
+gzip compressed data, was "quool-5.1.0.tar", last modified: Mon May 20 03:34:13 2024, max compression
```

## Comparing `quool-5.0.8.tar` & `quool-5.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:38:09.513256 quool-5.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-09 05:37:43.000000 quool-5.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-04-09 05:38:09.513256 quool-5.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-09 05:37:43.000000 quool-5.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:38:09.513256 quool-5.0.8/quool/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-09 05:37:43.000000 quool-5.0.8/quool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-09 05:37:43.000000 quool-5.0.8/quool/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-04-09 05:37:43.000000 quool-5.0.8/quool/factor.py
--rw-r--r--   0 runner    (1001) docker     (127)    19383 2024-04-09 05:37:43.000000 quool-5.0.8/quool/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-09 05:37:43.000000 quool-5.0.8/quool/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-09 05:37:43.000000 quool-5.0.8/quool/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:38:09.513256 quool-5.0.8/quool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-04-09 05:38:09.000000 quool-5.0.8/quool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 05:38:09.000000 quool-5.0.8/quool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 05:38:09.000000 quool-5.0.8/quool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 05:38:09.000000 quool-5.0.8/quool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 05:38:09.000000 quool-5.0.8/quool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 05:38:09.513256 quool-5.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-09 05:37:43.000000 quool-5.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:34:13.413856 quool-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-20 03:33:40.000000 quool-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-20 03:34:13.413856 quool-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-20 03:33:40.000000 quool-5.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:34:13.413856 quool-5.1.0/quool/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-20 03:33:40.000000 quool-5.1.0/quool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-05-20 03:33:40.000000 quool-5.1.0/quool/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-05-20 03:33:40.000000 quool-5.1.0/quool/factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20456 2024-05-20 03:33:40.000000 quool-5.1.0/quool/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-20 03:33:40.000000 quool-5.1.0/quool/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-20 03:33:40.000000 quool-5.1.0/quool/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:34:13.413856 quool-5.1.0/quool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-20 03:34:13.000000 quool-5.1.0/quool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-20 03:34:13.000000 quool-5.1.0/quool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 03:34:13.000000 quool-5.1.0/quool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-20 03:34:13.000000 quool-5.1.0/quool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 03:34:13.000000 quool-5.1.0/quool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 03:34:13.413856 quool-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-20 03:33:40.000000 quool-5.1.0/setup.py
```

### Comparing `quool-5.0.8/LICENSE` & `quool-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quool-5.0.8/quool/core.py` & `quool-5.1.0/quool/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -93,30 +93,14 @@
                     new_dat.reindex(columns=frag_dat.columns).astype(self.dtypes)
                 ], axis=0)
             frag_dat.to_parquet(self._fragment_path(name))
         else:
             frag.reindex(columns=self.columns).astype(
                 self.dtypes).to_parquet(self._fragment_path(name))
     
-    def _add_frag(self, frag: pd.DataFrame):
-        # in case of empty dataframe
-        if frag.empty:
-            return
-        
-        name = self.namer(frag)
-        if name in self.fragments:
-            frag_dat = self._read_fragment(name)
-            # here we need to use outer join for inner join may delete data
-            frag_dat = pd.concat([frag_dat, frag], axis=1, join='outer')
-            frag_dat = frag_dat.astype(frag.dtypes)
-            frag_dat.to_parquet(self._fragment_path(name))
-        else:
-            frag.reindex(columns=self.columns.union(frag.columns)
-                ).to_parquet(self._fragment_path(name))
-    
     def _read_fragment(
         self,
         fragment: list | str = None,
     ):
         fragment = fragment or self.fragments
         fragment = [fragment] if not isinstance(fragment, list) else fragment
         fragment = [self._fragment_path(frag) for frag in fragment]
@@ -143,32 +127,22 @@
             df = df.to_frame()
         
         if not df.columns.difference(self.columns).empty:
             raise ValueError("new field found, please add first")
 
         df.groupby(self.spliter).apply(self._update_frag)
 
-    def add(self, df: pd.Series | pd.DataFrame):
-        if isinstance(df, pd.Series):
-            df = df.to_frame()
-        
-        if not (df.columns == df.columns.astype('str')).all():
-            raise TypeError("all columns or name should be string type")
-        
-        if not df.columns.intersection(self.columns).empty:
+    def add(self, column: dict):
+        if not self.columns.intersection(column.keys()).empty:
             raise ValueError("existing field found, please update it")
         
-        df.groupby(self.spliter).apply(self._add_frag)
-        related_fragment = self._related_frag(df)
-        dtypes = self._read_fragment(related_fragment[0]).dtypes
-        columns = df.columns if isinstance(df, pd.DataFrame) else [df.name]
-        for frag in set(self.fragments) - set(related_fragment):
+        for frag in self.fragments:
             d = self._read_fragment(frag)
-            d[columns] = np.nan
-            d = d.astype(dtypes)
+            d[list(column.keys())] = np.nan
+            d = d.astype(column)
             d.to_parquet(self._fragment_path(frag))
     
     def delete(self, index: pd.Index):
         related_fragment = self._related_frag(pd.DataFrame(index=index))
         for frag in related_fragment:
             df = self._read_fragment(frag)
             df = df.drop(index=index.intersection(df.index))
```

### Comparing `quool-5.0.8/quool/factor.py` & `quool-5.1.0/quool/factor.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         name: str = None, 
     ):
         code_level = self.get_levelname(self._code_level)
         date_level = self.get_levelname(self._date_level)
         code_level = 'order_book_id' if isinstance(code_level, int) else code_level
         date_level = 'date' if isinstance(date_level, int) else date_level
         if isinstance(df, pd.DataFrame) and df.index.nlevels == 1:
-            df = df.stack(dropna=True).swaplevel()
+            df = df.stack(future_stack=True).swaplevel()
             df.index.names = [code_level, date_level]
         
         if isinstance(df, pd.Series):
             if name is None:
                 raise ValueError('name cannot be None')
             df.index.names = [code_level, date_level]
             df = df.to_frame(name)
```

### Comparing `quool-5.0.8/quool/record.py` & `quool-5.1.0/quool/record.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import requests
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from lxml import etree
 from pathlib import Path
 from .table import ItemTable
+from .util import parse_commastr
 
 
 class RunRecorder(ItemTable):
 
     def __init__(
         self, 
         uri: str | Path, 
@@ -36,14 +37,16 @@
             self.update(rec)
         if not nonexisted.empty:
             self.add(rec)
 
 
 class TradeRecorder(ItemTable):
 
+    standard_columns = ["datetime", "code", "size", "price", "amount", "commission"]
+
     def __init__(
         self, 
         uri: str | Path, 
         principle: float = None, 
         start: str | pd.Timestamp = None,
     ):
         super().__init__(uri, True)
@@ -52,29 +55,56 @@
                 raise ValueError("principle and start_date must be specified when initiating")
             self.add(pd.DataFrame([{
                 "datetime": pd.to_datetime(start), 
                 "code": "cash", "size": float(principle), 
                 "price": 1.0, "amount": float(principle), "commission": 0.0
             }], index=[pd.to_datetime('now')]))
         
-        if not self.columns.isin(["datetime", "code", "size", "price", "amount", "commission"]).all():
-            raise ValueError("The table must have columns datetime, code, size, price, amount, commission")
+        if not self.columns.isin(self.standard_columns).all():
+            raise ValueError("The table must have standard columns")
     
     @property
     def spliter(self):
-        return pd.Grouper(key='datetime', freq='M')
+        return pd.Grouper(key='datetime', freq='ME')
 
     @property
     def namer(self):
         return lambda x: x['datetime'].iloc[0].strftime('%Y%m')
     
     def prune(self):
         for frag in self.fragments:
             self._fragment_path(frag).unlink()
 
+    def read(
+        self, 
+        field: str | list = None,
+        start: str | list = None, 
+        stop: str = None,
+        code: str | list = None,
+        filters: list = None,
+    ) -> pd.Series | pd.DataFrame:
+        field = parse_commastr(field)
+        code = parse_commastr(code)
+        start = pd.to_datetime(start if start is not None else 0)
+        stop = pd.to_datetime(stop if stop is not None else 'now')
+        filters = filters or []
+        if not isinstance(start, pd.DatetimeIndex):
+            filters += [
+                ("datetime", ">=", start),
+                ("datetime", "<=", stop)
+            ]
+            if code is not None:
+                filters.append(["code", "in", code])
+        else:
+            filters += [("datetime", "in", start)]
+            if code is not None:
+                filters.append(("code", "in", code))
+        
+        return pd.read_parquet(self.path, columns=field, filters=filters)
+
     def trade(
         self, 
         date: str | pd.Timestamp,
         code: str,
         size: float = None,
         price: float = None,
         amount: float = None,
@@ -94,32 +124,34 @@
             "commission": commission, **kwargs
         }], index=[pd.to_datetime('now')])
         if code != "cash":
             cash = pd.DataFrame([{
                 "datetime": pd.to_datetime(date),
                 "code": "cash", "size": -size * price - commission,
                 "price": 1, "commission": 0,
-                "amount": -size * price - commission, **kwargs
+                "amount": -size * price - commission
             }], index=[pd.to_datetime('now')])
             trade = pd.concat([trade, cash], axis=0)
         
+        if kwargs:
+            self.add(dict((k, type(v)) for k, v in kwargs.items()))
         self.update(trade)
 
     def peek(self, date: str | pd.Timestamp = None, price: pd.Series = None) -> pd.Series:
         df = self.read(filters=[("datetime", "<=", pd.to_datetime(date or 'now'))])
         df = df.groupby("code")[["size", "amount", "commission"]].sum()
         df["cost"] = (df["amount"] / df["size"]).replace([-np.inf, np.inf], 0)
         if price is None:
             return df
         price = price.copy()
         price.loc["cash"] = 1
         indexer = price.index.get_indexer_for(df.index)
         df["price"] = price.iloc[indexer[indexer != -1]]
         df["value"] = df["price"] * df["size"]
-        df["pnl"] = df["price"] / df["cost"] - 1
+        df['pnl'] = ((df['price'] - df['cost']) * df['size']).where(df['size'] != 0, -df['amount'])
         return df
         
     def report(
         self, 
         price: pd.Series, 
         code_level: int | str = 0,
         date_level: int | str = 1,
@@ -131,25 +163,24 @@
             price = price.stack().sort_index().to_frame("price")
             price.index.names = [date_level, code_level]
         price = price.squeeze().sort_index()
         dates = price.index.get_level_values(date_level).unique()
         dates = dates[dates >= data["datetime"].min()]
 
         data = data.groupby(["code", "datetime"]).sum()
-        data = data.groupby("code").apply(lambda x: x.droplevel('code').reindex(
-            dates.union(x.index.get_level_values('datetime').unique().sort_values())
-        ))
+        data = data.reindex(pd.MultiIndex.from_product(
+            [data.index.levels[0], dates], names=["code", "datetime"]))
         cash = data.loc["cash", "amount"]
         cash = cash.fillna(0).cumsum()
 
         noncash = data.drop(labels="cash", axis=0)
         noncash.index.names = price.index.names
         price = price.loc[noncash.index.intersection(price.index)]
         delta = (price * noncash["size"]).groupby(level=date_level).sum()
-        noncash = noncash.groupby(level=code_level, group_keys=False).apply(lambda x: x.fillna(0).cumsum())
+        noncash = noncash.fillna(0).groupby(level=code_level, group_keys=False).cumsum()
         market = (price * noncash["size"]).groupby(level=date_level).sum()
         market = market.reindex(cash.index).fillna(0)
         value = market + cash
         turnover = (delta / value.shift(1)).fillna(0)
 
         data = pd.concat([value, cash, turnover], axis=1, keys=["value", "cash", "turnover"])
         return data
@@ -164,25 +195,25 @@
         result: str = None,
     ):
         
         cash = cash.squeeze() if isinstance(cash, (pd.Series, pd.DataFrame)) else \
             pd.Series(np.zeros(value.shape[0]), index=value.index)
         turnover = turnover.squeeze() if isinstance(turnover, (pd.Series, pd.DataFrame)) else \
             pd.Series(np.zeros(value.shape[0]), index=value.index)
-        benchmark = benchmark.droplevel(0) if isinstance(benchmark, (pd.Series, pd.DataFrame)) else \
+        benchmark = benchmark if isinstance(benchmark, (pd.Series, pd.DataFrame)) else \
             pd.Series(np.zeros(value.shape[0]), index=value.index)
         benchmark = benchmark.loc[value.index]
         net_value = value / value.iloc[0]
         net_cash = cash / cash.iloc[0]
         returns = value.pct_change(fill_method=None).fillna(0)
         benchmark_returns = benchmark.pct_change(fill_method=None).fillna(0)
         benchmark_returns = benchmark_returns if not benchmark_returns.isna().all() else pd.Series(np.zeros(benchmark_returns.shape[0]), index=benchmark.index)
         drawdown = net_value / net_value.cummax() - 1
 
-        # # evaluation indicators
+        # evaluation indicators
         evaluation = pd.Series(name='evaluation')
         evaluation['total_return(%)'] = (net_value.iloc[-1] / net_value.iloc[0] - 1) * 100
         evaluation['annual_return(%)'] = ((evaluation['total_return(%)'] / 100 + 1) ** (
             365 / (value.index.max() - value.index.min()).days) - 1) * 100
         evaluation['annual_volatility(%)'] = (returns.std() * np.sqrt(252)) * 100
         down_volatility = (returns[returns < 0].std() * np.sqrt(252)) * 100
         enddate = drawdown.idxmin()
@@ -239,22 +270,22 @@
             ax00.legend(loc='lower left')
             ax00.set_ylabel("Cumulative Return")
             ax00_twi = ax[0,0].twinx()
             ax00_twi.fill_between(data.index, 0, data['drawdown'], color='#009100', alpha=0.3)
             ax00_twi.set_ylabel("Drawdown")
 
             if not (benchmark==0).all():
-                year = (data[['net_value', 'exvalue', 'benchmark']].resample('Y').last() - data[['net_value', 'exvalue', 'benchmark']].resample('Y').first())
+                year = (data[['net_value', 'exvalue', 'benchmark']].resample('YE').last() - data[['net_value', 'exvalue', 'benchmark']].resample('YE').first())
             else:
-                year = (data['net_value'].resample('Y').last() - data['net_value'].resample('Y').first())
-            month = (data['net_value'].resample('M').last() - data['net_value'].resample('M').first())
+                year = (data['net_value'].resample('YE').last() - data['net_value'].resample('YE').first())
+            month = (data['net_value'].resample('ME').last() - data['net_value'].resample('ME').first())
             year.index = year.index.year
             year.plot(ax=ax[0,1], kind='bar', title="Yearly Return", rot=45, colormap='Paired')
-            ax[0, 2].bar(month.index, month.values, width=20, title='Monthly Return')
-
+            ax[0, 2].bar(month.index, month.values, width=20)
+            ax[0, 2].set_title("Monthly Return")
 
             ax10 = data['exvalue'].plot(ax=ax[1,0], title='Extra Return', legend=True)
             ax10.legend(loc='lower left')
             ax10.set_ylabel("Cumulative Return")
             ax10_twi = ax[1,0].twinx()
             ax10_twi.fill_between(data.index, 0, data['exdrawdown'], color='#009100', alpha=0.3)
             ax10_twi.set_ylabel("Drawdown")
```

### Comparing `quool-5.0.8/quool/table.py` & `quool-5.1.0/quool/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 class PanelTable(Table):
     
     def __init__(
         self,
         uri: str | Path,
         code_level: str | int = 0,
         date_level: str | int = 1,
-        freq: str = "M",
+        freq: str = "ME",
         format: str = r"%Y%m",
         create: bool = False,
     ):
         self._code_level = code_level
         self._date_level = date_level
         self._freq = freq
         self._format = format
```

### Comparing `quool-5.0.8/quool/util.py` & `quool-5.1.0/quool/util.py`

 * *Files identical despite different names*

### Comparing `quool-5.0.8/setup.py` & `quool-5.1.0/setup.py`

 * *Files identical despite different names*


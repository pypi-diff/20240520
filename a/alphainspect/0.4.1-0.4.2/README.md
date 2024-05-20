# Comparing `tmp/alphainspect-0.4.1.tar.gz` & `tmp/alphainspect-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphainspect-0.4.1.tar", last modified: Thu May 16 02:07:20 2024, max compression
+gzip compressed data, was "alphainspect-0.4.2.tar", last modified: Sun May 19 11:30:28 2024, max compression
```

## Comparing `alphainspect-0.4.1.tar` & `alphainspect-0.4.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:07:20.701744 alphainspect-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-16 02:07:14.000000 alphainspect-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-16 02:07:20.701744 alphainspect-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-16 02:07:14.000000 alphainspect-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:07:20.701744 alphainspect-0.4.1/alphainspect/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-16 02:07:14.000000 alphainspect-0.4.1/alphainspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-16 02:07:14.000000 alphainspect-0.4.1/alphainspect/_nb.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 02:07:14.000000 alphainspect-0.4.1/alphainspect/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-16 02:07:14.000000 alphainspect-0.4.1/alphainspect/dtree.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-16 02:07:14.000000 alphainspect-0.4.1/alphainspect/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-05-16 02:07:14.000000 alphainspect-0.4.1/alphainspect/ic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-05-16 02:07:14.000000 alphainspect-0.4.1/alphainspect/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-16 02:07:14.000000 alphainspect-0.4.1/alphainspect/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-16 02:07:14.000000 alphainspect-0.4.1/alphainspect/returns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-16 02:07:14.000000 alphainspect-0.4.1/alphainspect/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-16 02:07:14.000000 alphainspect-0.4.1/alphainspect/turnover.py
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-05-16 02:07:14.000000 alphainspect-0.4.1/alphainspect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:07:20.701744 alphainspect-0.4.1/alphainspect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-16 02:07:20.000000 alphainspect-0.4.1/alphainspect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-16 02:07:20.000000 alphainspect-0.4.1/alphainspect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 02:07:20.000000 alphainspect-0.4.1/alphainspect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 02:07:20.000000 alphainspect-0.4.1/alphainspect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 02:07:20.000000 alphainspect-0.4.1/alphainspect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-16 02:07:14.000000 alphainspect-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 02:07:20.701744 alphainspect-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:30:28.538691 alphainspect-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-19 11:30:23.000000 alphainspect-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-19 11:30:28.534691 alphainspect-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-19 11:30:23.000000 alphainspect-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:30:28.534691 alphainspect-0.4.2/alphainspect/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-19 11:30:23.000000 alphainspect-0.4.2/alphainspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-19 11:30:23.000000 alphainspect-0.4.2/alphainspect/_nb.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 11:30:23.000000 alphainspect-0.4.2/alphainspect/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-19 11:30:23.000000 alphainspect-0.4.2/alphainspect/dtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-19 11:30:23.000000 alphainspect-0.4.2/alphainspect/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-05-19 11:30:23.000000 alphainspect-0.4.2/alphainspect/ic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-05-19 11:30:23.000000 alphainspect-0.4.2/alphainspect/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-19 11:30:23.000000 alphainspect-0.4.2/alphainspect/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-19 11:30:23.000000 alphainspect-0.4.2/alphainspect/returns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-19 11:30:23.000000 alphainspect-0.4.2/alphainspect/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-19 11:30:23.000000 alphainspect-0.4.2/alphainspect/turnover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-05-19 11:30:23.000000 alphainspect-0.4.2/alphainspect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:30:28.534691 alphainspect-0.4.2/alphainspect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-19 11:30:28.000000 alphainspect-0.4.2/alphainspect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-19 11:30:28.000000 alphainspect-0.4.2/alphainspect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:30:28.000000 alphainspect-0.4.2/alphainspect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-19 11:30:28.000000 alphainspect-0.4.2/alphainspect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 11:30:28.000000 alphainspect-0.4.2/alphainspect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-19 11:30:23.000000 alphainspect-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:30:28.538691 alphainspect-0.4.2/setup.cfg
```

### Comparing `alphainspect-0.4.1/LICENSE` & `alphainspect-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alphainspect-0.4.1/PKG-INFO` & `alphainspect-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphainspect
-Version: 0.4.1
+Version: 0.4.2
 Summary: factor performance visualization
 Author-email: wukan <wu-kan@163.com>
 License: MIT License
         
         Copyright (c) 2024 wukan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `alphainspect-0.4.1/README.md` & `alphainspect-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `alphainspect-0.4.1/alphainspect/_nb.py` & `alphainspect-0.4.2/alphainspect/_nb.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.4.1/alphainspect/dtree.py` & `alphainspect-0.4.2/alphainspect/dtree.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.4.1/alphainspect/events.py` & `alphainspect-0.4.2/alphainspect/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     mean_pd.plot.line(title='Average Cumulative Returns by Quantile', ax=ax, cmap='coolwarm', lw=1)
     ax.axvline(x=mean_pd.index.get_loc('+0'), c="r", ls="--", lw=1)
     ax.set_xlabel('')
 
 
 def plot_events_count(df_pl: pl.DataFrame, axvlines: Sequence[str] = (), ax=None) -> None:
     """事件发生次数"""
-    df_pl = df_pl.group_by(_DATE_).count()
+    df_pl = df_pl.group_by(_DATE_).count().sort(_DATE_)
     df_pd = df_pl.to_pandas().set_index(_DATE_)
     df_pd.plot.line(title='Distribution of events', ax=ax, lw=1, grid=True)
     ax.set_xlabel('')
     for v in axvlines:
         ax.axvline(x=v, c="b", ls="--", lw=1)
```

### Comparing `alphainspect-0.4.1/alphainspect/ic.py` & `alphainspect-0.4.2/alphainspect/ic.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.4.1/alphainspect/portfolio.py` & `alphainspect-0.4.2/alphainspect/portfolio.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
 def plot_quantile_portfolio(df_pd: pd.DataFrame, fwd_ret_1: str,
                             long_short=None,
                             *,
                             axvlines=None, ax=None) -> None:
     ax = df_pd.plot(ax=ax, title=f'{fwd_ret_1}', cmap='coolwarm', lw=1, grid=True)
     if long_short is not None:
-        long_short.plot(ax=ax, c="k", ls="--", lw=1, label='L-S')
+        long_short.plot(ax=ax, c="g", ls="--", lw=1, label='L-S')
     ax.legend(loc='upper left')
     ax.set_xlabel('')
     for v in axvlines:
         ax.axvline(x=v, c="b", ls="--", lw=1)
 
 
 def plot_portfolio_heatmap_monthly(df_pd: pd.DataFrame,
```

### Comparing `alphainspect-0.4.1/alphainspect/reports.py` & `alphainspect-0.4.2/alphainspect/reports.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.4.1/alphainspect/returns.py` & `alphainspect-0.4.2/alphainspect/returns.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.4.1/alphainspect/selection.py` & `alphainspect-0.4.2/alphainspect/selection.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.4.1/alphainspect/turnover.py` & `alphainspect-0.4.2/alphainspect/turnover.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.4.1/alphainspect/utils.py` & `alphainspect-0.4.2/alphainspect/utils.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.4.1/alphainspect.egg-info/PKG-INFO` & `alphainspect-0.4.2/alphainspect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphainspect
-Version: 0.4.1
+Version: 0.4.2
 Summary: factor performance visualization
 Author-email: wukan <wu-kan@163.com>
 License: MIT License
         
         Copyright (c) 2024 wukan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `alphainspect-0.4.1/pyproject.toml` & `alphainspect-0.4.2/pyproject.toml`

 * *Files identical despite different names*


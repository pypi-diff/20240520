# Comparing `tmp/atmospy-0.1.0a6.tar.gz` & `tmp/atmospy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atmospy-0.1.0a6.tar", max compression
+gzip compressed data, was "atmospy-0.1.1.tar", max compression
```

## Comparing `atmospy-0.1.0a6.tar` & `atmospy-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    11323 2024-04-25 14:04:27.380619 atmospy-0.1.0a6/LICENSE
--rw-r--r--   0        0        0     1603 2024-04-25 14:04:27.380619 atmospy-0.1.0a6/README.md
--rw-r--r--   0        0        0      411 2024-04-25 14:04:27.380619 atmospy-0.1.0a6/atmospy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 14:04:27.380619 atmospy-0.1.0a6/atmospy/_base.py
--rw-r--r--   0        0        0      640 2024-04-25 14:04:27.380619 atmospy-0.1.0a6/atmospy/distributions.py
--rw-r--r--   0        0        0     1936 2024-04-25 14:04:27.380619 atmospy-0.1.0a6/atmospy/rcmod.py
--rw-r--r--   0        0        0     4519 2024-04-25 14:04:27.380619 atmospy-0.1.0a6/atmospy/relational.py
--rw-r--r--   0        0        0     6828 2024-04-25 14:04:27.380619 atmospy-0.1.0a6/atmospy/rose.py
--rw-r--r--   0        0        0    13082 2024-04-25 14:04:27.380619 atmospy-0.1.0a6/atmospy/trends.py
--rw-r--r--   0        0        0     5208 2024-04-25 14:04:27.380619 atmospy-0.1.0a6/atmospy/utils.py
--rw-r--r--   0        0        0     1292 2024-04-25 14:04:27.384619 atmospy-0.1.0a6/pyproject.toml
--rw-r--r--   0        0        0     2641 1970-01-01 00:00:00.000000 atmospy-0.1.0a6/PKG-INFO
+-rw-r--r--   0        0        0    11323 2024-05-19 21:58:59.916768 atmospy-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1603 2024-05-19 21:58:59.916768 atmospy-0.1.1/README.md
+-rw-r--r--   0        0        0      432 2024-05-19 21:58:59.916768 atmospy-0.1.1/atmospy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 21:58:59.916768 atmospy-0.1.1/atmospy/_base.py
+-rw-r--r--   0        0        0      640 2024-05-19 21:58:59.916768 atmospy-0.1.1/atmospy/distributions.py
+-rw-r--r--   0        0        0     1936 2024-05-19 21:58:59.916768 atmospy-0.1.1/atmospy/rcmod.py
+-rw-r--r--   0        0        0     4519 2024-05-19 21:58:59.916768 atmospy-0.1.1/atmospy/relational.py
+-rw-r--r--   0        0        0     6910 2024-05-19 21:58:59.916768 atmospy-0.1.1/atmospy/rose.py
+-rw-r--r--   0        0        0     3649 2024-05-19 21:58:59.916768 atmospy-0.1.1/atmospy/stats.py
+-rw-r--r--   0        0        0    13902 2024-05-19 21:58:59.916768 atmospy-0.1.1/atmospy/trends.py
+-rw-r--r--   0        0        0     5316 2024-05-19 21:58:59.916768 atmospy-0.1.1/atmospy/utils.py
+-rw-r--r--   0        0        0     1072 2024-05-19 21:58:59.928768 atmospy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2594 1970-01-01 00:00:00.000000 atmospy-0.1.1/PKG-INFO
```

### Comparing `atmospy-0.1.0a6/LICENSE` & `atmospy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atmospy-0.1.0a6/README.md` & `atmospy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `atmospy-0.1.0a6/atmospy/distributions.py` & `atmospy-0.1.1/atmospy/distributions.py`

 * *Files identical despite different names*

### Comparing `atmospy-0.1.0a6/atmospy/rcmod.py` & `atmospy-0.1.1/atmospy/rcmod.py`

 * *Files identical despite different names*

### Comparing `atmospy-0.1.0a6/atmospy/relational.py` & `atmospy-0.1.1/atmospy/relational.py`

 * *Files identical despite different names*

### Comparing `atmospy-0.1.0a6/atmospy/rose.py` & `atmospy-0.1.1/atmospy/rose.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import math
 from .utils import (
     check_for_numeric_cols,
 )
 
+# Turn off chained assignment warnings
+pd.options.mode.chained_assignment = None
+
 __all__ = ["pollutionroseplot"]
 
 def pollutionroseplot(data=None, *, ws=None, wd=None, pollutant=None, 
                       faceted=False, segments=12, bins=[0, 10, 100, 1000], suffix="a.u.",
                       calm=0., lw=1, legend=True, palette="flare",
                       title=None, **kwargs):
     """Plot the intensity and directionality of a variable on a traditional wind-rose plot.
```

### Comparing `atmospy-0.1.0a6/atmospy/trends.py` & `atmospy-0.1.1/atmospy/trends.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,23 @@
 
 @mpl.ticker.FuncFormatter
 def custom_month_formatter(x, pos):
     return str(math.ceil(x))
 
 def _yearplot(data, x, y, ax=None, agg="mean", cmap="crest", 
               height=2, aspect=5, vmin=None, vmax=None,
-              linecolor="white", linewidths=0, cbar=True, cbar_kws=None, units=""):
+              linecolor="white", linewidths=0, cbar=True, cbar_kws=None, 
+              units="", faceted=False, **kwargs):
     """Plot a full year of time series data on a heatmap by month.
     """
     if ax is None:
         ax = plt.gca()
-        ax.figure.set_size_inches(height*aspect, height)
+        
+        if not faceted:
+            ax.figure.set_size_inches(height*aspect, height)
         
     # if more than 1Y of data was provided, limit to 1Y
     years = np.unique(data.index.year)
     if years.size > 1:
         # warn
         data = data[data.index.year == years[0]]
         
@@ -107,20 +110,23 @@
         cb.set_ticklabels(ticklabels)
     
     return ax
     
 
 def _monthplot(data, x, y, ax=None, agg="mean", height=3, aspect=1, 
                vmin=None, vmax=None, cmap="crest", linewidths=0.1,
-               linecolor="white", cbar=True, cbar_kws=None, units=None):
+               linecolor="white", cbar=True, cbar_kws=None, 
+               units=None, faceted=False, **kwargs):
     """Plot a full month of time series data on a heatmap by hour.
     """
     if ax is None:
         ax = plt.gca()
-        ax.figure.set_size_inches(height*aspect, height)
+        
+        if not faceted:
+            ax.figure.set_size_inches(height*aspect, height)
         
     # if more than 1mo of data was provided, limit to 1mo
     months = np.unique(data.index.month)
     if months.size > 1:
         # TODO: log warning
         data = data[data.index.month == months[0]]
         
@@ -182,15 +188,16 @@
     ])
     
     return ax
 
 
 def calendarplot(data, x, y, freq="day", agg="mean", vmin=None, vmax=None, cmap="crest", 
                  ax=None, linecolor="white", linewidths=0, cbar=True, cbar_kws=None,
-                 xlabel=None, ylabel=None, title=None, units="", height=2, aspect=5.0):
+                 xlabel=None, ylabel=None, title=None, units="", height=2, 
+                 aspect=5.0, faceted=False, **kwargs):
     """Visualize data as a heatmap on a monthly or annual basis.
     
     Calendar plots can be a useful way to visualize trends in data over longer periods 
     of time. This function is quite generic and allows you to visualize data either by 
     month (where the x-axis is day of month and y-axis is hour of day) or year (where 
     x-axis is the week of the year and y-axis is the day of the week). Configure the plot
     to aggregrate the data any way you choose (e.g., sum, mean, max).
@@ -238,14 +245,16 @@
         The figure title, by default None
     units : str, optional
         The units of the plotted item for labeling purposes only, by default ""
     height : int, optional
         The figure height in inches, by default 2
     aspect : float, optional
         The aspect ratio of the figure, by default 5.0
+    faceted : bool optional
+        Set to `True` if combining with a FacetGrid, optional
     
     Returns
     -------
     :class:`matplotlib.axes._axes.Axes`
 
     Examples
     --------
@@ -277,22 +286,22 @@
     df = df.set_index(x)
     
     if freq == "day":
         ax = _yearplot(
             df, x, y,
             agg=agg, height=height, aspect=aspect,
             vmin=vmin, vmax=vmax, linewidths=linewidths, linecolor=linecolor,
-            cbar=cbar, cbar_kws=cbar_kws, units=units, cmap=cmap
+            cbar=cbar, cbar_kws=cbar_kws, units=units, cmap=cmap, faceted=faceted, **kwargs
         )
     elif freq == "hour":
         ax = _monthplot(
             df, x, y,
             agg=agg, height=height, aspect=aspect,
             vmin=vmin, vmax=vmax, linewidths=linewidths, linecolor=linecolor,
-            cbar=cbar, cbar_kws=cbar_kws, units=units, cmap=cmap
+            cbar=cbar, cbar_kws=cbar_kws, units=units, cmap=cmap, faceted=faceted, **kwargs
         )
     
     ax.set_aspect("equal")
 
     # remove the spines
     for spine in ("top", "bottom", "right", "left"):
         ax.spines[spine].set_visible(False)
@@ -305,16 +314,16 @@
         
     if ylabel:
         ax.set_ylabel(ylabel)
     
     return ax
 
 
-def dielplot(data, x, y, ax=None, ylim=None, xlabel=None, 
-             ylabel=None, title=None, plot_kws=None, **kwargs):
+def dielplot(data=None, *, x=None, y=None, ax=None, ylim=None, xlabel=None, 
+             ylabel=None, title=None, color=None, show_iqr=True, plot_kws=None, **kwargs):
     """Plot the diel (e.g., diurnal) trend for a pollutant.
     
     Diel plots can be incredibly useful for understanding daily 
     patterns of air pollutants.
 
     Parameters
     ----------
@@ -330,14 +339,18 @@
         A tuple describing (ymin, ymax), by default None
     xlabel : str, optional
         The label for the x-axis, by default None
     ylabel : str, optional
         The label for the y-axis, by default None
     title : str, optional
         The title for the plot, by default None
+    color : str, optional
+        Specify the color to use in the figure
+    shoq_iqr : bool, optional
+        If True, plot the interquartile range as a shaded region, default True
     plot_kws : dict or None, optional
         Additional keyword arguments are passed directly to the underlying plot call
         , by default None
         
     Returns
     -------
     :class:`matplotlib.axes._axes.Axes`
@@ -345,57 +358,63 @@
         
     Examples
     --------
     
     Plot a simple heatmap for the entire year.
 
     >>> df = atmospy.load_dataset("us-bc")
-    >>> atmospy.dielplot(df, x="Timestamp GMT", y="Sample Measurement")
+    >>> atmospy.dielplot(data=df, x="Timestamp GMT", y="Sample Measurement")
     
     """
     default_plot_kws = {
         "lw": 3,
     }
     
     # complete some initial data quality checks
     check_for_timestamp_col(data, x)
     check_for_numeric_cols(data, [y])
     
     # 
     plot_kws = {} if plot_kws is None else dict(default_plot_kws, **plot_kws)
+    if color is not None:
+        plot_kws.update(dict(c=color))
     
     # copy over only the needed data
     _data = data[[x, y]].copy(deep=True)
     _data = _data.set_index(x)
     
     # 
     # figure setup
     if ax is None:
         ax = plt.gca()
         
     # compute the diel statistics
     stats = _data.groupby([_data.index.hour, _data.index.minute], as_index=False).describe()
     
+    # append the first record so the first and last records are identical
+    stats.loc[len(stats.index)] = stats.loc[0]
+    
     # build an index we can use to make the figure
     index = stats.index.values
-    freq = int(60 / (index.size / 24))
+    freq = int(60 / ((index.size - 1) / 24))
     figure_index = pd.date_range(start='2020-01-01', periods=index.size, freq=f"{freq}min")
     
     # plot the diel average
     ax.plot(figure_index, stats[y]['mean'], **plot_kws)
     
     # add the IQR as a shaded region
-    ax.fill_between(
-        figure_index,
-        y1=stats[y]['25%'],
-        y2=stats[y]['75%'],
-        alpha=0.25,
-        lw=2,
-        color=plt.gca().lines[-1].get_color()
-    )
+    if show_iqr:
+        ax.fill_between(
+            figure_index,
+            y1=stats[y]['25%'],
+            y2=stats[y]['75%'],
+            alpha=0.25,
+            lw=2,
+            color=plt.gca().lines[-1].get_color()
+        )
     
     # adjust plot parameters
     xticks = ax.get_xticks()
     ax.set_xticks(np.linspace(xticks[0], xticks[-1], 5))
     ax.set(xlim=(xticks[0], xticks[-1]))
     ax.xaxis.set_major_formatter(mpl.dates.DateFormatter("%I:%M\n%p"))
     ax.xaxis.set_minor_locator(mpl.dates.HourLocator(interval=1))
```

### Comparing `atmospy-0.1.0a6/atmospy/utils.py` & `atmospy-0.1.1/atmospy/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,14 +122,17 @@
             lambda x: x["Timestamp GMT"] + pd.Timedelta(hours=x["GMT Offset"]), axis=1)
         
     if name == "air-sensors-pm":
         df["timestamp"] = pd.to_datetime(df["timestamp"])
     
     if name == "air-sensors-met":
         df["timestamp_local"] = pd.to_datetime(df["timestamp_local"])
+        
+        # only keep data after april
+        df = df[df["timestamp_local"] >= "2023-05-01"].copy()
     
     return df
 
 def remove_na(vec):
     return
 
 def check_for_timestamp_col(data, col):
```

### Comparing `atmospy-0.1.0a6/pyproject.toml` & `atmospy-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 [tool.poetry]
 name = "atmospy"
-version = "0.1.0a6"
+version = "0.1.1"
 description = "Data analysis and visualization for air quality data."
 authors = ["David H Hagan <david.hagan@quant-aq.com>"]
 license = "Apache-2.0"
 maintainers = []
 readme = "README.md"
 homepage = "https://github.com/dhhagan/atmospy/"
 repository = "https://github.com/dhhagan/atmospy/"
 documentation = "https://dhhagan.github.io/atmospy/"
 packages = [
     { include = "atmospy" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8"
+python = ">=3.8,<3.12"
 pandas = ">=1.2"
 numpy = ">=1.20,<1.24.0 || >1.24.0"
 matplotlib = ">=3.4,<3.6.1 || >3.6.1"
 seaborn = ">=0.12"
 scipy = ">=1.7"
 
-# [tool.poetry.dev-dependencies]
-# pytest = "^6.2.4"
-# pytest-cov = "^2.12.1"
-# jupyter = "^1.0.0"
-# Sphinx = "^4.0.2"
-# pandoc = "^1.0.2"
-# sphinx-bootstrap-theme = "^0.7.1"
-# numpydoc = "^1.1.0"
-# sphinx-issues = "^1.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 ipykernel = "^6.29.4"
 jupyter = "^1.0.0"
 sphinx = "<6.0.0"
```

### Comparing `atmospy-0.1.0a6/PKG-INFO` & `atmospy-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: atmospy
-Version: 0.1.0a6
+Version: 0.1.1
 Summary: Data analysis and visualization for air quality data.
 Home-page: https://github.com/dhhagan/atmospy/
 License: Apache-2.0
 Author: David H Hagan
 Author-email: david.hagan@quant-aq.com
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: matplotlib (>=3.4,!=3.6.1)
 Requires-Dist: numpy (>=1.20,!=1.24.0)
 Requires-Dist: pandas (>=1.2)
 Requires-Dist: scipy (>=1.7)
 Requires-Dist: seaborn (>=0.12)
 Project-URL: Bug Tracker, https://github.com/quant-aq/atmospy/issues
 Project-URL: Documentation, https://dhhagan.github.io/atmospy/
```


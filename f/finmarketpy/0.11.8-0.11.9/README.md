# Comparing `tmp/finmarketpy-0.11.8.tar.gz` & `tmp/finmarketpy-0.11.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\finmarketpy-0.11.8.tar", last modified: Mon Jan 25 15:00:30 2021, max compression
+gzip compressed data, was "dist\finmarketpy-0.11.9.tar", last modified: Tue Jun  1 16:10:21 2021, max compression
```

## Comparing `finmarketpy-0.11.8.tar` & `finmarketpy-0.11.9.tar`

### file list

```diff
@@ -1,110 +1,106 @@
-drwxrwxrwx   0        0        0        0 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/
--rw-rw-rw-   0        0        0       96 2016-08-17 15:04:18.000000 finmarketpy-0.11.8/.gitattributes
-drwxrwxrwx   0        0        0        0 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/.github/
--rw-rw-rw-   0        0        0      656 2020-07-01 07:02:55.000000 finmarketpy-0.11.8/.github/FUNDING.yml
--rw-rw-rw-   0        0        0      869 2019-10-23 08:19:35.000000 finmarketpy-0.11.8/.gitignore
--rw-rw-rw-   0        0        0    17360 2020-12-24 23:38:47.000000 finmarketpy-0.11.8/INSTALL.md
--rw-rw-rw-   0        0        0    11580 2016-08-17 12:31:22.000000 finmarketpy-0.11.8/LICENCE
--rw-rw-rw-   0        0        0      130 2021-01-23 00:06:47.000000 finmarketpy-0.11.8/MANIFEST.in
--rw-rw-rw-   0        0        0      595 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/PKG-INFO
--rw-rw-rw-   0        0        0     2380 2017-09-17 16:42:36.000000 finmarketpy-0.11.8/PLANNED_FEATURES.md
--rw-rw-rw-   0        0        0    20782 2021-01-25 14:59:35.000000 finmarketpy-0.11.8/README.md
-drwxrwxrwx   0        0        0        0 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/binder/
--rw-rw-rw-   0        0        0     1423 2020-11-13 17:14:55.000000 finmarketpy-0.11.8/binder/Dockerfile
--rwxrwxrwx   0        0        0       41 2015-12-10 11:19:46.000000 finmarketpy-0.11.8/create_package.bat
-drwxrwxrwx   0        0        0        0 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/doc/
--rw-rw-rw-   0        0        0        0 2017-01-18 12:16:42.000000 finmarketpy-0.11.8/doc/__init__.py
-drwxrwxrwx   0        0        0        0 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/finmarketpy/
--rw-rw-rw-   0        0        0       51 2016-08-22 15:14:28.000000 finmarketpy-0.11.8/finmarketpy/__init__.py
-drwxrwxrwx   0        0        0        0 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/finmarketpy/backtest/
--rw-rw-rw-   0        0        0      274 2016-08-12 13:33:24.000000 finmarketpy-0.11.8/finmarketpy/backtest/__init__.py
--rw-rw-rw-   0        0        0     3820 2020-12-20 23:07:50.000000 finmarketpy-0.11.8/finmarketpy/backtest/backtestcomparison.py
--rw-rw-rw-   0        0        0    90952 2021-01-13 00:00:01.000000 finmarketpy-0.11.8/finmarketpy/backtest/backtestengine.py
--rw-rw-rw-   0        0        0    15253 2020-12-20 23:06:02.000000 finmarketpy-0.11.8/finmarketpy/backtest/backtestrequest.py
--rw-rw-rw-   0        0        0    19730 2020-12-20 23:06:14.000000 finmarketpy-0.11.8/finmarketpy/backtest/tradeanalysis.py
-drwxrwxrwx   0        0        0        0 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/finmarketpy/curve/
--rw-rw-rw-   0        0        0      175 2020-12-16 09:58:33.000000 finmarketpy-0.11.8/finmarketpy/curve/__init__.py
--rw-rw-rw-   0        0        0     1173 2020-12-20 23:12:19.000000 finmarketpy-0.11.8/finmarketpy/curve/abstractcurve.py
--rw-rw-rw-   0        0        0      801 2020-12-21 14:46:36.000000 finmarketpy-0.11.8/finmarketpy/curve/abstractpricer.py
--rw-rw-rw-   0        0        0    19102 2021-01-09 17:36:59.000000 finmarketpy-0.11.8/finmarketpy/curve/fxforwardscurve.py
--rw-rw-rw-   0        0        0    39421 2021-01-16 15:05:31.000000 finmarketpy-0.11.8/finmarketpy/curve/fxoptionscurve.py
--rw-rw-rw-   0        0        0    11770 2021-01-22 12:29:15.000000 finmarketpy-0.11.8/finmarketpy/curve/fxspotcurve.py
-drwxrwxrwx   0        0        0        0 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/finmarketpy/curve/rates/
--rw-rw-rw-   0        0        0        0 2020-12-19 23:06:28.000000 finmarketpy-0.11.8/finmarketpy/curve/rates/__init__.py
--rw-rw-rw-   0        0        0    17813 2021-01-12 19:07:09.000000 finmarketpy-0.11.8/finmarketpy/curve/rates/fxforwardspricer.py
-drwxrwxrwx   0        0        0        0 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/finmarketpy/curve/volatility/
--rw-rw-rw-   0        0        0        0 2020-10-06 12:05:42.000000 finmarketpy-0.11.8/finmarketpy/curve/volatility/__init__.py
--rw-rw-rw-   0        0        0     3005 2021-01-17 18:00:01.000000 finmarketpy-0.11.8/finmarketpy/curve/volatility/abstractvolsurface.py
--rw-rw-rw-   0        0        0    12333 2021-01-16 17:17:32.000000 finmarketpy-0.11.8/finmarketpy/curve/volatility/fxoptionspricer.py
--rw-rw-rw-   0        0        0    21046 2021-01-16 14:19:48.000000 finmarketpy-0.11.8/finmarketpy/curve/volatility/fxvolsurface.py
--rw-rw-rw-   0        0        0    11290 2020-12-20 23:07:57.000000 finmarketpy-0.11.8/finmarketpy/curve/volatility/volstats.py
-drwxrwxrwx   0        0        0        0 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/finmarketpy/economics/
--rw-rw-rw-   0        0        0      474 2020-05-05 17:22:21.000000 finmarketpy-0.11.8/finmarketpy/economics/__init__.py
--rw-rw-rw-   0        0        0    25405 2020-12-20 23:08:15.000000 finmarketpy-0.11.8/finmarketpy/economics/eventstudy.py
--rw-rw-rw-   0        0        0     1843 2020-12-20 23:08:19.000000 finmarketpy-0.11.8/finmarketpy/economics/marketliquidity.py
--rw-rw-rw-   0        0        0     6090 2021-01-08 19:01:02.000000 finmarketpy-0.11.8/finmarketpy/economics/quickchart.py
--rw-rw-rw-   0        0        0     3500 2020-12-20 23:11:58.000000 finmarketpy-0.11.8/finmarketpy/economics/report.py
--rw-rw-rw-   0        0        0     7189 2020-12-20 23:08:29.000000 finmarketpy-0.11.8/finmarketpy/economics/seasonality.py
--rw-rw-rw-   0        0        0    19044 2020-12-20 23:08:39.000000 finmarketpy-0.11.8/finmarketpy/economics/techindicator.py
--rw-rw-rw-   0        0        0        0 2017-01-18 15:39:22.000000 finmarketpy-0.11.8/finmarketpy/make.py
-drwxrwxrwx   0        0        0        0 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/finmarketpy/network_analysis/
--rw-rw-rw-   0        0        0      130 2019-11-02 18:59:45.000000 finmarketpy-0.11.8/finmarketpy/network_analysis/__init__.py
--rw-rw-rw-   0        0        0     4978 2020-12-20 23:09:00.000000 finmarketpy-0.11.8/finmarketpy/network_analysis/learn_network_structure.py
--rw-rw-rw-   0        0        0     4971 2019-11-14 16:02:25.000000 finmarketpy-0.11.8/finmarketpy/network_analysis/plot_network_structure.py
-drwxrwxrwx   0        0        0        0 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/finmarketpy/util/
--rw-rw-rw-   0        0        0        0 2016-08-15 18:03:48.000000 finmarketpy-0.11.8/finmarketpy/util/__init__.py
--rw-rw-rw-   0        0        0     5676 2021-01-16 17:19:37.000000 finmarketpy-0.11.8/finmarketpy/util/marketconstants.py
--rw-rw-rw-   0        0        0     2587 2020-12-20 23:09:21.000000 finmarketpy-0.11.8/finmarketpy/util/marketutil.py
-drwxrwxrwx   0        0        0        0 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/finmarketpy.egg-info/
--rw-rw-rw-   0        0        0      595 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/finmarketpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3384 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/finmarketpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/finmarketpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2016-09-15 15:32:08.000000 finmarketpy-0.11.8/finmarketpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       92 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/finmarketpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       43 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/finmarketpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/finmarketpy_examples/
--rw-rw-rw-   0        0        0        0 2016-08-11 14:20:42.000000 finmarketpy-0.11.8/finmarketpy_examples/__init__.py
--rw-rw-rw-   0        0        0     7818 2020-12-20 23:11:50.000000 finmarketpy-0.11.8/finmarketpy_examples/backtest_example.py
--rw-rw-rw-   0        0        0   133447 2020-05-07 14:07:30.000000 finmarketpy-0.11.8/finmarketpy_examples/boe-rate.png
--rw-rw-rw-   0        0        0      422 2017-06-14 11:11:30.000000 finmarketpy-0.11.8/finmarketpy_examples/download_data_ams.py
--rw-rw-rw-   0        0        0      408 2021-01-03 19:42:04.000000 finmarketpy-0.11.8/finmarketpy_examples/dukascopy_example.py
--rw-rw-rw-   0        0        0     4313 2020-12-20 23:09:31.000000 finmarketpy-0.11.8/finmarketpy_examples/events_examples.py
-drwxrwxrwx   0        0        0        0 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/finmarketpy_examples/finmarketpy_notebooks/
--rw-rw-rw-   0        0        0        0 2019-11-03 14:18:28.000000 finmarketpy-0.11.8/finmarketpy_examples/finmarketpy_notebooks/__init__.py
--rw-rw-rw-   0        0        0    60300 2020-11-13 16:18:14.000000 finmarketpy-0.11.8/finmarketpy_examples/finmarketpy_notebooks/backtest_example.ipynb
--rw-rw-rw-   0        0        0   177064 2020-11-12 13:59:09.000000 finmarketpy-0.11.8/finmarketpy_examples/finmarketpy_notebooks/quandl_example.ipynb
--rw-rw-rw-   0        0        0     8658 2020-12-26 18:36:40.000000 finmarketpy-0.11.8/finmarketpy_examples/fx_forwards_indices_examples.py
--rw-rw-rw-   0        0        0     4884 2020-12-23 19:13:26.000000 finmarketpy-0.11.8/finmarketpy_examples/fx_forwards_pricing_examples.py
--rw-rw-rw-   0        0        0    11550 2021-01-22 15:06:57.000000 finmarketpy-0.11.8/finmarketpy_examples/fx_options_indices_examples.py
--rw-rw-rw-   0        0        0    10691 2021-01-16 14:14:06.000000 finmarketpy-0.11.8/finmarketpy_examples/fx_options_pricing_examples.py
--rw-rw-rw-   0        0        0     6535 2021-01-22 15:13:59.000000 finmarketpy-0.11.8/finmarketpy_examples/fx_spot_indices_examples.py
--rw-rw-rw-   0        0        0     2529 2020-12-20 23:05:32.000000 finmarketpy-0.11.8/finmarketpy_examples/fx_vol_surface_animation.py
--rw-rw-rw-   0        0        0    10332 2021-01-17 18:00:29.000000 finmarketpy-0.11.8/finmarketpy_examples/fx_vol_surface_interpolation_examples.py
-drwxrwxrwx   0        0        0        0 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/finmarketpy_examples/gallery/
--rw-rw-rw-   0        0        0        0 2016-08-17 15:22:02.000000 finmarketpy-0.11.8/finmarketpy_examples/gallery/__init__.py
--rw-rw-rw-   0        0        0   147546 2016-08-17 15:11:26.000000 finmarketpy-0.11.8/finmarketpy_examples/gallery/fx-trend-cumulative.png
--rw-rw-rw-   0        0        0   141286 2016-08-17 15:11:30.000000 finmarketpy-0.11.8/finmarketpy_examples/gallery/fx-trend-leverage.png
--rw-rw-rw-   0        0        0   368124 2016-08-17 15:11:36.000000 finmarketpy-0.11.8/finmarketpy_examples/gallery/fx-trend-trade-returns.png
--rw-rw-rw-   0        0        0   276893 2016-09-01 09:55:14.000000 finmarketpy-0.11.8/finmarketpy_examples/gallery/fx-vol-seasonality.png
--rw-rw-rw-   0        0        0   123694 2016-08-23 14:03:12.000000 finmarketpy-0.11.8/finmarketpy_examples/gallery/gold-seasonality.png
--rw-rw-rw-   0        0        0   222562 2016-09-02 16:34:56.000000 finmarketpy-0.11.8/finmarketpy_examples/gallery/usdjpy-nfp.png
--rw-rw-rw-   0        0        0   123575 2016-08-23 14:29:42.000000 finmarketpy-0.11.8/finmarketpy_examples/gold seasonality.png
--rw-rw-rw-   0        0        0      428 2020-12-31 14:45:07.000000 finmarketpy-0.11.8/finmarketpy_examples/new_dukascopy.py
--rw-rw-rw-   0        0        0     2292 2020-12-20 23:09:41.000000 finmarketpy-0.11.8/finmarketpy_examples/quandl_examples.py
--rw-rw-rw-   0        0        0     2543 2020-12-20 23:09:45.000000 finmarketpy-0.11.8/finmarketpy_examples/quickchart_examples.py
--rw-rw-rw-   0        0        0     2230 2020-12-20 23:09:48.000000 finmarketpy-0.11.8/finmarketpy_examples/returns_examples.py
--rw-rw-rw-   0        0        0     7943 2020-12-20 23:09:51.000000 finmarketpy-0.11.8/finmarketpy_examples/seasonality_examples.py
--rw-rw-rw-   0        0        0     2425 2020-12-20 23:09:55.000000 finmarketpy-0.11.8/finmarketpy_examples/technicals_example.py
--rw-rw-rw-   0        0        0     9380 2020-12-20 23:10:04.000000 finmarketpy-0.11.8/finmarketpy_examples/tradingmodelfxtrend_bbg_example.py
--rw-rw-rw-   0        0        0     9654 2020-12-20 23:10:07.000000 finmarketpy-0.11.8/finmarketpy_examples/tradingmodelfxtrend_example.py
--rw-rw-rw-   0        0        0    10706 2020-12-20 23:10:16.000000 finmarketpy-0.11.8/finmarketpy_examples/vol_stats_examples.py
--rw-rw-rw-   0        0        0     1496 2020-12-20 23:10:26.000000 finmarketpy-0.11.8/finmarketpy_examples/vwap_example.py
--rw-rw-rw-   0        0        0    23395 2017-02-11 12:58:16.000000 finmarketpy-0.11.8/finmarketpy_logo.png
--rwxrwxrwx   0        0        0      497 2017-02-16 10:20:44.000000 finmarketpy-0.11.8/install_extra_packages.bat
--rw-rw-rw-   0        0        0       31 2020-11-12 13:55:34.000000 finmarketpy-0.11.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/setup.cfg
--rw-rw-rw-   0        0        0     1227 2021-01-25 14:59:12.000000 finmarketpy-0.11.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-01-25 15:00:30.000000 finmarketpy-0.11.8/tests/
--rw-rw-rw-   0        0        0        0 2019-11-02 13:56:21.000000 finmarketpy-0.11.8/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2019-11-02 18:59:45.000000 finmarketpy-0.11.8/tests/test_backtestengine.py
--rw-rw-rw-   0        0        0    25800 2020-12-20 23:11:14.000000 finmarketpy-0.11.8/tests/test_techindicator.py
+drwxrwxrwx   0        0        0        0 2021-06-01 16:10:21.451338 finmarketpy-0.11.9/
+-rw-rw-rw-   0        0        0       96 2016-08-17 15:04:18.000000 finmarketpy-0.11.9/.gitattributes
+drwxrwxrwx   0        0        0        0 2021-06-01 16:10:21.379593 finmarketpy-0.11.9/.github/
+-rw-rw-rw-   0        0        0      656 2020-07-01 07:02:55.000000 finmarketpy-0.11.9/.github/FUNDING.yml
+-rw-rw-rw-   0        0        0      877 2021-05-26 15:52:01.000000 finmarketpy-0.11.9/.gitignore
+-rw-rw-rw-   0        0        0    17360 2020-12-24 23:38:47.000000 finmarketpy-0.11.9/INSTALL.md
+-rw-rw-rw-   0        0        0    11580 2016-08-17 12:31:22.000000 finmarketpy-0.11.9/LICENCE
+-rw-rw-rw-   0        0        0      130 2021-01-23 00:06:47.000000 finmarketpy-0.11.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      595 2021-06-01 16:10:21.451338 finmarketpy-0.11.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2380 2017-09-17 16:42:36.000000 finmarketpy-0.11.9/PLANNED_FEATURES.md
+-rw-rw-rw-   0        0        0    22202 2021-06-01 16:04:33.000000 finmarketpy-0.11.9/README.md
+drwxrwxrwx   0        0        0        0 2021-06-01 16:10:21.380593 finmarketpy-0.11.9/binder/
+-rw-rw-rw-   0        0        0     1423 2020-11-13 17:14:55.000000 finmarketpy-0.11.9/binder/Dockerfile
+-rwxrwxrwx   0        0        0       41 2015-12-10 11:19:46.000000 finmarketpy-0.11.9/create_package.bat
+drwxrwxrwx   0        0        0        0 2021-06-01 16:10:21.381590 finmarketpy-0.11.9/doc/
+-rw-rw-rw-   0        0        0        0 2017-01-18 12:16:42.000000 finmarketpy-0.11.9/doc/__init__.py
+drwxrwxrwx   0        0        0        0 2021-06-01 16:10:21.382592 finmarketpy-0.11.9/finmarketpy/
+-rw-rw-rw-   0        0        0       51 2016-08-22 15:14:28.000000 finmarketpy-0.11.9/finmarketpy/__init__.py
+drwxrwxrwx   0        0        0        0 2021-06-01 16:10:21.400589 finmarketpy-0.11.9/finmarketpy/backtest/
+-rw-rw-rw-   0        0        0      274 2016-08-12 13:33:24.000000 finmarketpy-0.11.9/finmarketpy/backtest/__init__.py
+-rw-rw-rw-   0        0        0     3820 2020-12-20 23:07:50.000000 finmarketpy-0.11.9/finmarketpy/backtest/backtestcomparison.py
+-rw-rw-rw-   0        0        0   102182 2021-05-21 15:48:43.000000 finmarketpy-0.11.9/finmarketpy/backtest/backtestengine.py
+-rw-rw-rw-   0        0        0    16095 2021-03-07 23:29:43.000000 finmarketpy-0.11.9/finmarketpy/backtest/backtestrequest.py
+-rw-rw-rw-   0        0        0    19766 2021-01-30 15:02:11.000000 finmarketpy-0.11.9/finmarketpy/backtest/tradeanalysis.py
+drwxrwxrwx   0        0        0        0 2021-06-01 16:10:21.405591 finmarketpy-0.11.9/finmarketpy/curve/
+-rw-rw-rw-   0        0        0      175 2020-12-16 09:58:33.000000 finmarketpy-0.11.9/finmarketpy/curve/__init__.py
+-rw-rw-rw-   0        0        0     1173 2020-12-20 23:12:19.000000 finmarketpy-0.11.9/finmarketpy/curve/abstractcurve.py
+-rw-rw-rw-   0        0        0      801 2020-12-21 14:46:36.000000 finmarketpy-0.11.9/finmarketpy/curve/abstractpricer.py
+-rw-rw-rw-   0        0        0    19493 2021-05-04 15:42:55.000000 finmarketpy-0.11.9/finmarketpy/curve/fxforwardscurve.py
+-rw-rw-rw-   0        0        0    39487 2021-02-16 12:21:15.000000 finmarketpy-0.11.9/finmarketpy/curve/fxoptionscurve.py
+-rw-rw-rw-   0        0        0    12105 2021-02-10 12:05:19.000000 finmarketpy-0.11.9/finmarketpy/curve/fxspotcurve.py
+drwxrwxrwx   0        0        0        0 2021-06-01 16:10:21.406590 finmarketpy-0.11.9/finmarketpy/curve/rates/
+-rw-rw-rw-   0        0        0        0 2020-12-19 23:06:28.000000 finmarketpy-0.11.9/finmarketpy/curve/rates/__init__.py
+-rw-rw-rw-   0        0        0    17813 2021-01-12 19:07:09.000000 finmarketpy-0.11.9/finmarketpy/curve/rates/fxforwardspricer.py
+drwxrwxrwx   0        0        0        0 2021-06-01 16:10:21.410590 finmarketpy-0.11.9/finmarketpy/curve/volatility/
+-rw-rw-rw-   0        0        0        0 2020-10-06 12:05:42.000000 finmarketpy-0.11.9/finmarketpy/curve/volatility/__init__.py
+-rw-rw-rw-   0        0        0     3061 2021-02-17 00:01:06.000000 finmarketpy-0.11.9/finmarketpy/curve/volatility/abstractvolsurface.py
+-rw-rw-rw-   0        0        0    13613 2021-02-17 00:07:49.000000 finmarketpy-0.11.9/finmarketpy/curve/volatility/fxoptionspricer.py
+-rw-rw-rw-   0        0        0    21676 2021-02-17 00:01:37.000000 finmarketpy-0.11.9/finmarketpy/curve/volatility/fxvolsurface.py
+-rw-rw-rw-   0        0        0    11290 2020-12-20 23:07:57.000000 finmarketpy-0.11.9/finmarketpy/curve/volatility/volstats.py
+drwxrwxrwx   0        0        0        0 2021-06-01 16:10:21.415591 finmarketpy-0.11.9/finmarketpy/economics/
+-rw-rw-rw-   0        0        0      474 2020-05-05 17:22:21.000000 finmarketpy-0.11.9/finmarketpy/economics/__init__.py
+-rw-rw-rw-   0        0        0    28182 2021-04-08 18:34:37.000000 finmarketpy-0.11.9/finmarketpy/economics/eventstudy.py
+-rw-rw-rw-   0        0        0     1843 2020-12-20 23:08:19.000000 finmarketpy-0.11.9/finmarketpy/economics/marketliquidity.py
+-rw-rw-rw-   0        0        0     6090 2021-01-08 19:01:02.000000 finmarketpy-0.11.9/finmarketpy/economics/quickchart.py
+-rw-rw-rw-   0        0        0     3500 2020-12-20 23:11:58.000000 finmarketpy-0.11.9/finmarketpy/economics/report.py
+-rw-rw-rw-   0        0        0     7554 2021-01-26 17:39:37.000000 finmarketpy-0.11.9/finmarketpy/economics/seasonality.py
+-rw-rw-rw-   0        0        0    19769 2021-04-13 12:37:01.000000 finmarketpy-0.11.9/finmarketpy/economics/techindicator.py
+drwxrwxrwx   0        0        0        0 2021-06-01 16:10:21.418590 finmarketpy-0.11.9/finmarketpy/network_analysis/
+-rw-rw-rw-   0        0        0      130 2019-11-02 18:59:45.000000 finmarketpy-0.11.9/finmarketpy/network_analysis/__init__.py
+-rw-rw-rw-   0        0        0     4978 2020-12-20 23:09:00.000000 finmarketpy-0.11.9/finmarketpy/network_analysis/learn_network_structure.py
+-rw-rw-rw-   0        0        0     4971 2019-11-14 16:02:25.000000 finmarketpy-0.11.9/finmarketpy/network_analysis/plot_network_structure.py
+drwxrwxrwx   0        0        0        0 2021-06-01 16:10:21.421589 finmarketpy-0.11.9/finmarketpy/util/
+-rw-rw-rw-   0        0        0        0 2016-08-15 18:03:48.000000 finmarketpy-0.11.9/finmarketpy/util/__init__.py
+-rw-rw-rw-   0        0        0     6158 2021-04-14 18:24:40.000000 finmarketpy-0.11.9/finmarketpy/util/marketconstants.py
+-rw-rw-rw-   0        0        0     2587 2020-12-20 23:09:21.000000 finmarketpy-0.11.9/finmarketpy/util/marketutil.py
+drwxrwxrwx   0        0        0        0 2021-06-01 16:10:21.396590 finmarketpy-0.11.9/finmarketpy.egg-info/
+-rw-rw-rw-   0        0        0      595 2021-06-01 16:10:21.000000 finmarketpy-0.11.9/finmarketpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3247 2021-06-01 16:10:21.000000 finmarketpy-0.11.9/finmarketpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-06-01 16:10:21.000000 finmarketpy-0.11.9/finmarketpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2016-09-15 15:32:08.000000 finmarketpy-0.11.9/finmarketpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       92 2021-06-01 16:10:21.000000 finmarketpy-0.11.9/finmarketpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       43 2021-06-01 16:10:21.000000 finmarketpy-0.11.9/finmarketpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-06-01 16:10:21.438341 finmarketpy-0.11.9/finmarketpy_examples/
+-rw-rw-rw-   0        0        0        0 2016-08-11 14:20:42.000000 finmarketpy-0.11.9/finmarketpy_examples/__init__.py
+-rw-rw-rw-   0        0        0     7818 2020-12-20 23:11:50.000000 finmarketpy-0.11.9/finmarketpy_examples/backtest_example.py
+-rw-rw-rw-   0        0        0   133447 2020-05-07 14:07:30.000000 finmarketpy-0.11.9/finmarketpy_examples/boe-rate.png
+-rw-rw-rw-   0        0        0     4314 2021-03-13 18:50:03.000000 finmarketpy-0.11.9/finmarketpy_examples/events_examples.py
+drwxrwxrwx   0        0        0        0 2021-06-01 16:10:21.440338 finmarketpy-0.11.9/finmarketpy_examples/finmarketpy_notebooks/
+-rw-rw-rw-   0        0        0        0 2019-11-03 14:18:28.000000 finmarketpy-0.11.9/finmarketpy_examples/finmarketpy_notebooks/__init__.py
+-rw-rw-rw-   0        0        0    59946 2021-05-04 15:56:54.000000 finmarketpy-0.11.9/finmarketpy_examples/finmarketpy_notebooks/backtest_example.ipynb
+-rw-rw-rw-   0        0        0   191846 2021-06-01 15:54:54.000000 finmarketpy-0.11.9/finmarketpy_examples/finmarketpy_notebooks/market_data_example.ipynb
+-rw-rw-rw-   0        0        0     8658 2021-01-30 15:03:52.000000 finmarketpy-0.11.9/finmarketpy_examples/fx_forwards_indices_examples.py
+-rw-rw-rw-   0        0        0     4884 2021-01-30 15:03:42.000000 finmarketpy-0.11.9/finmarketpy_examples/fx_forwards_pricing_examples.py
+-rw-rw-rw-   0        0        0    12454 2021-02-26 18:38:22.000000 finmarketpy-0.11.9/finmarketpy_examples/fx_options_indices_examples.py
+-rw-rw-rw-   0        0        0    12874 2021-02-22 16:04:42.000000 finmarketpy-0.11.9/finmarketpy_examples/fx_options_pricing_examples.py
+-rw-rw-rw-   0        0        0     6535 2021-01-30 15:04:31.000000 finmarketpy-0.11.9/finmarketpy_examples/fx_spot_indices_examples.py
+-rw-rw-rw-   0        0        0     2529 2020-12-20 23:05:32.000000 finmarketpy-0.11.9/finmarketpy_examples/fx_vol_surface_animation.py
+-rw-rw-rw-   0        0        0    10373 2021-03-30 09:32:34.000000 finmarketpy-0.11.9/finmarketpy_examples/fx_vol_surface_interpolation_examples.py
+drwxrwxrwx   0        0        0        0 2021-06-01 16:10:21.448337 finmarketpy-0.11.9/finmarketpy_examples/gallery/
+-rw-rw-rw-   0        0        0        0 2016-08-17 15:22:02.000000 finmarketpy-0.11.9/finmarketpy_examples/gallery/__init__.py
+-rw-rw-rw-   0        0        0   147546 2016-08-17 15:11:26.000000 finmarketpy-0.11.9/finmarketpy_examples/gallery/fx-trend-cumulative.png
+-rw-rw-rw-   0        0        0   141286 2016-08-17 15:11:30.000000 finmarketpy-0.11.9/finmarketpy_examples/gallery/fx-trend-leverage.png
+-rw-rw-rw-   0        0        0   368124 2016-08-17 15:11:36.000000 finmarketpy-0.11.9/finmarketpy_examples/gallery/fx-trend-trade-returns.png
+-rw-rw-rw-   0        0        0   276893 2016-09-01 09:55:14.000000 finmarketpy-0.11.9/finmarketpy_examples/gallery/fx-vol-seasonality.png
+-rw-rw-rw-   0        0        0   123694 2016-08-23 14:03:12.000000 finmarketpy-0.11.9/finmarketpy_examples/gallery/gold-seasonality.png
+-rw-rw-rw-   0        0        0   222562 2016-09-02 16:34:56.000000 finmarketpy-0.11.9/finmarketpy_examples/gallery/usdjpy-nfp.png
+-rw-rw-rw-   0        0        0   123575 2016-08-23 14:29:42.000000 finmarketpy-0.11.9/finmarketpy_examples/gold seasonality.png
+-rw-rw-rw-   0        0        0     2292 2020-12-20 23:09:41.000000 finmarketpy-0.11.9/finmarketpy_examples/quandl_examples.py
+-rw-rw-rw-   0        0        0     2543 2020-12-20 23:09:45.000000 finmarketpy-0.11.9/finmarketpy_examples/quickchart_examples.py
+-rw-rw-rw-   0        0        0     2230 2020-12-20 23:09:48.000000 finmarketpy-0.11.9/finmarketpy_examples/returns_examples.py
+-rw-rw-rw-   0        0        0     7943 2020-12-20 23:09:51.000000 finmarketpy-0.11.9/finmarketpy_examples/seasonality_examples.py
+-rw-rw-rw-   0        0        0     2425 2020-12-20 23:09:55.000000 finmarketpy-0.11.9/finmarketpy_examples/technicals_example.py
+-rw-rw-rw-   0        0        0     9380 2020-12-20 23:10:04.000000 finmarketpy-0.11.9/finmarketpy_examples/tradingmodelfxtrend_bbg_example.py
+-rw-rw-rw-   0        0        0     9654 2020-12-20 23:10:07.000000 finmarketpy-0.11.9/finmarketpy_examples/tradingmodelfxtrend_example.py
+-rw-rw-rw-   0        0        0    10705 2021-02-11 13:42:53.000000 finmarketpy-0.11.9/finmarketpy_examples/vol_stats_examples.py
+-rw-rw-rw-   0        0        0     1496 2020-12-20 23:10:26.000000 finmarketpy-0.11.9/finmarketpy_examples/vwap_example.py
+-rw-rw-rw-   0        0        0    23395 2017-02-11 12:58:16.000000 finmarketpy-0.11.9/finmarketpy_logo.png
+-rwxrwxrwx   0        0        0      497 2017-02-16 10:20:44.000000 finmarketpy-0.11.9/install_extra_packages.bat
+-rw-rw-rw-   0        0        0       31 2020-11-12 13:55:34.000000 finmarketpy-0.11.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2021-06-01 16:10:21.452346 finmarketpy-0.11.9/setup.cfg
+-rw-rw-rw-   0        0        0     1227 2021-06-01 16:02:41.000000 finmarketpy-0.11.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-06-01 16:10:21.450338 finmarketpy-0.11.9/tests/
+-rw-rw-rw-   0        0        0        0 2019-11-02 13:56:21.000000 finmarketpy-0.11.9/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2019-11-02 18:59:45.000000 finmarketpy-0.11.9/tests/test_backtestengine.py
+-rw-rw-rw-   0        0        0    25800 2020-12-20 23:11:14.000000 finmarketpy-0.11.9/tests/test_techindicator.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `finmarketpy-0.11.8/.github/FUNDING.yml` & `finmarketpy-0.11.9/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/.gitignore` & `finmarketpy-0.11.9/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 *.egg-info/
 .installed.cfg
 *.egg
 output_data
 output_files
 dash/
 dash-master/
+scrap/
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
```

### Comparing `finmarketpy-0.11.8/INSTALL.md` & `finmarketpy-0.11.9/INSTALL.md`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/LICENCE` & `finmarketpy-0.11.9/LICENCE`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/PKG-INFO` & `finmarketpy-0.11.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: finmarketpy
-Version: 0.11.8
+Version: 0.11.9
 Summary: finmarketpy is a Python based library for backtesting trading strategies
 Home-page: https://github.com/cuemacro/finmarketpy
 Author: Saeed Amen
 Author-email: saeed@cuemacro.com
 License: Apache 2.0
 Description: finmarketpy is a Python based library that enables you to analyze market data and also to backtest 
         trading strategies using a simple to use API, which has prebuilt templates for you to define backtest.
```

### Comparing `finmarketpy-0.11.8/PLANNED_FEATURES.md` & `finmarketpy-0.11.9/PLANNED_FEATURES.md`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/README.md` & `finmarketpy-0.11.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -113,16 +113,17 @@
 You can run some of the Jupyter notebooks in Binder interactively in your browser to play around with finmarketpy. It might take a few minutes for the 
 Binder instance to start. We are currently working on having more notebooks in Binder, so stay tuned!
 
 Note that you will need to get a Quandl
 API key to download market data to use some of these, and you can sign up for a free account at https://www.quandl.com.
 
 * [Backtesting an FX trend following strategy - backtest_example (Binder Link)](https://mybinder.org/v2/gh/cuemacro/finmarketpy/master?filepath=finmarketpy_examples/finmarketpy_notebooks/backtest_example.ipynb)
+* [Downloading market data examples - market_data_example (Binder Link)](https://mybinder.org/v2/gh/cuemacro/finmarketpy/master?filepath=finmarketpy_examples/finmarketpy_notebooks/market_data_example.ipynb)
 
-# Syncronizing your fork of finmarketpy with master
+# Synchronizing your fork of finmarketpy with master
 
 I found this [article useful](https://stackoverflow.com/questions/7244321/how-do-i-update-a-github-forked-repository) for 
 explaining how to update your fork to match the master changes.
 
 # Contributors
 
 Contributors are always welcome for finmarketpy, findatapy and chartpy. If you'd like to contribute, have a look at
@@ -149,28 +150,58 @@
 
 # finmarketpy examples
 
 In finmarketpy/examples you will find several examples, including some simple trading models
 
 # Release Notes
 
+* 0.11.9 - finmarketpy (01 Jun 2021)
 * 0.11.8 - finmarketpy (25 Jan 2021)
 * 0.11.7 - finmarketpy (20 Oct 2020)
 * 0.11.6 - finmarketpy (02 Oct 2020)
 * 0.11.5 - finmarketpy (24 Aug 2020)
 * 0.11.4 - finmarketpy (06 May 2020)
 * 0.11.3 - finmarketpy (04 Dec 2019)
 * 0.11.1 - finmarketpy (23 Oct 2019)
 * 0.11 - finmarketpy
 * First prerelease version 
 
 # Coding log
 
 # finmarketpy log
 
+* 30 May 2021
+  * Added S3 Jupyter notebook for use with findatapy
+* 21 May 2021
+  * Fix bug with plotting vol target charts when vol targeting is off
+* 12 May 2021
+  * Fixed bug when calculating benchmark return statistics in TradingModel with different start/finish date
+* 04 May 2021
+  * Revamped Jupyter notebook for downloading market data with findatapy
+* 28 Apr 2021
+  * Added signal multiplier parameter for charts
+* 21 Apr 2021
+  * Format changes to TradingModel charts
+* 15 Apr 2021
+  * Constant overrides now persist
+* 13 Apr 2021
+  * Replaced loc with iloc in TechIndicator to remove Pandas deprecated functionality
+* 08 Apr 2021
+  * Fixed EventStudy issue when start window is before time series
+* 21 Mar 2021
+  * Fixed issue with EventStudy
+  * Refactored TradingModel when constructing weights
+* 22 Feb 2021
+  * Fix bug when plotting IR of strategies
+* 16 Feb 2021
+  * Added total returns in example for options indices construction
+* 11 Feb 2021
+  * Refactored to use join from Calculations instead of pandas_outer_join
+  * Allowed backtesting by fields other than close
+  * Customize strike range for extracting FX vol surface
 * 22 Jan 2021
   * FX spot total returns now supports intraday data and added example
   * Fixed problem with Numba implementation of FX spot total returns
 * 17 Jan 2021
   * Fix vol surface examples to work with new FXVolSurface
 * 16 Jan 2021
   * Additional work on FXOptionPricer and total returns (FXOptionCurve)
```

### Comparing `finmarketpy-0.11.8/binder/Dockerfile` & `finmarketpy-0.11.9/binder/Dockerfile`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy/backtest/backtestcomparison.py` & `finmarketpy-0.11.9/finmarketpy/backtest/backtestcomparison.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy/backtest/backtestengine.py` & `finmarketpy-0.11.9/finmarketpy/backtest/backtestengine.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,49 +8,49 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and limitations under the License.
 #
 
-import numpy
+import numpy as np
+import pandas as pd
 
 from finmarketpy.util.marketconstants import MarketConstants
 
 from findatapy.util import SwimPool
 from findatapy.util import LoggerManager
 
 import pickle
 #import zlib
 #import lz4framed    # conda install -c conda-forge py-lz4framed
 
-# make blosc optional (only when trying to run backtests in parallel)
+# Make blosc optional (only when trying to run backtests in parallel)
 try:
     import blosc
 except:
     pass
 
 import pickle
 
 market_constants = MarketConstants()
 
-
 class Backtest(object):
     """Conducts backtest for strategies trading assets. Assumes we have an input of total returns. Reports historical return statistics
     and returns time series.
 
     """
 
     def __init__(self):
         self._pnl = None
         self._portfolio = None
         return
 
     def calculate_diagnostic_trading_PnL(self, asset_a_df, signal_df, further_df=[], further_df_labels=[]):
-        """Calculates P&L table which can be used for debugging purposes,
+        """Calculates P&L table which can be used for debugging purposes.
 
         The table is populated with asset, signal and further dataframes provided by the user, can be used to check signalling methodology.
         It does not apply parameters such as transaction costs, vol adjusment and so on.
 
         Parameters
         ----------
         asset_a_df : DataFrame
@@ -73,15 +73,15 @@
         calculations = Calculations()
         asset_rets_df = calculations.calculate_returns(asset_a_df)
         strategy_rets = calculations.calculate_signal_returns(signal_df, asset_rets_df)
 
         reset_points = ((signal_df - signal_df.shift(1)).abs())
 
         asset_a_df_entry = asset_a_df.copy(deep=True)
-        asset_a_df_entry[reset_points == 0] = numpy.nan
+        asset_a_df_entry[reset_points == 0] = np.nan
         asset_a_df_entry = asset_a_df_entry.ffill()
 
         asset_a_df_entry.columns = [x + '_entry' for x in asset_a_df_entry.columns]
         asset_rets_df.columns = [x + '_asset_rets' for x in asset_rets_df.columns]
         strategy_rets.columns = [x + '_strat_rets' for x in strategy_rets.columns]
         signal_df.columns = [x + '_final_signal' for x in signal_df.columns]
 
@@ -89,15 +89,15 @@
             further_df[i].columns = [x + '_' + further_df_labels[i] for x in further_df[i].columns]
 
         flatten_df = [asset_a_df, asset_a_df_entry, asset_rets_df, strategy_rets, signal_df]
 
         for f in further_df:
             flatten_df.append(f)
 
-        return calculations.pandas_outer_join(flatten_df)
+        return calculations.join(flatten_df, how='outer')
 
     def calculate_trading_PnL(self, br, asset_a_df, signal_df, contract_value_df, run_in_parallel):
         """Calculates P&L of a trading strategy and statistics to be retrieved later
 
         Calculates the P&L for each asset/signal combination and also for the finally strategy applying appropriate
         weighting in the portfolio, depending on predefined parameters, for example:
             static weighting for each asset
@@ -105,34 +105,34 @@
             static weighting for each asset + vol weighting for each asset + vol weighting for the portfolio
 
         Parameters
         ----------
         br : BacktestRequest
             Parameters for the backtest specifying start date, finish data, transaction costs etc.
 
-        asset_a_df : pandas.DataFrame
+        asset_a_df : pd.DataFrame
             Asset prices to be traded
 
-        signal_df : pandas.DataFrame
+        signal_df : pd.DataFrame
             Signals for the trading strategy
 
-        contract_value_df : pandas.DataFrame
+        contract_value_df : pd.DataFrame
             Daily size of contracts
         """
 
         calculations = Calculations()
         risk_engine = RiskEngine()
 
-        # # do an outer join first, so can fill out signal and fill it down
+        # # Do an outer join first, so can fill out signal and fill it down
         # # this captures the case where the signal changes on an asset holiday
         # # it will just get delayed till the next tradable day when we do this
         # asset_df_2, signal_df_2 = asset_a_df.align(signal_df, join='outer', axis='index')
         # signal_df = signal_df_2.fillna(method='ffill')
         #
-        # # now make sure the dates of both traded asset and signal are aligned properly
+        # # Now make sure the dates of both traded asset and signal are aligned properly
         # # and use as reference only those days where we have asset information
         # asset_df, signal_df = asset_a_df.align(signal_df, join='left', axis = 'index')
 
         logger = LoggerManager().getLogger(__name__)
 
         logger.info("Calculating trading P&L...")
 
@@ -140,19 +140,19 @@
         asset_df, signal_df = calculations.join_left_fill_right(asset_a_df, signal_df)
 
         if (contract_value_df is not None):
             asset_df, contract_value_df = asset_df.align(contract_value_df, join='left', axis='index')
             contract_value_df = contract_value_df.fillna(
                 method='ffill')  # fill down asset holidays (we won't trade on these days)
 
-        # non-trading days of the assets (this may of course vary between the assets we are trading
+        # Non-trading days of the assets (this may of course vary between the assets we are trading
         # if they are from different asset classes)
-        non_trading_days = numpy.isnan(asset_df.values)
+        non_trading_days = np.isnan(asset_df.values)
 
-        # only allow signals to change on the days when we can trade assets
+        # Only allow signals to change on the days when we can trade assets
         signal_df = signal_df.mask(non_trading_days)  # fill asset holidays with NaN signals
         signal_df = signal_df.fillna(method='ffill')  # fill these down
 
         tc = br.spot_tc_bp
 
         signal_cols = signal_df.columns.values
         asset_df_cols = asset_df.columns.values
@@ -161,20 +161,20 @@
 
         for i in range(0, len(asset_df_cols)):
             pnl_cols.append(asset_df_cols[i] + " / " + signal_cols[i])
 
         asset_df = asset_df.fillna(method='ffill')  # fill down asset holidays (we won't trade on these days)
         returns_df = calculations.calculate_returns(asset_df)
 
-        # apply a stop loss/take profit to every trade if this has been specified
+        # Apply a stop loss/take profit to every trade if this has been specified
         # do this before we start to do vol weighting etc.
         if br.take_profit is not None and br.stop_loss is not None:
             returns_df = calculations.calculate_returns(asset_df)
 
-            # makes assumption that signal column order matches that of returns
+            # Makes assumption that signal column order matches that of returns
             temp_strategy_rets_df = calculations.calculate_signal_returns_as_matrix(signal_df, returns_df)
 
             trade_rets_df = calculations.calculate_cum_rets_trades(signal_df, temp_strategy_rets_df)
 
             # pre_signal_df = signal_df.copy()
 
             signal_df = calculations.calculate_risk_stop_signals(signal_df, trade_rets_df, br.stop_loss, br.take_profit)
@@ -192,238 +192,166 @@
             #     temp_strategy_rets_df.columns = [x + '_strategy_rets' for x in temp_strategy_rets_df.columns]
             #     signal_df_copy.columns = [x + '_final_signal' for x in signal_df_copy.columns]
             #     trade_rets_df_copy.columns = [x + '_cum_trade' for x in trade_rets_df_copy.columns]
             #
             #     to_plot = _calculations.pandas_outer_join([asset_df_copy, pre_signal_df, signal_df_copy, trade_rets_df_copy, temp_strategy_rets_df])
             #     to_plot.to_csv('test.csv')
 
-        # do we have a vol target for individual signals?
-        if br.signal_vol_adjust is True:
-            leverage_df = risk_engine.calculate_leverage_factor(returns_df, br.signal_vol_target,
-                                                                br.signal_vol_max_leverage,
-                                                                br.signal_vol_periods, br.signal_vol_obs_in_year,
-                                                                br.signal_vol_rebalance_freq,
-                                                                br.signal_vol_resample_freq,
-                                                                br.signal_vol_resample_type,
-                                                                period_shift=br.signal_vol_period_shift)
-
-            signal_df = pandas.DataFrame(
-                signal_df.values * leverage_df.values, index=signal_df.index, columns=signal_df.columns)
-
-            self._individual_leverage = leverage_df  # contains leverage of individual signal (before portfolio vol target)
-
-        _pnl = calculations.calculate_signal_returns_with_tc_matrix(signal_df, returns_df, tc=tc)
-        _pnl.columns = pnl_cols
-
-        adjusted_weights_matrix = None
-
-        # portfolio is average of the underlying signals: should we sum them or average them or use another
-        # weighting scheme?
-        if br.portfolio_combination is not None:
-            if br.portfolio_combination == 'sum' and br.portfolio_combination_weights is None:
-                portfolio = pandas.DataFrame(data=_pnl.sum(axis=1), index=_pnl.index, columns=['Portfolio'])
-            elif br.portfolio_combination == 'mean' and br.portfolio_combination_weights is None:
-                portfolio = pandas.DataFrame(data=_pnl.mean(axis=1), index=_pnl.index, columns=['Portfolio'])
-
-                adjusted_weights_matrix = self.create_portfolio_weights(br, _pnl, method='mean')
-            elif 'weighted' in br.portfolio_combination and isinstance(br.portfolio_combination_weights, dict):
-
-                # get the weights for each asset
-                adjusted_weights_matrix = self.create_portfolio_weights(br, _pnl, method=br.portfolio_combination)
-
-                portfolio = pandas.DataFrame(data=(_pnl.values * adjusted_weights_matrix), index=_pnl.index)
-                is_all_na = pandas.isnull(portfolio).all(axis=1)
-                portfolio = pandas.DataFrame(portfolio.sum(axis=1), columns=['Portfolio'])
-
-                # overwrite days when every asset PnL was null is NaN with nan
-                portfolio[is_all_na] = numpy.nan
+        if br.portfolio_weight_construction is None:
+            pwc = PortfolioWeightConstruction(br=br)
         else:
-            portfolio = pandas.DataFrame(data=_pnl.mean(axis=1), index=_pnl.index, columns=['Portfolio'])
-
-            adjusted_weights_matrix = self.create_portfolio_weights(br, _pnl, method='mean')
-
-        portfolio_leverage_df = pandas.DataFrame(data=numpy.ones(len(_pnl.index)), index=_pnl.index,
-                                                 columns=['Portfolio'])
-
-        # should we apply vol target on a portfolio level basis?
-        if br.portfolio_vol_adjust is True:
-            # calculate portfolio leverage
-            portfolio_leverage_df = risk_engine.calculate_leverage_factor(portfolio,
-                                                                          br.portfolio_vol_target,
-                                                                          br.portfolio_vol_max_leverage,
-                                                                          br.portfolio_vol_periods,
-                                                                          br.portfolio_vol_obs_in_year,
-                                                                          br.portfolio_vol_rebalance_freq,
-                                                                          br.portfolio_vol_resample_freq,
-                                                                          br.portfolio_vol_resample_type,
-                                                                          period_shift=br.portfolio_vol_period_shift)
+            pwc = br.portfolio_weight_construction
 
-            # portfolio, portfolio_leverage_df = risk_engine.calculate_vol_adjusted_returns(portfolio, br = br)
-
-        # multiply portfolio leverage * individual signals to get final position signals
-        length_cols = len(signal_df.columns)
-        leverage_matrix = numpy.transpose(
-            numpy.repeat(portfolio_leverage_df.values.flatten()[numpy.newaxis, :], length_cols, 0))
-
-        # final portfolio signals (including signal & portfolio leverage)
-        portfolio_signal = pandas.DataFrame(
-            data=numpy.multiply(leverage_matrix, signal_df.values),
-            index=signal_df.index, columns=signal_df.columns)
-
-        # later when we plot the portfolio components, we do that without weighting the individual components
-        portfolio_signal_before_weighting = portfolio_signal.copy()
-
-        if br.portfolio_combination is not None:
-            if 'sum' in br.portfolio_combination:
-                pass
-            elif br.portfolio_combination == 'mean' \
-                    or (br.portfolio_combination == 'weighted' and isinstance(br.portfolio_combination_weights, dict)):
-                portfolio_signal = pandas.DataFrame(data=(portfolio_signal.values * adjusted_weights_matrix),
-                                                    index=portfolio_signal.index,
-                                                    columns=portfolio_signal.columns)
-        else:
-            portfolio_signal = pandas.DataFrame(data=(portfolio_signal.values * adjusted_weights_matrix),
-                                                index=portfolio_signal.index,
-                                                columns=portfolio_signal.columns)
+        # Adjust signal weights and portfolio weights (eg. using various rules, like vol targeting)
+        # and also aggregate final portfolio weights
+        portfolio_signal_before_weighting, portfolio_signal, portfolio_leverage_df, portfolio, individual_leverage_df, pnl = \
+            pwc.optimize_portfolio_weights(returns_df, signal_df, pnl_cols)
 
         portfolio_total_longs, portfolio_total_shorts, portfolio_net_exposure, portfolio_total_exposure \
             = self.calculate_exposures(portfolio_signal)
 
-        # apply position limits?
+        # Apply position limits?
         position_clip_adjustment = risk_engine.calculate_position_clip_adjustment \
             (portfolio_net_exposure, portfolio_total_exposure, br)
 
-        # if we have any position clip adjustment, for example related to max position sizes
+        # If we have any position clip adjustment, for example related to max position sizes
         if position_clip_adjustment is not None:
-            position_clip_adjustment_matrix = numpy.transpose(
-                numpy.repeat(position_clip_adjustment.values.flatten()[numpy.newaxis, :], length_cols, 0))
+            length_cols = len(signal_df.columns)
+
+            position_clip_adjustment_matrix = np.transpose(
+                np.repeat(position_clip_adjustment.values.flatten()[np.newaxis, :], length_cols, 0))
 
-            # recalculate portfolio signals after adjustment (for individual components - without
+            # Recalculate portfolio signals after adjustment (for individual components - without
             # weighting each signal separately)
-            portfolio_signal_before_weighting = pandas.DataFrame(
+            portfolio_signal_before_weighting = pd.DataFrame(
                 data=(portfolio_signal_before_weighting.values * position_clip_adjustment_matrix),
                 index=portfolio_signal_before_weighting.index,
                 columns=portfolio_signal_before_weighting.columns)
 
-            # recalculate portfolio signal after adjustment (for portfolio level positions)
-            portfolio_signal = pandas.DataFrame(
+            # Recalculate portfolio signal after adjustment (for portfolio level positions)
+            portfolio_signal = pd.DataFrame(
                 data=(portfolio_signal.values * position_clip_adjustment_matrix),
                 index=portfolio_signal.index,
                 columns=portfolio_signal.columns)
 
-            # recalculate portfolio leverage with position constraint (multiply vectors elementwise)
-            portfolio_leverage_df = pandas.DataFrame(
+            # Recalculate portfolio leverage with position constraint (multiply vectors elementwise)
+            portfolio_leverage_df = pd.DataFrame(
                 data=(portfolio_leverage_df.values * position_clip_adjustment.values),
                 index=portfolio_leverage_df.index,
                 columns=portfolio_leverage_df.columns)
 
-            # recalculate total long, short, net and absolute exposures of the whole portfolio after the position
+            # Recalculate total long, short, net and absolute exposures of the whole portfolio after the position
             # clip adjustment
             portfolio_total_longs, portfolio_total_shorts, portfolio_net_exposure, portfolio_total_exposure \
                 = self.calculate_exposures(portfolio_signal)
 
-        # calculate final portfolio returns with the amended portfolio leverage (by default just 1s)
+        # Calculate final portfolio returns with the amended portfolio leverage (by default just 1s)
         portfolio = calculations.calculate_signal_returns_with_tc_matrix(portfolio_leverage_df, portfolio, tc=tc)
 
-        # assign all the property variables
-        self._signal = signal_df  # individual signals (before portfolio leverage)
-        self._portfolio_signal = portfolio_signal  # individual signals (AFTER portfolio leverage/constraints)
-        self._portfolio_leverage = portfolio_leverage_df  # leverage on portfolio
+        # Assign all the property variables
+        # Trim them if we have asked for a different plot start/finish
+        self._signal = self._filter_by_plot_start_finish_date(signal_df, br)  # individual signals (before portfolio leverage)
+        self._portfolio_signal = self._filter_by_plot_start_finish_date(portfolio_signal, br)  # individual signals (AFTER portfolio leverage/constraints)
+        self._portfolio_leverage = self._filter_by_plot_start_finish_date(portfolio_leverage_df, br)  # leverage on portfolio
 
-        self._portfolio = portfolio
+        self._portfolio = self._filter_by_plot_start_finish_date(portfolio, br)
 
-        # calculate each period of trades
+        # Calculate each period of trades
         self._portfolio_trade = self._portfolio_signal - self._portfolio_signal.shift(1)
 
-        # expressing trades/positions in terms of notionals
+        # Expressing trades/positions in terms of notionals
         self._portfolio_signal_notional = None
         self._portfolio_signal_trade_notional = None
 
-        # expressing trades/positions in terms of contracts (useful for futures)
+        # Expressing trades/positions in terms of contracts (useful for futures)
         self._portfolio_signal_contracts = None
         self._portfolio_signal_trade_contracts = None
 
-        self._portfolio_total_longs = portfolio_total_longs
-        self._portfolio_total_shorts = portfolio_total_shorts
-        self._portfolio_net_exposure = portfolio_net_exposure
-        self._portfolio_total_exposure = portfolio_total_exposure
+        self._portfolio_total_longs = self._filter_by_plot_start_finish_date(portfolio_total_longs, br)
+        self._portfolio_total_shorts = self._filter_by_plot_start_finish_date(portfolio_total_shorts, br)
+        self._portfolio_net_exposure = self._filter_by_plot_start_finish_date(portfolio_net_exposure, br)
+        self._portfolio_total_exposure = self._filter_by_plot_start_finish_date(portfolio_total_exposure, br)
 
         self._portfolio_total_longs_notional = None
         self._portfolio_total_shorts_notional = None
         self._portfolio_net_exposure_notional = None
         self._portfolio_total_exposure_notional = None
         self._portfolio_signal_trade_notional_sizes = None
 
-        # also create other measures of portfolio
-        # portfolio & trades in terms of a predefined notional (in USD)
-        # portfolio & trades in terms of contract sizes (particularly useful for futures)
+        # Individual signals P&L (before portfolio volatility targeting, position limits etc)
+        self._pnl = pnl
+
+        self._individual_leverage = self._filter_by_plot_start_finish_date(individual_leverage_df, br)
+
+        # P&L components of individual assets after all the portfolio level risk signals and position limits have been applied
+        self._components_pnl = self._filter_by_plot_start_finish_date(calculations.calculate_signal_returns_with_tc_matrix(portfolio_signal_before_weighting,
+                                                                                    returns_df, tc=tc), br)
+        self._components_pnl.columns = pnl_cols
+
+        # TODO FIX very slow - hence only calculate on demand
+        # _pnl_trades = _calculations.calculate_individual_trade_gains(signal_df, _pnl)
+        self._pnl_trades = None
+        self._components_pnl_trades = None
+
+        self._trade_no = None
+        self._portfolio_trade_no = None
+
+        self._portfolio.columns = ['Port']
+
+        self._pnl_ret_stats = RetStats(self._pnl, br.ann_factor, br.resample_ann_factor)
+        self._components_pnl_ret_stats = RetStats(self._components_pnl, br.ann_factor, br.resample_ann_factor)
+        self._portfolio_ret_stats = RetStats(self._portfolio, br.ann_factor, br.resample_ann_factor)
+
+        # Also create other measures of portfolio
+        # * portfolio & trades in terms of a predefined notional (in USD)
+        # * portfolio & trades in terms of contract sizes (particularly useful for futures)
         if br.portfolio_notional_size is not None:
-            # express positions in terms of the notional size specified
+
+            # Express positions in terms of the notional size specified
             self._portfolio_signal_notional = self._portfolio_signal * br.portfolio_notional_size
-            self._portfolio_signal_trade_notional = self._portfolio_signal_notional - self._portfolio_signal_notional.shift(
-                1)
+            self._portfolio_signal_trade_notional = self._portfolio_signal_notional \
+                                                    - self._portfolio_signal_notional.shift(1)
 
-            df_trades_sizes = pandas.DataFrame()
+            df_trades_sizes = pd.DataFrame()
 
             rounded_portfolio_signal_trade_notional = self._portfolio_signal_trade_notional.round(2)
 
             for k in rounded_portfolio_signal_trade_notional.columns:
-                df_trades_sizes[k] = pandas.value_counts(rounded_portfolio_signal_trade_notional[k], sort=True)
+                df_trades_sizes[k] = pd.value_counts(rounded_portfolio_signal_trade_notional[k], sort=True)
 
             df_trades_sizes = df_trades_sizes[df_trades_sizes.index != 0]
 
             self._portfolio_signal_trade_notional_sizes = df_trades_sizes
 
             self._portfolio_total_longs_notional = portfolio_total_longs * br.portfolio_notional_size
             self._portfolio_total_shorts_notional = portfolio_total_shorts * br.portfolio_notional_size
             self._portfolio_net_exposure_notional = portfolio_net_exposure * br.portfolio_notional_size
             self._portfolio_total_exposure_notional = portfolio_total_exposure * br.portfolio_notional_size
 
-            # get the positions in terms of the contract sizes
+            # Get the positions in terms of the contract sizes
             notional_copy = self._portfolio_signal_notional.copy(deep=True)
             notional_copy_cols = [x.split('.')[0] for x in notional_copy.columns]
             notional_copy_cols = [x + '.contract-value' for x in notional_copy_cols]
 
             notional_copy.columns = notional_copy_cols
 
-            # can only give contract sizes if these are defined
+            # Can only give contract sizes if these are defined
             if contract_value_df is not None:
                 contract_value_df = contract_value_df[notional_copy_cols]
                 notional_df, contract_value_df = notional_copy.align(contract_value_df, join='left', axis='index')
 
-                # careful make sure orders of magnitude are same for the notional and the contract value
+                # Careful make sure orders of magnitude are same for the notional and the contract value
                 self._portfolio_signal_contracts = notional_df / contract_value_df
                 self._portfolio_signal_contracts.columns = self._portfolio_signal_notional.columns
-                self._portfolio_signal_trade_contracts = self._portfolio_signal_contracts - self._portfolio_signal_contracts.shift(
-                    1)
-
-        self._pnl = _pnl  # individual signals P&L (before portfolio volatility targeting, position limits etc)
-
-        # _pnl_components of individual assets after all the portfolio level risk signals and position limits have been applied
-        self._components_pnl = calculations.calculate_signal_returns_with_tc_matrix(portfolio_signal_before_weighting,
-                                                                                    returns_df, tc=tc)
-        self._components_pnl.columns = pnl_cols
-
-        # TODO FIX very slow - hence only calculate on demand
-        # _pnl_trades = _calculations.calculate_individual_trade_gains(signal_df, _pnl)
-        self._pnl_trades = None
-        self._components_pnl_trades = None
-
-        self._trade_no = None
-        self._portfolio_trade_no = None
-
-        self._portfolio.columns = ['Port']
-
-        self._pnl_ret_stats = RetStats(self._pnl, br.ann_factor, br.resample_ann_factor)
-        self._components_pnl_ret_stats = RetStats(self._components_pnl, br.ann_factor, br.resample_ann_factor)
-        self._portfolio_ret_stats = RetStats(self._portfolio, br.ann_factor, br.resample_ann_factor)
+                self._portfolio_signal_trade_contracts = self._portfolio_signal_contracts \
+                                                         - self._portfolio_signal_contracts.shift(1)
 
         # TODO parallel version still work in progress!
 
-        logger.info("Cumulative index _calculations")
+        logger.info("Cumulative index calculations")
 
         if False: # market_constants.backtest_thread_no[market_constants.generic_plat] > 1 and run_in_parallel:
             swim_pool = SwimPool(multiprocessing_library=market_constants.multiprocessing_library)
 
             pool = swim_pool.create_pool(thread_technique=market_constants.backtest_thread_technique,
                                          thread_no=market_constants.backtest_thread_no[market_constants.generic_plat])
 
@@ -470,138 +398,104 @@
                 self._pnl_cum = calculations.create_add_index(self._pnl)
 
                 # Calculate individual signals cumulative P&L after signal leverage AND after portfolio level constraints
                 self._components_pnl_cum = calculations.create_add_index(self._components_pnl)
 
                 self._portfolio_cum = calculations.create_add_index(self._portfolio)  # portfolio cumulative P&L
 
-        logger.info("Completed cumulative index _calculations")
+        logger.info("Completed cumulative index calculations")
 
         self._pnl_cum.columns = pnl_cols
         self._components_pnl_cum.columns = pnl_cols
         self._portfolio_cum.columns = ['Port']
 
+    def _filter_by_plot_start_finish_date(self, df, br):
+
+        if br.plot_start is None and br.plot_finish is None:
+            return df
+        elif df is None:
+            return None
+        else:
+            filter = Filter()
+            plot_start = br.start_date;
+            plot_finish = br.finish_date
+
+            if br.plot_start is not None:
+                plot_start = br.plot_start
+
+            if br.plot_finish is not None:
+                plot_finish = br.plot_finish
+
+            return filter.filter_time_series_by_date(plot_start, plot_finish, df)
+
     def calculate_exposures(self, portfolio_signal):
         """Calculates time series for the total longs, short, net and absolute exposure on an aggregated portfolio basis.
 
         Parameters
         ----------
         portfolio_signal : DataFrame
             Signals for each asset in the portfolio after all weighting, portfolio & signal level volatility adjustments
 
         Returns
         -------
         DataFrame (list)
 
         """
-        # calculate total portfolio longs/total portfolio shorts/total portfolio exposure
-        portfolio_total_longs = pandas.DataFrame(portfolio_signal[portfolio_signal > 0].sum(axis=1))
-        portfolio_total_shorts = pandas.DataFrame(portfolio_signal[portfolio_signal < 0].sum(axis=1))
+
+        # Calculate total portfolio longs/total portfolio shorts/total portfolio exposure
+        portfolio_total_longs = pd.DataFrame(portfolio_signal[portfolio_signal > 0].sum(axis=1))
+        portfolio_total_shorts = pd.DataFrame(portfolio_signal[portfolio_signal < 0].sum(axis=1))
 
         portfolio_total_longs.columns = ['Total Longs']
         portfolio_total_shorts.columns = ['Total Shorts']
 
         # NOTE: careful usage of signs (portfolio_total_shorts are NEGATIVE)
-        portfolio_net_exposure = pandas.DataFrame(
+        portfolio_net_exposure = pd.DataFrame(
             index=portfolio_signal.index, columns=['Net Exposure'],
             data=portfolio_total_longs.values + portfolio_total_shorts.values)
 
-        portfolio_total_exposure = pandas.DataFrame(
+        portfolio_total_exposure = pd.DataFrame(
             index=portfolio_signal.index, columns=['Total Exposure'],
             data=portfolio_total_longs.values - portfolio_total_shorts.values)
 
         return portfolio_total_longs, portfolio_total_shorts, portfolio_net_exposure, portfolio_total_exposure
 
-    def create_portfolio_weights(self, br, _pnl, method='mean'):
-        """Calculates P&L of a trading strategy and statistics to be retrieved later
-
-        Parameters
-        ----------
-        br : BacktestRequest
-            Parameters for the backtest specifying start date, finish data, transaction costs etc.
-
-        _pnl : pandas.DataFrame
-            Contains the daily P&L for the portfolio
-
-        method : String
-            'mean' - assumes equal weighting for each signal
-            'weighted' - can use predefined user weights (eg. if we assign weighting of 1, 1, 0.5, for three signals
-            the third signal will have a weighting of half versus the others)
-        
-        weights : dict
-            Portfolio weights
-
-        Returns
-        -------
-        pandas.DataFrame
-            Contains the portfolio weights
-        """
-        if method == 'mean':
-            weights_vector = numpy.ones(len(_pnl.columns))
-        elif method == 'weighted' or 'weighted-sum':
-            # get the weights for each asset
-            weights_vector = numpy.array([float(br.portfolio_combination_weights[col]) for col in _pnl.columns])
-
-        # repeat this down for every day
-        weights_matrix = numpy.repeat(weights_vector[numpy.newaxis, :], len(_pnl.index), 0)
-
-        # where we don't have old price data, make the weights 0 there
-        ind = numpy.isnan(_pnl.values)
-        weights_matrix[ind] = 0
-
-        if method != 'weighted-sum':
-            # the total weights will vary, as historically might not have all the assets trading
-            total_weights = numpy.sum(weights_matrix, axis=1)
-
-            # replicate across columns
-            total_weights = numpy.transpose(numpy.repeat(total_weights[numpy.newaxis, :], len(_pnl.columns), 0))
-
-            # to avoid divide by zero
-            total_weights[total_weights == 0.0] = 1.0
-
-            adjusted_weights_matrix = weights_matrix / total_weights
-            adjusted_weights_matrix[ind] = numpy.nan
-
-            return adjusted_weights_matrix
-
-        return weights_matrix
-
     def backtest_output(self):
         return
 
     ### Get PnL of individual assets before portfolio constraints
     def pnl(self):
         """Gets P&L returns of all the individual sub_components of the model (before any portfolio level leverage is applied)
 
         Returns
         -------
-        pandas.Dataframe
+        pd.Dataframe
         """
         return self._pnl
 
     def trade_no(self):
         """Gets number of trades for each signal in the backtest (before
 
         Returns
         -------
-        pandas.Dataframe
+        pd.Dataframe
         """
 
         if self._trade_no is None:
             calculations = Calculations()
             self._trade_no = calculations.calculate_trade_no(self._signal)
 
         return self._trade_no
 
     def pnl_trades(self):
         """Gets P&L of each individual trade per signal
 
         Returns
         -------
-        pandas.Dataframe
+        pd.Dataframe
         """
 
         if self._pnl_trades is None:
             calculations = Calculations()
             self._pnl_trades = calculations.calculate_individual_trade_gains(self._signal, self._pnl)
 
         return self._pnl_trades
@@ -626,35 +520,35 @@
         return self._pnl_ret_stats
 
     def pnl_cum(self):
         """Gets P&L as a cumulative time series of individual assets
 
         Returns
         -------
-        pandas.DataFrame
+        pd.DataFrame
         """
 
         return self._pnl_cum
 
     ### Get PnL of individual assets AFTER portfolio constraints
     def components_pnl(self):
         """Gets P&L returns of all the individual subcomponents of the model (after portfolio level leverage is applied)
 
         Returns
         -------
-        pandas.Dataframe
+        pd.Dataframe
         """
         return self._components_pnl
 
     def components_pnl_trades(self):
         """Gets P&L of each individual trade per signal
 
         Returns
         -------
-        pandas.Dataframe
+        pd.Dataframe
         """
 
         if self._components_pnl_trades is None:
             calculations = Calculations()
             self._components_pnl_trades = calculations.calculate_individual_trade_gains(self._signal,
                                                                                         self._components_pnl)
 
@@ -680,47 +574,47 @@
         return self._components_pnl_ret_stats
 
     def components_pnl_cum(self):
         """Gets P&L as a cumulative time series of individual assets (after portfolio level leverage adjustments)
 
         Returns
         -------
-        pandas.DataFrame
+        pd.DataFrame
         """
 
         return self._components_pnl_cum
 
     ### Get PnL of the final portfolio
 
     def portfolio_cum(self):
         """Gets P&L as a cumulative time series of portfolio
 
         Returns
         -------
-        pandas.DataFrame
+        pd.DataFrame
         """
 
         return self._portfolio_cum
 
     def portfolio_pnl(self):
         """Gets portfolio returns in raw form (ie. not indexed into cumulative form)
 
         Returns
         -------
-        pandas.DataFrame
+        pd.DataFrame
         """
 
         return self._portfolio
 
     def portfolio_pnl_desc(self):
         """Gets P&L return statistics of portfolio as string
 
         Returns
         -------
-        pandas.DataFrame
+        pd.DataFrame
         """
 
         return self._portfolio_ret_stats.summary()
 
     def portfolio_pnl_ret_stats(self):
         """Gets P&L return statistics of portfolio as class to be queried
 
@@ -732,35 +626,35 @@
         return self._portfolio_ret_stats
 
     def individual_leverage(self):
         """Gets leverage for each asset historically
 
         Returns
         -------
-        pandas.DataFrame
+        pd.DataFrame
         """
 
         return self._individual_leverage
 
     def portfolio_leverage(self):
         """Gets the leverage for the portfolio
 
         Returns
         -------
-        pandas.DataFrame
+        pd.DataFrame
         """
 
         return self._portfolio_leverage
 
     def portfolio_trade_no(self):
         """Gets number of trades for each signal in the backtest (after both signal and portfolio level vol adjustment)
 
         Returns
         -------
-        pandas.Dataframe
+        pd.Dataframe
         """
 
         if self._portfolio_trade_no is None:
             calculations = Calculations()
             self._portfolio_trade_no = calculations.calculate_trade_no(self._portfolio_signal)
 
         return self._portfolio_trade_no
@@ -925,59 +819,58 @@
         return self._portfolio_signal_trade_contracts
 
     def signal(self):
         """Gets signal for each asset (with individual leverage, but excluding portfolio leverage constraints) for each asset
 
         Returns
         -------
-        pandas.DataFrame
+        pd.DataFrame
         """
 
         return self._signal
 
 
 ########################################################################################################################
 
 import abc
-import pandas
 import datetime
 import copy
 
 from chartpy import Chart, Style, ChartConstants
 
 from finmarketpy.economics import TechParams
 from findatapy.timeseries import Calculations, RetStats, Filter
 
-
 class TradingModel(object):
     """Abstract class which wraps around Backtest, providing convenient functions for analaysis. Implement your own
     subclasses of this for your own strategy. See tradingmodelfxtrend_example.py for a simple implementation of a
     FX trend following strategy.
-
     """
 
     #### Default parameters for outputting of results from trading model
     SAVE_FIGURES = True
     SHOW_CHARTS = True
     SHOW_TITLES = True
 
     DEFAULT_PLOT_ENGINE = ChartConstants().chartfactory_default_engine
     SCALE_FACTOR = ChartConstants().chartfactory_scale_factor
+    WIDTH = ChartConstants().chartfactory_width
+    HEIGHT = ChartConstants().chartfactory_height
     CHART_SOURCE = ChartConstants().chartfactory_source
     CHART_STYLE = Style()
 
     DUMP_CSV = ''
     DUMP_PATH = datetime.date.today().strftime("%Y%m%d") + ' '
 
     # logger = LoggerManager().getLogger(__name__)
 
     def __init__(self):
         pass
 
-    # to be implemented by every trading strategy
+    # To be implemented by every trading strategy
     @abc.abstractmethod
     def load_parameters(self, br=None):
         """Fills parameters for the backtest, such as start-end dates, transaction costs etc. To
         be implemented by subclass. Can overwrite it with our own BacktestRequest.
         """
         return
 
@@ -990,18 +883,18 @@
 
     @abc.abstractmethod
     def construct_signal(self, spot_df, spot_df2, tech_params, br, run_in_parallel=False):
         """Constructs signal from pre-loaded time series
 
         Parameters
         ----------
-        spot_df : pandas.DataFrame
+        spot_df : pd.DataFrame
             Market time series for generating signals
 
-        spot_df2 : pandas.DataFrame
+        spot_df2 : pd.DataFrame
             Market time series for generated signals (can be of different frequency)
 
         tech_params : TechParams
             Parameters for generating signals
 
         run_in_parallel : bool
             Allow signal calculation in parallel
@@ -1034,21 +927,22 @@
         It gets backtesting parameters from fill_backtest_request (although these can be overwritten
         and then market data from fill_assets
 
         Parameters
         ----------
         br : BacktestRequest
             Parameters which define the backtest (for example start date, end date, transaction costs etc.
-
         """
 
         logger = LoggerManager().getLogger(__name__)
 
         # Get the parameters for backtesting
-        if hasattr(self, 'br'):
+        if br is not None:
+            pass
+        elif hasattr(self, 'br'):
             br = self.br
         elif br is None:
             br = self.load_parameters()
 
         # Get market data for backtest (not every load_assets model will take br)
         try:
             market_data = self.load_assets(br=br)
@@ -1068,25 +962,25 @@
             contract_value_df = market_data[4]
 
         if hasattr(br, 'tech_params'):
             tech_params = br.tech_params
         else:
             tech_params = TechParams()
 
-        cum_results = pandas.DataFrame(index=asset_df.index)
-        port_leverage = pandas.DataFrame(index=asset_df.index)
+        cum_results = pd.DataFrame(index=asset_df.index)
+        port_leverage = pd.DataFrame(index=asset_df.index)
 
         from collections import OrderedDict
         ret_stats_results = OrderedDict()
 
         bask_results = {}
 
         bask_keys = basket_dict.keys()
 
-        # each portfolio key calculate returns - can put parts of the portfolio in the key
+        # Each portfolio key calculate returns - can put parts of the portfolio in the key
         if market_constants.backtest_thread_no[market_constants.generic_plat] > 1 and run_in_parallel:
             swim_pool = SwimPool(multiprocessing_library=market_constants.multiprocessing_library)
 
             pool = swim_pool.create_pool(thread_technique=market_constants.backtest_thread_technique,
                                          thread_no=market_constants.backtest_thread_no[market_constants.generic_plat])
 
             mult_results = []
@@ -1097,30 +991,30 @@
             # calculate sub substrategies in sub-processes
             # TODO cut up in time chunks
             for key in bask_keys:
 
                 if key != self.FINAL_STRATEGY:
                     logger.info("Calculating (parallel) " + key)
 
-                    asset_cut_df = asset_df[[x + '.close' for x in basket_dict[key]]]
-                    spot_cut_df = spot_df[[x + '.close' for x in basket_dict[key]]]
+                    asset_cut_df = asset_df[[x + '.' + br.trading_field for x in basket_dict[key]]]
+                    spot_cut_df = spot_df[[x + '.' + br.trading_field for x in basket_dict[key]]]
 
                     mult_results.append(
                         pool.apply_async(self.construct_individual_strategy, args=(br, spot_cut_df, spot_df2, asset_cut_df,
                                                                                    tech_params, key, contract_value_df,
                                                                                    False, True,))
                     )
 
-                    # calculate final strategy separately in my main process (so don't have issues with pickling back large output)
+                    # Calculate final strategy separately in my main process (so don't have issues with pickling back large output)
 
             logger.info("Calculating final strategy " + self.FINAL_STRATEGY)
 
-            # calculate the final strategy separately (can often be a lot larger)
-            asset_cut_df = asset_df[[x + '.close' for x in basket_dict[self.FINAL_STRATEGY]]]
-            spot_cut_df = spot_df[[x + '.close' for x in basket_dict[self.FINAL_STRATEGY]]]
+            # Calculate the final strategy separately (can often be a lot larger)
+            asset_cut_df = asset_df[[x + '.' + br.trading_field for x in basket_dict[self.FINAL_STRATEGY]]]
+            spot_cut_df = spot_df[[x + '.' + br.trading_field for x in basket_dict[self.FINAL_STRATEGY]]]
 
             desc, results, leverage, stats, key, backtest = \
                     self.construct_individual_strategy(br, spot_cut_df, spot_df2,
                                                            asset_cut_df,
                                                            tech_params,
                                                            self.FINAL_STRATEGY,
                                                            contract_value_df, True,
@@ -1152,111 +1046,121 @@
             except:
                 pass
 
         else:
             for key in bask_keys:
                 logger.info("Calculating (single thread) " + key)
 
-                asset_cut_df = asset_df[[x + '.close' for x in basket_dict[key]]]
-                spot_cut_df = spot_df[[x + '.close' for x in basket_dict[key]]]
+                asset_cut_df = asset_df[[x + '.' + br.trading_field for x in basket_dict[key]]]
+                spot_cut_df = spot_df[[x + '.' + br.trading_field for x in basket_dict[key]]]
 
-                desc, results, leverage, stats, key, backtest = \
+                desc, results, leverage, ret_stats, key, backtest = \
                     self.construct_individual_strategy(br, spot_cut_df, spot_df2, asset_cut_df,
                                                                        tech_params, key,
                                                                        contract_value_df, False, False)
 
                 #results = backtest.portfolio_cum()
                 results.columns = desc
 
                 cum_results[results.columns[0]] = results
                 port_leverage[results.columns[0]] = leverage
-                ret_stats_results[key] = stats
+                ret_stats_results[key] = ret_stats
 
                 if key == self.FINAL_STRATEGY:
                     self._assign_final_strategy_results(results, backtest)
 
-        # get benchmark for comparison
+        # Get benchmark for comparison
         benchmark = self.construct_strategy_benchmark()
 
         cum_results_benchmark = self.compare_strategy_vs_benchmark(br, cum_results, benchmark)
 
         self._strategy_group_benchmark_pnl_ret_stats = ret_stats_results
 
         if hasattr(self, '_benchmark_ret_stats'):
             ret_stats_list = ret_stats_results
             ret_stats_list['Benchmark'] = (self._strategy_benchmark_pnl_ret_stats)
             self._strategy_group_benchmark_pnl_ret_stats = ret_stats_list
 
-        self._strategy_group_pnl = cum_results  # individual parts (all after individually applying portfolio level vol adjustment)
+        # Individual parts (all after individually applying portfolio level vol adjustment)
+        self._strategy_group_pnl = cum_results
         self._strategy_group_pnl_ret_stats = ret_stats_results
 
         self._strategy_group_leverage = port_leverage
         self._strategy_group_benchmark_pnl = cum_results_benchmark
 
     def _assign_final_strategy_results(self, results, backtest):
-            # for a key, designated as the final strategy save that as the "strategy"
+        # For a key, designated as the final strategy save that as the "strategy"
 
-            self._strategy_pnl = results  # cumulative P&L for the final strategy
-            self._strategy_components_pnl = backtest.pnl_cum()  # P&L of the individual components (after portfolio level vol adjustments)
-            self._strategy_components_pnl_ret_stats = backtest.components_pnl_ret_stats().split_into_dict()  # backtest.get_pnl_components_ret_stats()
-
-            self._strategy_pnl_ret_stats = backtest.portfolio_pnl_ret_stats()
-            self._strategy_leverage = backtest.portfolio_leverage()
-
-            # collect the position sizes and trade sizes (in several different formats)
-            self._strategy_signal = backtest.portfolio_signal()
-            self._strategy_trade_no = backtest.portfolio_trade_no()
-            self._strategy_trade = backtest.portfolio_trade()
-
-            # scaled by notional
-            self._strategy_signal_notional = backtest.portfolio_signal_notional()
-            self._strategy_trade_notional = backtest.portfolio_trade_notional()
-            self._strategy_trade_notional_sizes = backtest.portfolio_trade_notional_sizes()
-
-            # scaled by notional and adjusted into contract sizes
-            self._strategy_signal_contracts = backtest.portfolio_signal_contracts()
-            self._strategy_trade_contracts = backtest.portfolio_trade_contracts()
-
-            self._strategy_group_pnl_trades = backtest.pnl_trades()  # get individual trades P&L before (before portfolio adjustment)
-            self._strategy_pnl_trades_components = backtest.components_pnl_trades()
-
-            self._strategy_total_longs = backtest.portfolio_total_longs()
-            self._strategy_total_shorts = backtest.portfolio_total_shorts()
-            self._strategy_net_exposure = backtest.portfolio_net_exposure()
-            self._strategy_total_exposure = backtest.portfolio_total_exposure()
-
-            self._strategy_total_longs_notional = backtest.portfolio_total_longs_notional()
-            self._strategy_total_shorts_notional = backtest.portfolio_total_shorts_notional()
-            self._strategy_net_exposure_notional = backtest.portfolio_net_exposure_notional()
-            self._strategy_total_exposure_notional = backtest.portfolio_total_exposure_notional()
+        # backtest.pnl_cum()
+        # self._strategy_components_pnl_after_portfolio_weights = backtest.components_pnl_cum()
+        # self._strategy_components_pnl_ret_stats_after_portfolio_weights = backtest.components_pnl_ret_stats()
+
+        self._strategy_pnl = results  # Cumulative P&L for the final strategy
+        self._strategy_components_pnl = backtest.components_pnl_cum()  # P&L of the individual components (after portfolio level vol adjustments)
+        self._strategy_components_pnl_ret_stats = backtest.components_pnl_ret_stats().split_into_dict()  # backtest.get_pnl_components_ret_stats()
+
+        self._individual_leverage = backtest.individual_leverage()
+
+        self._strategy_pnl_ret_stats = backtest.portfolio_pnl_ret_stats()
+        self._strategy_leverage = backtest.portfolio_leverage()
+
+        # Collect the position sizes and trade sizes (in several different formats)
+        self._strategy_signal = backtest.portfolio_signal()
+        self._strategy_trade_no = backtest.portfolio_trade_no()
+        self._strategy_trade = backtest.portfolio_trade()
+
+        # Scaled by notional
+        self._strategy_signal_notional = backtest.portfolio_signal_notional()
+        self._strategy_trade_notional = backtest.portfolio_trade_notional()
+        self._strategy_trade_notional_sizes = backtest.portfolio_trade_notional_sizes()
+
+        # Scaled by notional and adjusted into contract sizes
+        self._strategy_signal_contracts = backtest.portfolio_signal_contracts()
+        self._strategy_trade_contracts = backtest.portfolio_trade_contracts()
+
+        # Get PnL by component (before portfolio vol targeting and after)
+        self._strategy_group_pnl_trades = backtest.pnl_trades()  # get individual trades P&L before (before portfolio adjustment)
+        self._strategy_pnl_trades_components = backtest.components_pnl_trades()
+
+        # Get the total size of longs, short, net exposure and total exposure
+        self._strategy_total_longs = backtest.portfolio_total_longs()
+        self._strategy_total_shorts = backtest.portfolio_total_shorts()
+        self._strategy_net_exposure = backtest.portfolio_net_exposure()
+        self._strategy_total_exposure = backtest.portfolio_total_exposure()
+
+        # Get the total notionals of longs, short, net exposure and total exposure
+        self._strategy_total_longs_notional = backtest.portfolio_total_longs_notional()
+        self._strategy_total_shorts_notional = backtest.portfolio_total_shorts_notional()
+        self._strategy_net_exposure_notional = backtest.portfolio_net_exposure_notional()
+        self._strategy_total_exposure_notional = backtest.portfolio_total_exposure_notional()
 
     def construct_individual_strategy(self, br, spot_df, spot_df2, asset_df, tech_params, key, contract_value_df,
                                       run_in_parallel, compress_output):
         """Combines the signal with asset returns to find the returns of an individual strategy
 
         Parameters
         ----------
         br : BacktestRequest
             Parameters for backtest such as start and finish dates
 
-        spot_df : pandas.DataFrame
+        spot_df : pd.DataFrame
             Market time series for generating signals
 
-        spot_df2 : pandas.DataFrame
+        spot_df2 : pd.DataFrame
             Secondary Market time series for generated signals (can be of different frequency)
 
         tech_params : TechParams
             Parameters for generating signals
 
-        contract_value_df : pandas.DataFrame
+        contract_value_df : pd.DataFrame
             Dataframe with the contract sizes for each asset
 
         Returns
         -------
-        portfolio_cum : pandas.DataFrame
+        portfolio_cum : pd.DataFrame
         backtest : Backtest
         """
         backtest = Backtest()
 
         logger = LoggerManager().getLogger(__name__)
 
         logger.info("Calculating trading signals for " + key + "...")
@@ -1272,89 +1176,106 @@
         if br.write_csv: backtest.pnl_cum().to_csv(self.DUMP_CSV + key + ".csv")
 
         if br.calc_stats:
             desc = [key + ' ' + str(backtest.portfolio_pnl_desc()[0])]
         else:
             desc = [key]
 
-        # for final strategy return heavyweight backtest object (contains lots of auxilliary information about trades etc)
+        # For final strategy return heavyweight backtest object (contains lots of auxilliary information about trades etc)
         if key == self.FINAL_STRATEGY and compress_output:
             logger.debug('Compressing ' + key)
 
             backtest = blosc.compress(pickle.dumps(backtest))
 
             logger.debug('Compressed ' + key)
 
         logger.info('Calculated for ' + key)
 
         if key != self.FINAL_STRATEGY:
-            return desc, backtest.portfolio_cum(), backtest.portfolio_leverage(), backtest.pnl_ret_stats(), key, None
+            # return desc, backtest.portfolio_cum(), backtest.portfolio_leverage(), backtest.pnl_ret_stats(), key, None
+            return desc, backtest.portfolio_cum(), backtest.portfolio_leverage(), backtest.portfolio_pnl_ret_stats(), key, None
 
-        return desc, backtest.portfolio_cum(), backtest.portfolio_leverage(), backtest.pnl_ret_stats(), key, backtest
+        return desc, backtest.portfolio_cum(), backtest.portfolio_leverage(), backtest.portfolio_pnl_ret_stats(), key, backtest
 
         # have lightweight output for subcomponents of portfolio
         # return desc, backtest.portfolio_cum(), backtest.portfolio_leverage(), backtest.portfolio_pnl_ret_stats(), \
         #       key, _
 
     def compare_strategy_vs_benchmark(self, br, strategy_df, benchmark_df):
         """Compares the trading strategy we are backtesting against a benchmark
 
         Parameters
         ----------
         br : BacktestRequest
             Parameters for backtest such as start and finish dates
-        strategy_df : pandas.DataFrame
+        strategy_df : pd.DataFrame
             Strategy time series
-        benchmark_df : pandas.DataFrame
+        benchmark_df : pd.DataFrame
             Benchmark time series
         """
 
         if br.include_benchmark:
             ret_stats = RetStats(br.resample_ann_factor)
             risk_engine = RiskEngine()
             filter = Filter()
             calculations = Calculations()
 
-            # align strategy time series with that of benchmark
+            # Align strategy time series with that of benchmark
             benchmark_df.columns = [x + ' be' for x in benchmark_df.columns]
             strategy_df, benchmark_df = strategy_df.align(benchmark_df, join='left', axis=0)
 
-            # if necessary apply vol target to benchmark (to make it comparable with strategy)
+            # If necessary apply vol target to benchmark (to make it comparable with strategy)
             if br.portfolio_vol_adjust is True:
                 benchmark_df = risk_engine.calculate_vol_adjusted_index_from_prices(benchmark_df, br=br)
 
-            # only calculate return statistics if this has been specified (note when different frequencies of data
+            # Only calculate return statistics if this has been specified (note when different frequencies of data
             # might underrepresent vol
             # if calc_stats:
             benchmark_df = benchmark_df.fillna(method='ffill')
+            benchmark_df = self._filter_by_plot_start_finish_date(benchmark_df, br)
+
             ret_stats.calculate_ret_stats_from_prices(benchmark_df, br.ann_factor)
 
             if br.calc_stats:
                 benchmark_df.columns = ret_stats.summary()
 
-            # realign strategy & benchmark
+            # Realign strategy & benchmark
             strategy_benchmark_df = strategy_df.join(benchmark_df, how='inner')
             strategy_benchmark_df = strategy_benchmark_df.fillna(method='ffill')
 
-            if br.plot_start is not None:
-                strategy_benchmark_df = filter.filter_time_series_by_date(br.plot_start, br.finish_date,
-                                                                          strategy_benchmark_df)
+            strategy_benchmark_df = self._filter_by_plot_start_finish_date(strategy_benchmark_df, br)
 
             if br.cum_index == 'mult':
                 strategy_benchmark_df = calculations.create_mult_index_from_prices(strategy_benchmark_df)
             elif br.cum_index == 'add':
                 strategy_benchmark_df = calculations.create_add_index_from_prices(strategy_benchmark_df)
 
             self._strategy_benchmark_pnl = benchmark_df
             self._strategy_benchmark_pnl_ret_stats = ret_stats
 
             return strategy_benchmark_df
 
         return strategy_df
 
+    def _filter_by_plot_start_finish_date(self, df, br):
+        if br.plot_start is None and br.plot_finish is None:
+            return df
+        else:
+            filter = Filter()
+            plot_start = br.start_date;
+            plot_finish = br.finish_date
+
+            if br.plot_start is not None:
+                plot_start = br.plot_start
+
+            if br.plot_finish is not None:
+                plot_finish = br.plot_finish
+
+            return filter.filter_time_series_by_date(plot_start, plot_finish, df)
+
     def _flatten_list(self, list_of_lists):
         """Flattens list, particularly useful for combining baskets
 
         Parameters
         ----------
         list_of_lists : str (list)
             List to be flattened
@@ -1380,56 +1301,56 @@
 
     def individual_leverage(self):
         return self._individual_leverage
 
     def strategy_group_pnl_trades(self):
         return self._strategy_group_pnl_trades
 
-    ### components
+    ### components (after signal and portfolio weighting)
     def strategy_components_pnl(self):
         return self._strategy_components_pnl
 
     def strategy_components_pnl_ret_stats(self):
         return self._strategy_components_pnl_ret_stats
 
-    ### final strategy
+    ### Final strategy
     def strategy_pnl(self):
         return self._strategy_pnl
 
     def strategy_pnl_ret_stats(self):
         return self._strategy_pnl_ret_stats
 
     def strategy_leverage(self):
         return self._strategy_leverage
 
-    ### final PNL strategy + benchmark
+    ### Final PNL strategy + benchmark
     def strategy_benchmark_pnl(self):
         return self._strategy_benchmark_pnl
 
     def strategy_benchmark_pnl_ret_stats(self):
         return self._strategy_benchmark_pnl_ret_stats
 
-    ### final PNL + group
+    ### Final PNL + group
     def strategy_group_pnl(self):
         return self._strategy_group_pnl
 
     def strategy_group_pnl_ret_stats(self):
         return self._strategy_group_pnl_ret_stats
 
-    ### final P&L + group + benchmark
+    ### Final P&L + group + benchmark
     def strategy_group_benchmark_pnl(self):
         return self._strategy_group_benchmark_pnl
 
     def strategy_group_benchmark_pnl_ret_stats(self):
         return self._strategy_group_benchmark_pnl_ret_stats
 
     def strategy_group_leverage(self):
         return self._strategy_group_leverage
 
-    # signals
+    # Signals
     def strategy_signal(self):
         return self._strategy_signal
 
     def strategy_trade(self):
         return self._strategy_trade
 
     def strategy_signal_notional(self):
@@ -1469,233 +1390,278 @@
         return self._strategy_net_exposure_notional
 
     def strategy_total_exposure_notional(self):
         return self._strategy_total_exposure_notional
 
     #### Plotting
 
+    #### Plotting
+
     def _reduce_plot(self, data_frame, reduce_plot=True, resample='B'):
         """Reduces the frequency of a time series to every business day so it can be plotted more easily
 
         Parameters
         ----------
-        data_frame: pandas.DataFrame
+        data_frame: pd.DataFrame
             Strategy time series
 
         Returns
         -------
-        pandas.DataFrame
+        pd.DataFrame
         """
         try:
-            if reduce_plot:
+            if reduce_plot and resample is not None:
                 # make plots on every business day (will downsample intraday data)
                 data_frame = data_frame.resample(resample).last()
                 data_frame = data_frame.fillna(method='pad')
 
             return data_frame
         except:
             return data_frame
 
-    ##### Quick helper functions to plot aspects of the strategy such as P&L, leverage etc.
-    def plot_individual_leverage(self, strip, silent_plot=False, reduce_plot=True, resample='B'):
+    def _chart_return_with_df(self, df, style, silent_plot, chart_type='line', ret_with_df=False, split_on_char=None):
+
+        if split_on_char is not None:
+            d_split = []
+
+            for d in df.columns:
+                try:
+                    d_split.append(d.split(".")[0])
+                except:
+                    d_split.append(d)
+
+            df.columns = d_split
+
+        chart = Chart(df, engine=self.DEFAULT_PLOT_ENGINE, chart_type=chart_type, style=style)
+        if not (silent_plot): chart.plot()
+        if ret_with_df:
+            return chart, df
+
+        return chart
+
+        ##### Quick helper functions to plot aspects of the strategy such as P&L, leverage etc.
+
+    def plot_individual_leverage(self, strip=None, silent_plot=False, reduce_plot=True, resample='B', ret_with_df=False,
+                                 split_on_char=None):
 
-        style = self._create_style("Leverage", "Individual Leverage", reduce_plot=reduce_plot)
+        style = self._create_style("Individual Leverage", "Individual Leverage", reduce_plot=reduce_plot)
 
         try:
-            chart = Chart(self._strip_dataframe(self._reduce_plot(self._individual_leverage,
-                                                                  reduce_plot=reduce_plot, resample=resample), strip),
-                          engine=self.DEFAULT_PLOT_ENGINE, chart_type='line', style=style)
-            if not (silent_plot): chart.plot()
-            return chart
+            df = self._strip_dataframe(self._reduce_plot(self._individual_leverage,
+                                                         reduce_plot=reduce_plot, resample=resample), strip)
+
+            return self._chart_return_with_df(df, style, silent_plot, chart_type='line', ret_with_df=ret_with_df,
+                                              split_on_char=split_on_char)
         except:
             pass
 
-    def plot_strategy_group_pnl_trades(self, strip=None, silent_plot=False, reduce_plot=True, resample='B'):
+    def plot_strategy_group_pnl_trades(self, strip=None, silent_plot=False, reduce_plot=True, resample='B',
+                                       ret_with_df=False, split_on_char=None):
 
         style = self._create_style("(bp)", "Individual Trade PnL", reduce_plot=reduce_plot)
 
         # zero when there isn't a trade exit
         # strategy_pnl_trades = self._strategy_pnl_trades * 100 * 100
         # strategy_pnl_trades = strategy_pnl_trades.dropna()
 
         # note only works with single large basket trade
         try:
             strategy_pnl_trades = self._strategy_group_pnl_trades.fillna(0) * 100 * 100
-            chart = Chart(self._strip_dataframe(self._reduce_plot(strategy_pnl_trades, reduce_plot=reduce_plot,
-                                                                  resample=resample), strip),
-                          engine=self.DEFAULT_PLOT_ENGINE, chart_type='line', style=style)
-            if not (silent_plot): chart.plot()
-            return chart
+            df = self._strip_dataframe(self._reduce_plot(strategy_pnl_trades, reduce_plot=reduce_plot,
+                                                         resample=resample), strip)
+
+            return self._chart_return_with_df(df, style, silent_plot, chart_type='line', ret_with_df=ret_with_df,
+                                              split_on_char=split_on_char)
         except:
             pass
 
-    def plot_strategy_pnl(self, strip=None, silent_plot=False, reduce_plot=True, resample='B'):
+    def plot_strategy_pnl(self, strip=None, silent_plot=False, reduce_plot=True, resample='B', ret_with_df=False,
+                          split_on_char=None):
 
         style = self._create_style("", "Strategy PnL", reduce_plot=reduce_plot)
 
         try:
             df = self._strip_dataframe(self._reduce_plot(self._strategy_pnl,
-                                                        reduce_plot=reduce_plot, resample=resample), strip)
-
-            chart = Chart(df, engine=self.DEFAULT_PLOT_ENGINE, chart_type='line', style=style)
-
-            if not (silent_plot): chart.plot()
+                                                         reduce_plot=reduce_plot, resample=resample), strip)
 
             if hasattr(self, 'br'):
                 if self.br.write_csv_pnl:
                     df.to_csv(self.DUMP_PATH + self.FINAL_STRATEGY + "_pnl.csv")
 
-            return chart
+            return self._chart_return_with_df(df, style, silent_plot, chart_type='line', ret_with_df=ret_with_df,
+                                              split_on_char=split_on_char)
         except Exception as e:
             print(str(e))
 
-    def plot_strategy_trade_no(self, strip=None, silent_plot=False, reduce_plot=True, resample='B'):
+    def plot_strategy_trade_no(self, strip=None, silent_plot=False, reduce_plot=True, resample='B', ret_with_df=False,
+                               split_on_char=None):
         df_trades = self._strategy_trade_no
 
         if strip is not None: df_trades.index = [k.replace(strip, '') for k in df_trades.index]
 
         style = self._create_style("", "", reduce_plot=reduce_plot)
 
         try:
             style.file_output = self.DUMP_PATH + self.FINAL_STRATEGY + ' (Strategy trade no).png'
             style.html_file_output = self.DUMP_PATH + self.FINAL_STRATEGY + ' (Strategy trade no).html'
 
-            chart = Chart(self._strip_dataframe(self._reduce_plot(df_trades, reduce_plot=reduce_plot,
-                                                                  resample=resample), strip),
-                          engine=self.DEFAULT_PLOT_ENGINE,
-                          chart_type='bar', style=style)
-            if not (silent_plot): chart.plot()
-            return chart
+            df = self._strip_dataframe(self._reduce_plot(df_trades, reduce_plot=reduce_plot, resample=resample), strip)
+
+            return self._chart_return_with_df(df, style, silent_plot, chart_type='bar', ret_with_df=ret_with_df,
+                                              split_on_char=split_on_char)
         except:
             pass
 
-    def plot_strategy_signal_proportion(self, strip=None, silent_plot=False, reduce_plot=True, resample='B'):
+    def plot_strategy_signal_proportion(self, strip=None, silent_plot=False, reduce_plot=True, resample='B',
+                                        ret_with_df=False,
+                                        split_on_char=None):
 
         signal = self._strategy_signal
 
         ####### count number of long, short and flat periods in our sample
         long = signal[signal > 0].count()
         short = signal[signal < 0].count()
         flat = signal[signal == 0].count()
 
-        df = pandas.DataFrame(index=long.index, columns=['Long', 'Short', 'Flat'])
+        df = pd.DataFrame(index=long.index, columns=['Long', 'Short', 'Flat'])
 
         df['Long'] = long
         df['Short'] = short
         df['Flat'] = flat
 
         if strip is not None: df.index = [k.replace(strip, '') for k in df.index]
 
         style = self._create_style("", "")
 
         try:
             style.file_output = self.DUMP_PATH + self.FINAL_STRATEGY + ' (Strategy signal proportion).png'
             style.html_file_output = self.DUMP_PATH + self.FINAL_STRATEGY + ' (Strategy signal proportion).html'
 
-            chart = Chart(self._strip_dataframe(self._reduce_plot(df), strip, reduce_plot=reduce_plot,
-                                                resample=resample), engine=self.DEFAULT_PLOT_ENGINE,
-                          chart_type='bar', style=style)
-            if not (silent_plot): chart.plot()
-            return chart
+            df = self._strip_dataframe(self._reduce_plot(df), strip, reduce_plot=reduce_plot,
+                                       resample=resample)
+
+            return self._chart_return_with_df(df, style, silent_plot, chart_type='bar', ret_with_df=ret_with_df,
+                                              split_on_char=split_on_char)
         except:
             pass
 
-    def plot_strategy_leverage(self, strip=None, silent_plot=False, reduce_plot=True, resample='B'):
-        style = self._create_style("Leverage", "Strategy Leverage", reduce_plot=reduce_plot)
+    def plot_strategy_leverage(self, strip=None, silent_plot=False, reduce_plot=True, resample='B', ret_with_df=False,
+                               split_on_char=None):
+        style = self._create_style("Portfolio Leverage", "Strategy Leverage", reduce_plot=reduce_plot)
 
         try:
-            chart = Chart(self._strip_dataframe(self._reduce_plot(self._strategy_leverage,
-                                                                  reduce_plot=reduce_plot, resample=resample), strip),
-                          engine=self.DEFAULT_PLOT_ENGINE, chart_type='line', style=style)
-            if not (silent_plot): chart.plot()
-            return chart
+            df = self._strip_dataframe(self._reduce_plot(self._strategy_leverage,
+                                                         reduce_plot=reduce_plot, resample=resample), strip)
+
+            return self._chart_return_with_df(df, style, silent_plot, chart_type='line', ret_with_df=ret_with_df,
+                                              split_on_char=split_on_char)
         except:
             pass
 
-    ##### plot the individual components cumulative returns and return statistics (including portfolio level constraints)
-    def plot_strategy_components_pnl(self, strip=None, silent_plot=False, reduce_plot=True, resample='B'):
+        ##### Plot the individual components cumulative returns and return statistics (including portfolio level constraints)
+
+    def plot_strategy_components_pnl(self, strip=None, silent_plot=False, reduce_plot=True, resample='B',
+                                     ret_with_df=False, split_on_char=None):
 
         style = self._create_style("Ind Components", "Strategy PnL Components", reduce_plot=reduce_plot)
 
         try:
-            chart = Chart(self._strip_dataframe(self._reduce_plot(self._strategy_components_pnl,
-                                                                  reduce_plot=reduce_plot, resample=resample), strip),
-                          engine=self.DEFAULT_PLOT_ENGINE, chart_type='line', style=style)
-            if not (silent_plot): chart.plot()
-            return chart
+            df = self._strip_dataframe(self._reduce_plot(self._strategy_components_pnl,
+                                                         reduce_plot=reduce_plot, resample=resample), strip)
+
+            return self._chart_return_with_df(df, style, silent_plot, chart_type='line', ret_with_df=ret_with_df,
+                                              split_on_char=split_on_char)
         except:
             pass
 
-    def plot_strategy_components_pnl_ir(self, strip=None, silent_plot=False):
+    def plot_strategy_components_pnl_ir(self, strip=None, silent_plot=False, ret_with_df=False,
+                                        split_on_char=None):
         return self._plot_ret_stats_helper(self._strategy_components_pnl_ret_stats, 'IR', 'Ind Component',
                                            'Ind Component IR',
                                            strip=strip,
-                                           silent_plot=silent_plot)
+                                           silent_plot=silent_plot, ret_with_df=ret_with_df,
+                                           split_on_char=split_on_char)
 
-    def plot_strategy_components_pnl_returns(self, strip=None, silent_plot=False):
+    def plot_strategy_components_pnl_returns(self, strip=None, silent_plot=False, ret_with_df=False,
+                                             split_on_char=None):
         return self._plot_ret_stats_helper(self._strategy_components_pnl_ret_stats, 'Returns', 'Ind Component (%)',
                                            'Ind Component Returns', strip=strip,
-                                           silent_plot=silent_plot)
+                                           silent_plot=silent_plot, ret_with_df=ret_with_df,
+                                           split_on_char=split_on_char)
 
-    def plot_strategy_components_pnl_vol(self, strip=None, silent_plot=False):
+    def plot_strategy_components_pnl_vol(self, strip=None, silent_plot=False, ret_with_df=False, split_on_char=None):
         return self._plot_ret_stats_helper(self._strategy_components_pnl_ret_stats, 'Vol', 'Ind Component (%)',
                                            'Ind Component Vol', strip=strip,
-                                           silent_plot=silent_plot)
+                                           silent_plot=silent_plot, ret_with_df=ret_with_df,
+                                           split_on_char=split_on_char)
 
-    def plot_strategy_components_pnl_drawdowns(self, strip=None, silent_plot=False):
+    def plot_strategy_components_pnl_drawdowns(self, strip=None, silent_plot=False, ret_with_df=False,
+                                               split_on_char=None):
         return self._plot_ret_stats_helper(self._strategy_components_pnl_ret_stats, 'Drawdowns', 'Ind Component (%)',
                                            'Ind Component Drawdowns', strip=strip,
-                                           silent_plot=silent_plot)
+                                           silent_plot=silent_plot, ret_with_df=ret_with_df,
+                                           split_on_char=split_on_char)
 
-    def plot_strategy_components_pnl_yoy(self, strip=None, silent_plot=False):
+    def plot_strategy_components_pnl_yoy(self, strip=None, silent_plot=False, ret_with_df=False,
+                                         split_on_char=None):
 
         return self.plot_yoy_helper(self._strategy_components_pnl_ret_stats, 'Ind Component YoY', 'Ind Component (%)',
-                                    strip=strip, silent_plot=silent_plot)
+                                    strip=strip, silent_plot=silent_plot, ret_with_df=ret_with_df,
+                                    split_on_char=split_on_char)
+
+        ##### plot the cumulative returns and return statistics for the strategy group
+        ##### this will plot the final strategy, benchmark and all the individual baskets (as though they were run by themselves)
 
-    ##### plot the cumulative returns and return statistics for the strategy group
-    ##### this will plot the final strategy, benchmark and all the individual baskets (as though they were run by themselves)
-    def plot_strategy_group_benchmark_pnl(self, strip=None, silent_plot=False, reduce_plot=True, resample='B'):
+    def plot_strategy_group_benchmark_pnl(self, strip=None, silent_plot=False, reduce_plot=True, resample='B',
+                                          ret_with_df=False, split_on_char=None):
         logger = LoggerManager().getLogger(__name__)
 
         style = self._create_style("", "Group Benchmark PnL - cumulative")
 
         strat_list = self._strategy_group_benchmark_pnl.columns  # .sort_values()
 
         for line in strat_list: logger.info(line)
 
         # plot cumulative line of returns
-        chart = Chart(
-            self._strip_dataframe(self._reduce_plot(self._strategy_group_benchmark_pnl,
-                                                    reduce_plot=reduce_plot, resample=resample), strip),
-            engine=self.DEFAULT_PLOT_ENGINE, chart_type='line', style=style)
+        df = self._strip_dataframe(self._reduce_plot(self._strategy_group_benchmark_pnl,
+                                                     reduce_plot=reduce_plot, resample=resample), strip)
 
-        if not (silent_plot): chart.plot()
-        return chart
+        return self._chart_return_with_df(df, style, silent_plot, chart_type='line', ret_with_df=ret_with_df,
+                                          split_on_char=split_on_char)
 
-    def plot_strategy_group_benchmark_pnl_ir(self, strip=None, silent_plot=False):
+    def plot_strategy_group_benchmark_pnl_ir(self, strip=None, silent_plot=False, ret_with_df=False,
+                                             split_on_char=None):
         return self._plot_ret_stats_helper(self._strategy_group_benchmark_pnl_ret_stats, 'IR', '',
                                            'Group Benchmark IR',
-                                           strip=strip, silent_plot=silent_plot)
+                                           strip=strip, silent_plot=silent_plot, ret_with_df=ret_with_df,
+                                           split_on_char=split_on_char)
 
-    def plot_strategy_group_benchmark_pnl_returns(self, strip=None, silent_plot=False):
+    def plot_strategy_group_benchmark_pnl_returns(self, strip=None, silent_plot=False, ret_with_df=False,
+                                                  split_on_char=None):
         return self._plot_ret_stats_helper(self._strategy_group_benchmark_pnl_ret_stats, 'Returns', '(%)',
                                            'Group Benchmark Returns',
-                                           strip=strip, silent_plot=silent_plot)
+                                           strip=strip, silent_plot=silent_plot, ret_with_df=ret_with_df,
+                                           split_on_char=split_on_char)
 
-    def plot_strategy_group_benchmark_pnl_vol(self, strip=None, silent_plot=False):
+    def plot_strategy_group_benchmark_pnl_vol(self, strip=None, silent_plot=False, ret_with_df=False,
+                                              split_on_char=None):
         return self._plot_ret_stats_helper(self._strategy_group_benchmark_pnl_ret_stats, 'Vol', '(%)',
                                            'Group Benchmark Vol',
-                                           strip=strip, silent_plot=silent_plot)
+                                           strip=strip, silent_plot=silent_plot, ret_with_df=ret_with_df,
+                                           split_on_char=split_on_char)
 
-    def plot_strategy_group_benchmark_pnl_drawdowns(self, strip=None, silent_plot=False):
+    def plot_strategy_group_benchmark_pnl_drawdowns(self, strip=None, silent_plot=False, ret_with_df=False,
+                                                    split_on_char=None):
         return self._plot_ret_stats_helper(self._strategy_group_benchmark_pnl_ret_stats, 'Drawdowns', '(%)',
                                            'Group Benchmark Drawdowns', strip=strip,
-                                           silent_plot=silent_plot)
+                                           silent_plot=silent_plot, ret_with_df=ret_with_df,
+                                           split_on_char=split_on_char)
 
-    def _plot_ret_stats_helper(self, ret_stats, metric, title, file_tag, strip=None, silent_plot=False):
+    def _plot_ret_stats_helper(self, ret_stats, metric, title, file_tag, strip=None, silent_plot=False,
+                               ret_with_df=False, split_on_char=None):
         style = self._create_style(title, file_tag)
         keys = ret_stats.keys()
         ret_metric = []
 
         for key in keys:
             if metric == 'IR':
                 ret_metric.append(ret_stats[key].inforatio()[0])
@@ -1704,227 +1670,302 @@
             elif metric == 'Vol':
                 ret_metric.append(ret_stats[key].ann_vol()[0] * 100)
             elif metric == 'Drawdowns':
                 ret_metric.append(ret_stats[key].drawdowns()[0] * 100)
 
         if strip is not None: keys = [k.replace(strip, '') for k in keys]
 
-        ret_stats = pandas.DataFrame(index=keys, data=ret_metric, columns=[metric])
+        ret_stats = pd.DataFrame(index=keys, data=ret_metric, columns=[metric])
         # ret_stats = ret_stats.sort_index()
         style.file_output = self.DUMP_PATH + self.FINAL_STRATEGY + ' (' + file_tag + ') ' + str(
             style.scale_factor) + '.png'
         style.html_file_output = self.DUMP_PATH + self.FINAL_STRATEGY + ' (' + file_tag + ') ' + str(
             style.scale_factor) + '.html'
         style.display_brand_label = False
 
-        chart = Chart(ret_stats, engine=self.DEFAULT_PLOT_ENGINE, chart_type='bar', style=style)
-        if not (silent_plot): chart.plot()
-
-        return chart
+        return self._chart_return_with_df(ret_stats, style, silent_plot, chart_type='bar', ret_with_df=ret_with_df,
+                                          split_on_char=split_on_char)
 
-    def plot_strategy_group_benchmark_pnl_yoy(self, strip=None, silent_plot=False):
+    def plot_strategy_group_benchmark_pnl_yoy(self, strip=None, silent_plot=False, split_on_char=None):
 
         return self.plot_yoy_helper(self._strategy_group_benchmark_pnl_ret_stats, "", "Group Benchmark PnL YoY",
                                     strip=strip, silent_plot=silent_plot)
 
-    def plot_yoy_helper(self, ret_stats, title, file_tag, strip=None, silent_plot=False):
+    def plot_yoy_helper(self, ret_stats, title, file_tag, strip=None, silent_plot=False, ret_with_df=False,
+                        split_on_char=None):
 
         style = self._create_style(title, title)
         # keys = self._strategy_group_benchmark_ret_stats.keys()
         yoy = []
 
         for key in ret_stats.keys():
             col = ret_stats[key].yoy_rets()
             col.columns = [key]
             yoy.append(col)
 
         calculations = Calculations()
-        ret_stats = calculations.pandas_outer_join(yoy)
+        ret_stats = calculations.join(yoy, how='outer')
         ret_stats.index = ret_stats.index.year
 
         ret_stats = self._strip_dataframe(ret_stats, strip)
 
         # ret_stats = ret_stats.sort_index()
         style.file_output = self.DUMP_PATH + self.FINAL_STRATEGY + ' (' + file_tag + ') ' \
                             + str(style.scale_factor) + '.png'
         style.html_file_output = self.DUMP_PATH + self.FINAL_STRATEGY + ' (' + file_tag + ') ' \
                                  + str(style.scale_factor) + '.html'
         style.display_brand_label = False
         style.date_formatter = "%Y"
 
-        chart = Chart(ret_stats * 100, engine=self.DEFAULT_PLOT_ENGINE, chart_type='bar', style=style)
-        if not (silent_plot): chart.plot()
-        return chart
+        ret_stats = ret_stats * 100
+
+        return self._chart_return_with_df(ret_stats, style, silent_plot, chart_type='line', ret_with_df=ret_with_df,
+                                          split_on_char=split_on_char)
 
-    def plot_strategy_group_leverage(self, silent_plot=False, reduce_plot=True, resample='B'):
+    def plot_strategy_group_leverage(self, silent_plot=False, reduce_plot=True, resample='B', ret_with_df=False,
+                                     split_on_char=None):
 
         style = self._create_style("Leverage", "Group Leverage", reduce_plot=reduce_plot)
 
-        chart = Chart(self._reduce_plot(self._strategy_group_leverage,
-                                        reduce_plot=reduce_plot, resample=resample), engine=self.DEFAULT_PLOT_ENGINE,
-                      chart_type='line', style=style)
-        if not (silent_plot): chart.plot()
-        return chart
+        df = self._reduce_plot(self._strategy_group_leverage, reduce_plot=reduce_plot, resample=resample)
+
+        return self._chart_return_with_df(df, style, silent_plot, chart_type='line', ret_with_df=ret_with_df,
+                                          split_on_char=split_on_char)
+
+    ###### Plot signals and trades, in terms of units, notionals and contract sizes (eg. for futures)
+
+    def plot_strategy_all_signals(self, signal_show=None, strip=None, silent_plot=False, reduce_plot=True, resample='B',
+                                  ret_with_df=False, split_on_char=None, multiplier=100):
+
+        style = self._create_style("positions (% portfolio notional)", "Positions", reduce_plot=reduce_plot)
+
+        df = self._strategy_signal.copy() * multiplier
+
+        if signal_show is not None:
+
+            if signal_show != []:
+                not_found = []
+
+                if split_on_char is not None:
+                    for d in df.columns:
+                        d_split = d.split(split_on_char)[0]
 
-    ###### plot signals and trades, in terms of units, notionals and contract sizes (eg. for futures)
-    def plot_strategy_signals(self, date=None, strip=None, silent_plot=False):
-        self._plot_signal(self._strategy_signal, label="positions (% portfolio notional)", caption="Positions",
-                          date=date, strip=strip, silent_plot=silent_plot)
-
-    def plot_strategy_trades(self, date=None, strip=None, silent_plot=False):
-        self._plot_signal(self._strategy_trade, label="trades (% portfolio notional)", caption="Trades",
-                          date=date, strip=strip, silent_plot=silent_plot)
-
-    def plot_strategy_signals_notional(self, date=None, strip=None, silent_plot=False):
-        self._plot_signal(self._strategy_signal_notional, label="positions (scaled by notional)", caption="Positions",
-                          date=date, strip=strip, silent_plot=silent_plot)
-
-    def plot_strategy_trades_notional(self, date=None, strip=None, silent_plot=False):
-        self._plot_signal(self._strategy_trade_notional, label="trades (scaled by notional)", caption="Trades",
-                          date=date, strip=strip, silent_plot=silent_plot)
+                        if d_split not in signal_show:
+                            not_found.append(d)
 
-    def plot_strategy_trades_notional_sizes(self, strip=None, silent_plot=False):
+                    df = df.drop(not_found, axis=1)
+
+        try:
+            df = self._strip_dataframe(self._reduce_plot(df, reduce_plot=reduce_plot,
+                                                         resample=resample), strip)
+            return self._chart_return_with_df(df, style, silent_plot, chart_type='line', ret_with_df=ret_with_df)
+        except:
+            pass
+
+    def plot_strategy_signals(self, date=None, strip=None, silent_plot=False, strip_times=False, ret_with_df=False,
+                              split_on_char=None, multiplier=100):
+        return self._plot_signal(self._strategy_signal, label="positions (% portfolio notional)", caption="Positions",
+                                 date=date, strip=strip, silent_plot=silent_plot, strip_times=strip_times,
+                                 ret_with_df=ret_with_df,
+                                 split_on_char=split_on_char, multiplier=multiplier)
+
+    def plot_strategy_trades(self, date=None, strip=None, silent_plot=False, strip_times=False, ret_with_df=False,
+                             split_on_char=None, multiplier=100):
+        return self._plot_signal(self._strategy_trade, label="trades (% portfolio notional)", caption="Trades",
+                                 date=date, strip=strip, silent_plot=silent_plot, strip_times=strip_times,
+                                 ret_with_df=ret_with_df,
+                                 split_on_char=split_on_char, multiplier=multiplier)
+
+    def plot_strategy_signals_notional(self, date=None, strip=None, silent_plot=False, strip_times=False,
+                                       ret_with_df=False,
+                                       split_on_char=None, multiplier=1):
+        return self._plot_signal(self._strategy_signal_notional, label="positions (scaled by notional)",
+                                 caption="Positions",
+                                 date=date, strip=strip, silent_plot=silent_plot, strip_times=strip_times,
+                                 ret_with_df=ret_with_df,
+                                 split_on_char=split_on_char, multiplier=multiplier)
+
+    def plot_strategy_trades_notional(self, date=None, strip=None, silent_plot=False, strip_times=False,
+                                      split_on_char=None, multiplier=1):
+        return self._plot_signal(self._strategy_trade_notional, label="trades (scaled by notional)", caption="Trades",
+                                 date=date, strip=strip, silent_plot=silent_plot, strip_times=strip_times,
+                                 split_on_char=split_on_char, multiplier=multiplier)
+
+    def plot_strategy_trades_notional_sizes(self, strip=None, silent_plot=False, ret_with_df=False, split_on_char=None):
 
         if strip is not None: self._strategy_trade_notional_sizes.index = [k.replace(strip, '')
                                                                            for k in
                                                                            self._strategy_trade_notional_sizes.index]
 
         style = self._create_style("", "", reduce_plot=False)
 
         try:
             style.file_output = self.DUMP_PATH + self.FINAL_STRATEGY + ' (Strategy trade notional size).png'
             style.html_file_output = self.DUMP_PATH + self.FINAL_STRATEGY + ' (Strategy trade notional size).html'
 
-            chart = Chart(self._strip_dataframe(self._strategy_trade_notional_sizes, strip),
-                          engine=self.DEFAULT_PLOT_ENGINE,
-                          chart_type='bar', style=style)
-            if not (silent_plot): chart.plot()
-            return chart
+            df = self._strip_dataframe(self._strategy_trade_notional_sizes, strip)
+
+            return self._chart_return_with_df(df, style, silent_plot, chart_type='bar', ret_with_df=ret_with_df,
+                                              split_on_char=split_on_char)
         except:
             pass
 
-    def plot_strategy_signals_contracts(self, date=None, strip=None, silent_plot=False):
-        self._plot_signal(self._strategy_signal_contracts, label="positions (contracts)", caption="Positions",
-                          date=date, strip=strip, silent_plot=silent_plot)
-
-    def plot_strategy_trades_contracts(self, date=None, strip=None, silent_plot=False):
-        self._plot_signal(self._strategy_trade_contracts, label="trades (contracts)", caption="Contracts",
-                          date=date, strip=strip, silent_plot=silent_plot)
-
-    ###### plot aggregated portfolio exposures
-    def plot_strategy_total_exposures(self, strip=None, silent_plot=False, reduce_plot=True, resample='B'):
-
-        df = pandas.concat([self._strategy_total_longs, self._strategy_total_shorts, self._strategy_total_exposure],
-                           axis=1)
+    def plot_strategy_signals_contracts(self, date=None, strip=None, silent_plot=False, strip_times=False,
+                                        ret_with_df=False, split_on_char=None, multiplier=1):
+        return self._plot_signal(self._strategy_signal_contracts, label="positions (contracts)", caption="Positions",
+                                 date=date, strip=strip, silent_plot=silent_plot, strip_times=strip_times,
+                                 ret_with_df=ret_with_df, split_on_char=split_on_charm, multiplier=multiplier)
+
+    def plot_strategy_trades_contracts(self, date=None, strip=None, silent_plot=False, strip_times=False,
+                                       ret_with_df=False, split_on_char=None, multiplier=1):
+        return self._plot_signal(self._strategy_trade_contracts, label="trades (contracts)", caption="Contracts",
+                                 date=date, strip=strip, silent_plot=silent_plot, strip_times=strip_times,
+                                 ret_with_df=ret_with_df, split_on_char=split_on_charm, multiplier=multiplier)
+
+        ###### plot aggregated portfolio exposures
+
+    def plot_strategy_total_exposures(self, strip=None, silent_plot=False, reduce_plot=True, resample='B',
+                                      ret_with_df=False, split_on_char=None):
+
+        style = self._create_style("", "Strategy Total Exposures")
+        df = pd.concat([self._strategy_total_longs, self._strategy_total_shorts, self._strategy_total_exposure],
+                       axis=1)
 
         try:
-            chart = Chart(
-                self._strip_dataframe(self._reduce_plot(df, reduce_plot=reduce_plot, resample=resample), strip),
-                engine=self.DEFAULT_PLOT_ENGINE, chart_type='line',
-                style=self._create_style("", "Strategy Total Exposures"))
-            if not (silent_plot): chart.plot()
-            return chart
+            df = self._strip_dataframe(self._reduce_plot(df, reduce_plot=reduce_plot, resample=resample), strip)
+            return self._chart_return_with_df(df, style, silent_plot, chart_type='line', ret_with_df=ret_with_df,
+                                              split_on_char=split_on_char)
         except:
             pass
 
-    def plot_strategy_net_exposures(self, strip=None, silent_plot=False, reduce_plot=True, resample='B'):
+    def plot_strategy_net_exposures(self, strip=None, silent_plot=False, reduce_plot=True, resample='B',
+                                    ret_with_df=False, split_on_char=None):
+        style = self._create_style("", "Strategy Net Exposures", reduce_plot=reduce_plot)
 
         try:
-            chart = Chart(self._strip_dataframe(self._reduce_plot(self._strategy_net_exposure,
-                                                                  reduce_plot=reduce_plot, resample=resample), strip),
-                          engine=self.DEFAULT_PLOT_ENGINE, chart_type='line',
-                          style=self._create_style("", "Strategy Net Exposures", reduce_plot=reduce_plot))
-            if not (silent_plot): chart.plot()
-            return chart
+            df = self._strip_dataframe(self._reduce_plot(self._strategy_net_exposure,
+                                                         reduce_plot=reduce_plot, resample=resample), strip)
+            return self._chart_return_with_df(df, style, silent_plot, chart_type='line', ret_with_df=ret_with_df,
+                                              split_on_char=split_on_char)
         except:
             pass
 
-    def plot_strategy_total_exposures_notional(self, strip=None, silent_plot=False, reduce_plot=True, resample='B'):
+    def plot_strategy_total_exposures_notional(self, strip=None, silent_plot=False, reduce_plot=True, resample='B',
+                                               ret_with_df=False, split_on_char=None):
 
-        df = pandas.concat([self._strategy_total_longs_notional,
-                            self._strategy_total_shorts_notional, self._strategy_total_exposure_notional], axis=1)
+        style = self._create_style("(mm)", "Strategy Total Exposures (mm)", reduce_plot=reduce_plot)
+        df = pd.concat([self._strategy_total_longs_notional,
+                        self._strategy_total_shorts_notional, self._strategy_total_exposure_notional], axis=1)
 
         try:
-            chart = Chart(
-                self._strip_dataframe(self._reduce_plot(df / 1000000.0, reduce_plot=reduce_plot, resample=resample),
-                                      strip),
-                engine=self.DEFAULT_PLOT_ENGINE, chart_type='line',
-                style=self._create_style("(mm)", "Strategy Total Exposures (mm)", reduce_plot=reduce_plot))
-            if not (silent_plot): chart.plot()
-            return chart
+            df = self._strip_dataframe(self._reduce_plot(df / 1000000.0, reduce_plot=reduce_plot, resample=resample),
+                                       strip)
+            return self._chart_return_with_df(df, style, silent_plot, chart_type='line', ret_with_df=ret_with_df,
+                                              split_on_char=split_on_char)
         except:
             pass
 
-    def plot_strategy_net_exposures_notional(self, strip=None, silent_plot=False, reduce_plot=True, resample='B'):
+    def plot_strategy_net_exposures_notional(self, strip=None, silent_plot=False, reduce_plot=True, resample='B',
+                                             ret_with_df=False, split_on_char=None):
+
+        style = self._create_style("(mm)", "Strategy Net Exposures (mm)", reduce_plot=reduce_plot)
 
         try:
-            chart = Chart(self._strip_dataframe(self._reduce_plot(self._strategy_net_exposure_notional / 1000000.0,
-                                                                  reduce_plot=reduce_plot, resample=resample),
-                                                strip),
-                          engine=self.DEFAULT_PLOT_ENGINE, chart_type='line',
-                          style=self._create_style("(mm)", "Strategy Net Exposures (mm)", reduce_plot=reduce_plot))
-            if not (silent_plot): chart.plot()
-            return chart
+            df = self._strip_dataframe(self._reduce_plot(self._strategy_net_exposure_notional / 1000000.0,
+                                                         reduce_plot=reduce_plot, resample=resample), strip)
+            return self._chart_return_with_df(df, style, silent_plot, chart_type='line', ret_with_df=ret_with_df,
+                                              split_on_char=split_on_char)
         except:
             pass
 
-    #### grab signals for specific days
+        #### Grab signals for specific days
+
     def _grab_signals(self, strategy_signal, date=None, strip=None):
         if date is None:
             last_day = strategy_signal.iloc[-1].transpose().to_frame()
         else:
             if not (isinstance(date, list)):
                 date = [date]
 
             last_day = []
 
+            # In case our history is not long enough
             for d in date:
-                last_day.append(strategy_signal[d].transpose().to_frame())
+                try:
+                    last_day.append(strategy_signal.iloc[d].transpose().to_frame())
+                except:
+                    pass
 
-            last_day = pandas.concat(last_day, axis=1)
+            last_day = pd.concat(last_day, axis=1)
             last_day = last_day.sort_index(axis=1)
 
         if strip is not None:
             last_day.index = [x.replace(strip, '') for x in last_day.index]
 
         return last_day
 
-    def _plot_signal(self, sig, label=' ', caption='', date=None, strip=None, silent_plot=False):
+    def _plot_signal(self, sig, label=' ', caption='', date=None, strip=None, silent_plot=False, strip_times=False,
+                     ret_with_df=False, split_on_char=None, multiplier=100):
+
+        ######## Plot signals
 
-        ######## plot signals
-        strategy_signal = 100 * (sig)
+        strategy_signal =  multiplier * (sig)
         last_day = self._grab_signals(strategy_signal, date=date, strip=strip)
 
         style = self._create_style(label, caption)
 
-        chart = Chart(last_day, engine=self.DEFAULT_PLOT_ENGINE, chart_type='bar', style=style)
-        if not (silent_plot): chart.plot()
-        return chart
+        # style.legend_x_pos = 1
+        style.legend_y_anchor = 'top'
+
+        if strip_times:
+            try:
+                last_day.index = [x.date() for x in last_day.index]
+            except:
+                pass
+
+            try:
+                last_day.columns = [x.date() for x in last_day.columns]
+            except:
+                pass
+
+        return self._chart_return_with_df(last_day, style, silent_plot, chart_type='bar', ret_with_df=ret_with_df,
+                                          split_on_char=split_on_char)
 
     def _strip_dataframe(self, data_frame, strip):
         if strip is None:
             return data_frame
 
-        data_frame.columns = [x.replace(strip, '') for x in data_frame.columns]
+        if not(isinstance(strip, list)):
+            strip = [strip]
+
+        for s in strip:
+            if s == '.':
+                data_frame.columns = [x.split(s)[0] if s in x else x for x in data_frame.columns]
+            else:
+                data_frame.columns = [x.replace(s, '') if s in x else x for x in data_frame.columns]
 
         return data_frame
 
     def _create_style(self, title, file_add, reduce_plot=True):
         style = copy.deepcopy(self.CHART_STYLE)
 
         if self.SHOW_TITLES:
             style.title = self.FINAL_STRATEGY + " " + title
             
         style.display_legend = True
         style.scale_factor = self.SCALE_FACTOR
+        style.width = self.WIDTH
+        style.height = self.HEIGHT
         style.source = self.CHART_SOURCE
-        style.silent_display = not (self.SHOW_CHARTS)
+        style.silent_display = not(self.SHOW_CHARTS)
 
-        # when plotting many points use WebGl version of plotly if specified
-        if not (reduce_plot):
+        style.legend_bgcolor = 'rgba(0,0,0,0)'
+
+        # When plotting many points use WebGl version of plotly if specified
+        if not(reduce_plot):
             style.plotly_webgl = True
 
         if self.DEFAULT_PLOT_ENGINE not in ['plotly', 'cufflinks'] and self.SAVE_FIGURES:
             style.file_output = self.DUMP_PATH + self.FINAL_STRATEGY + ' (' + file_add + ') ' \
                                 + str(style.scale_factor) + '.png'
 
         style.html_file_output = self.DUMP_PATH + self.FINAL_STRATEGY + ' (' + file_add + ') ' \
@@ -1936,17 +1977,181 @@
             pass
 
         return style
 
 
 #######################################################################################################################
 
-class PortfolioModel(object):
-    pass
+class PortfolioWeightConstruction(object):
+    """Creates dynamics weights for signals and also the portfolio
+
+    """
+
+    def __init__(self, br=None):
+        self._br = br
+        self._risk_engine = RiskEngine()
+        self._calculations = Calculations()
+
+    def optimize_portfolio_weights(self, returns_df, signal_df, signal_pnl_cols, br=None):
+
+        if br is None:
+            br = self._br
+
+        tc = br.spot_tc_bp
+
+        individual_leverage_df = None
+
+        # Do we have a vol target for individual signals?
+        if br.signal_vol_adjust is True:
+            leverage_df = self._risk_engine.calculate_leverage_factor(returns_df, br.signal_vol_target,
+                                                                br.signal_vol_max_leverage,
+                                                                br.signal_vol_periods, br.signal_vol_obs_in_year,
+                                                                br.signal_vol_rebalance_freq,
+                                                                br.signal_vol_resample_freq,
+                                                                br.signal_vol_resample_type,
+                                                                period_shift=br.signal_vol_period_shift)
+
+            signal_df = pd.DataFrame(
+                signal_df.values * leverage_df.values, index=signal_df.index, columns=signal_df.columns)
+
+            individual_leverage_df = leverage_df  # Contains leverage of individual signal (before portfolio vol target)
+
+        signal_pnl = self._calculations.calculate_signal_returns_with_tc_matrix(signal_df, returns_df, tc=tc)
+        signal_pnl.columns = signal_pnl_cols
+
+        adjusted_weights_matrix = None
+
+        # Portfolio is average of the underlying signals: should we sum them or average them or use another
+        # weighting scheme?
+        if br.portfolio_combination is not None:
+            if br.portfolio_combination == 'sum' and br.portfolio_combination_weights is None:
+                portfolio = pd.DataFrame(data=signal_pnl.sum(axis=1), index=signal_pnl.index, columns=['Portfolio'])
+            elif br.portfolio_combination == 'mean' and br.portfolio_combination_weights is None:
+                portfolio = pd.DataFrame(data=signal_pnl.mean(axis=1), index=signal_pnl.index, columns=['Portfolio'])
+
+                adjusted_weights_matrix = self.calculate_signal_weights_for_portfolio(br, signal_pnl, method='mean')
+            elif 'weighted' in br.portfolio_combination and isinstance(br.portfolio_combination_weights, dict):
+
+                # Get the weights for each asset
+                adjusted_weights_matrix = self.calculate_signal_weights_for_portfolio(br, signal_pnl, method=br.portfolio_combination)
+
+                portfolio = pd.DataFrame(data=(signal_pnl.values * adjusted_weights_matrix), index=signal_pnl.index)
+                is_all_na = pd.isnull(portfolio).all(axis=1)
+                portfolio = pd.DataFrame(portfolio.sum(axis=1), columns=['Portfolio'])
+
+                # Overwrite days when every asset PnL was null is NaN with nan
+                portfolio[is_all_na] = np.nan
+        else:
+            # Just assume to take the mean / ie. equal weights for each signal
+            portfolio = pd.DataFrame(data=signal_pnl.mean(axis=1), index=signal_pnl.index, columns=['Portfolio'])
+
+            adjusted_weights_matrix = self.calculate_signal_weights_for_portfolio(br, signal_pnl, method='mean')
 
+        portfolio_leverage_df = pd.DataFrame(data=np.ones(len(signal_pnl.index)), index=signal_pnl.index,
+                                                 columns=['Portfolio'])
+
+        # Should we apply vol target on a portfolio level basis?
+        if br.portfolio_vol_adjust is True:
+            # Calculate portfolio leverage
+            portfolio_leverage_df = self._risk_engine.calculate_leverage_factor(portfolio,
+                                                                          br.portfolio_vol_target,
+                                                                          br.portfolio_vol_max_leverage,
+                                                                          br.portfolio_vol_periods,
+                                                                          br.portfolio_vol_obs_in_year,
+                                                                          br.portfolio_vol_rebalance_freq,
+                                                                          br.portfolio_vol_resample_freq,
+                                                                          br.portfolio_vol_resample_type,
+                                                                          period_shift=br.portfolio_vol_period_shift)
+
+            # portfolio, portfolio_leverage_df = risk_engine.calculate_vol_adjusted_returns(portfolio, br = br)
+
+        # Multiply portfolio leverage * individual signals to get final position signals
+        length_cols = len(signal_df.columns)
+        leverage_matrix = np.transpose(
+            np.repeat(portfolio_leverage_df.values.flatten()[np.newaxis, :], length_cols, 0))
+
+        # Final portfolio signals (including signal & portfolio leverage)
+        portfolio_signal = pd.DataFrame(
+            data=np.multiply(leverage_matrix, signal_df.values),
+            index=signal_df.index, columns=signal_df.columns)
+
+        # Later, when we plot the portfolio components, we do that without weighting the individual components
+        portfolio_signal_before_weighting = portfolio_signal.copy()
+
+        if br.portfolio_combination is not None:
+            if 'sum' in br.portfolio_combination:
+                pass
+            elif br.portfolio_combination == 'mean' \
+                    or (br.portfolio_combination == 'weighted' and isinstance(br.portfolio_combination_weights, dict)):
+                portfolio_signal = pd.DataFrame(data=(portfolio_signal.values * adjusted_weights_matrix),
+                                                    index=portfolio_signal.index,
+                                                    columns=portfolio_signal.columns)
+        else:
+            # Otherwise it's "mean"
+            portfolio_signal = pd.DataFrame(data=(portfolio_signal.values * adjusted_weights_matrix),
+                                                index=portfolio_signal.index,
+                                                columns=portfolio_signal.columns)
+
+        
+        return portfolio_signal_before_weighting, portfolio_signal, portfolio_leverage_df, portfolio, individual_leverage_df, signal_pnl
+
+    def calculate_signal_weights_for_portfolio(self, br, signal_pnl, method='mean'):
+        """Calculates the weights of each signal for the portfolio
+
+        Parameters
+        ----------
+        br : BacktestRequest
+            Parameters for the backtest specifying start date, finish data, transaction costs etc.
+
+        signal_pnl : pd.DataFrame
+            Contains the daily P&L for the portfolio
+
+        method : String
+            'mean' - assumes equal weighting for each signal
+            'weighted' - can use predefined user weights (eg. if we assign weighting of 1, 1, 0.5, for three signals
+            the third signal will have a weighting of half versus the others)
+
+        weights : dict
+            Portfolio weights
+
+        Returns
+        -------
+        pd.DataFrame
+            Contains the portfolio weights
+        """
+
+        if method == 'mean':
+            weights_vector = np.ones(len(signal_pnl.columns))
+        elif method == 'weighted' or 'weighted-sum':
+            # Get the weights for each asset
+            weights_vector = np.array([float(br.portfolio_combination_weights[col]) for col in signal_pnl.columns])
+
+        # Repeat this down for every day
+        weights_matrix = np.repeat(weights_vector[np.newaxis, :], len(signal_pnl.index), 0)
+
+        # Where we don't have old price data, make the weights 0 there
+        ind = np.isnan(signal_pnl.values)
+        weights_matrix[ind] = 0
+
+        if method != 'weighted-sum':
+            # The total weights will vary, as historically might not have all the assets trading
+            total_weights = np.sum(weights_matrix, axis=1)
+
+            # Replicate across columns
+            total_weights = np.transpose(np.repeat(total_weights[np.newaxis, :], len(signal_pnl.columns), 0))
+
+            # To avoid divide by zero
+            total_weights[total_weights == 0.0] = 1.0
+
+            adjusted_weights_matrix = weights_matrix / total_weights
+            adjusted_weights_matrix[ind] = np.nan
+
+            return adjusted_weights_matrix
+
+        return weights_matrix
 
 #######################################################################################################################
 
 class RiskEngine(object):
     """Adjusts signal weighting according to risk constraints (volatility targeting and position limit constraints)
 
     """
@@ -1954,20 +2159,20 @@
     def calculate_vol_adjusted_index_from_prices(self, prices_df, br):
         """Adjusts an index of prices for a vol target
 
         Parameters
         ----------
         br : BacktestRequest
             Parameters for the backtest specifying start date, finish data, transaction costs etc.
-        asset_a_df : pandas.DataFrame
+        asset_a_df : pd.DataFrame
             Asset prices to be traded
 
         Returns
         -------
-        pandas.Dataframe containing vol adjusted index
+        pd.Dataframe containing vol adjusted index
         """
 
         calculations = Calculations()
 
         returns_df, leverage_df = self.calculate_vol_adjusted_returns(prices_df, br, returns=False)
 
         if br.cum_index == 'mult':
@@ -1978,20 +2183,20 @@
     def calculate_vol_adjusted_returns(self, returns_df, br, returns=True):
         """Adjusts returns for a vol target
 
         Parameters
         ----------
         br : BacktestRequest
             Parameters for the backtest specifying start date, finish data, transaction costs etc.
-        returns_a_df : pandas.DataFrame
+        returns_a_df : pd.DataFrame
             Asset returns to be traded
 
         Returns
         -------
-        pandas.DataFrame
+        pd.DataFrame
         """
 
         calculations = Calculations()
 
         if not returns: returns_df = calculations.calculate_returns(returns_df)
 
         leverage_df = self.calculate_leverage_factor(returns_df,
@@ -2030,15 +2235,15 @@
         returns : boolean
             is this returns time series or prices?
         period_shift : int
             should we delay the signal by a number of periods?
 
         Returns
         -------
-        pandas.Dataframe
+        pd.Dataframe
         """
 
         calculations = Calculations()
         filter = Filter()
 
         if resample_freq is not None:
             return
@@ -2065,15 +2270,15 @@
         # # the leverage
         # returns_df_1, lev_df = returns_df.align(lev_df, join='outer', axis=0)
         # lev_df = lev_df.fillna(method='ffill')
         #
         # # now realign back to days when we trade
         # returns_df, lev_df = returns_df.align(lev_df, join='left', axis=0)
 
-        lev_df[0:vol_periods] = numpy.nan  # ignore the first elements before the vol window kicks in
+        lev_df[0:vol_periods] = np.nan  # ignore the first elements before the vol window kicks in
 
         return lev_df
 
     def calculate_position_clip_adjustment(self, portfolio_net_exposure, portfolio_total_exposure, br):
         """Calculate the leverage adjustment that needs to be made in the portfolio such that either the net exposure or
         the absolute exposure fits within predefined limits
 
@@ -2089,43 +2294,43 @@
         Returns
         -------
         DataFrame
         """
 
         position_clip_adjustment = None
 
-        # adjust leverage of portfolio based on max NET position sizes
+        # Adjust leverage of portfolio based on max NET position sizes
         if br.max_net_exposure is not None:
             portfolio_net_exposure = portfolio_net_exposure.shift(br.position_clip_period_shift)
 
             # add further constraints on portfolio (total net amount of longs and short)
-            position_clip_adjustment = pandas.DataFrame(data=numpy.ones(len(portfolio_net_exposure.index)),
+            position_clip_adjustment = pd.DataFrame(data=np.ones(len(portfolio_net_exposure.index)),
                                                         index=portfolio_net_exposure.index,
                                                         columns=['Portfolio'])
 
             portfolio_abs_exposure = portfolio_net_exposure.abs()
 
-            # for those periods when the absolute net positioning is greater than our limit cut down the leverage
+            # For those periods when the absolute net positioning is greater than our limit cut down the leverage
             position_clip_adjustment[(portfolio_abs_exposure > br.max_net_exposure).values] = \
                 br.max_net_exposure / portfolio_abs_exposure
 
-        # adjust leverage of portfolio based on max TOTAL position sizes
+        # Adjust leverage of portfolio based on max TOTAL position sizes
         if br.max_abs_exposure is not None:
             portfolio_abs_exposure = portfolio_abs_exposure.shift(br.position_clip_period_shift)
 
             # add further constraints on portfolio (total net amount of longs and short)
-            position_clip_adjustment = pandas.DataFrame(data=numpy.ones(len(portfolio_abs_exposure.index)),
+            position_clip_adjustment = pd.DataFrame(data=np.ones(len(portfolio_abs_exposure.index)),
                                                         index=portfolio_abs_exposure.index,
                                                         columns=['Portfolio'])
 
-            # for those periods when the absolute TOTAL positioning is greater than our limit cut down the leverage
+            # For those periods when the absolute TOTAL positioning is greater than our limit cut down the leverage
             position_clip_adjustment[(portfolio_total_exposure > br.max_abs_exposure).values] = \
                 br.max_abs_exposure / portfolio_total_exposure
 
-        # only allow the position clip adjustment to change on certain days (eg. 'BM' = month end)
+        # Only allow the position clip adjustment to change on certain days (eg. 'BM' = month end)
         if br.position_clip_rebalance_freq is not None:
             calculations = Calculations()
             filter = Filter()
 
             position_clip_adjustment = filter.resample_time_series_frequency(position_clip_adjustment,
                                                                              br.position_clip_rebalance_freq,
                                                                              br.position_clip_resample_type)
```

### Comparing `finmarketpy-0.11.8/finmarketpy/backtest/backtestrequest.py` & `finmarketpy-0.11.9/finmarketpy/backtest/backtestrequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,22 +29,27 @@
     def __init__(self):
         super(MarketDataRequest, self).__init__()
 
         self.__signal_name = None
 
         # output parameters for backtest (should we add returns statistics on legends, write CSVs with returns etc.)
         self.__plot_start = None
+        self.__plot_finish = None
         self.__calc_stats = True
         self.__write_csv = False
         self.__write_csv_pnl = False
         self.__plot_interim = False
         self.__include_benchmark = False
 
+        self.__trading_field = 'close'
+
         self.__tech_params = TechParams()
 
+        self.__portfolio_weight_construction = None
+
         # default parameters for portfolio level vol adjustment
         self.__portfolio_vol_adjust = False
         self.__portfolio_vol_period_shift = 0
         self.__portfolio_vol_rebalance_freq = None
         self.__portfolio_vol_resample_freq = None
         self.__portfolio_vol_resample_type = 'mean'
         self.__portfolio_vol_target = 0.1           # 10% vol target
@@ -95,14 +100,22 @@
         
     ##### properties for output of the backtest
     @property
     def plot_start(self): return self.__plot_start
 
     @plot_start.setter
     def plot_start(self, plot_start): self.__plot_start = plot_start
+
+    @property
+    def plot_finish(self):
+        return self.__plot_finish
+
+    @plot_finish.setter
+    def plot_finish(self, plot_finish):
+        self.__plot_finish = plot_finish
     
     @property
     def calc_stats(self): return self.__calc_stats
 
     @calc_stats.setter
     def calc_stats(self, calc_stats): self.__calc_stats = calc_stats
     
@@ -127,16 +140,31 @@
     def plot_interim(self, plot_interim): self.__plot_interim = plot_interim
     
     @property
     def include_benchmark(self): return self.__include_benchmark
 
     @include_benchmark.setter
     def include_benchmark(self, include_benchmark): self.__include_benchmark = include_benchmark
+    
+    @property
+    def trading_field(self): return self.__trading_field
+
+    @trading_field.setter
+    def trading_field(self, trading_field): self.__trading_field = trading_field
+    
+    @property
+    def portfolio_weight_construction(self):
+        return self.__portfolio_weight_construction
 
-    ##### properties for portfolio level volatility adjustment
+    @portfolio_weight_construction.setter
+    def portfolio_weight_construction(self, portfolio_weight_construction):
+        self.__portfolio_weight_construction = portfolio_weight_construction
+    
+    ##### Properties for portfolio level volatility adjustment
+    
     @property
     def portfolio_vol_adjust(self): return self.__portfolio_vol_adjust
 
     @portfolio_vol_adjust.setter
     def portfolio_vol_adjust(self, portfolio_vol_adjust): self.__portfolio_vol_adjust = portfolio_vol_adjust
     
     @property
```

### Comparing `finmarketpy-0.11.8/finmarketpy/backtest/tradeanalysis.py` & `finmarketpy-0.11.9/finmarketpy/backtest/tradeanalysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,15 +292,15 @@
 
                 port, ret_stats = self._run_strategy(trading_model, asset_df, spot_df, spot_df2, br, contract_value_df,
                                                      pretty_portfolio_names[i])
 
                 port_list.append(port)
                 ret_stats_list.append(ret_stats)
 
-        port_list = Calculations().pandas_outer_join(port_list)
+        port_list = Calculations().join(port_list, how='outer')
 
         # reset the parameters of the strategy
         trading_model.br = trading_model.load_parameters()
 
         style = Style()
 
         ir = [t.inforatio()[0] for t in ret_stats_list]
@@ -417,23 +417,23 @@
         logger = LoggerManager().getLogger(__name__)
 
         calculations = Calculations()
         seas = Seasonality()
         trading_model.construct_strategy()
         pnl = trading_model.strategy_pnl()
 
-        # get seasonality by day of the month
+        # Get seasonality by day of the month
         pnl = pnl.resample('B').mean()
-        rets = calculations.calculate_returns(pnl)
+        rets = calculations.calculate_returns(pnl).tz_localize(None)
 
         bus_day = seas.bus_day_of_month_seasonality(rets, add_average=True, resample_freq=resample_freq)
 
-        # get seasonality by month
+        # Get seasonality by month
         pnl = pnl.resample('BM').mean()
-        rets = calculations.calculate_returns(pnl)
+        rets = calculations.calculate_returns(pnl).tz_localize(None)
         month = seas.monthly_seasonality(rets)
 
         logger.info("About to plot seasonality...")
         style = Style()
 
         # Plotting spot over day of month/month of year
         style.color = 'Blues'
```

### Comparing `finmarketpy-0.11.8/finmarketpy/curve/abstractcurve.py` & `finmarketpy-0.11.9/finmarketpy/curve/abstractcurve.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy/curve/abstractpricer.py` & `finmarketpy-0.11.9/finmarketpy/curve/abstractpricer.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy/curve/fxforwardscurve.py` & `finmarketpy-0.11.9/finmarketpy/curve/fxforwardscurve.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,25 +27,25 @@
 
 data_constants = DataConstants()
 market_constants = MarketConstants()
 
 class FXForwardsCurve(object):
     """Constructs continuous forwards time series total return indices from underlying forwards contracts.
 
-
     """
 
     def __init__(self, market_data_generator=None, fx_forwards_trading_tenor=market_constants.fx_forwards_trading_tenor,
                  roll_days_before=market_constants.fx_forwards_roll_days_before,
                  roll_event=market_constants.fx_forwards_roll_event, construct_via_currency='no',
                  fx_forwards_tenor_for_interpolation=market_constants.fx_forwards_tenor_for_interpolation,
                  base_depos_tenor=data_constants.base_depos_tenor,
                  roll_months=market_constants.fx_forwards_roll_months,
                  cum_index=market_constants.fx_forwards_cum_index,
-                 output_calculation_fields=market_constants.output_calculation_fields):
+                 output_calculation_fields=market_constants.output_calculation_fields,
+                 field='close'):
         """Initializes FXForwardsCurve
 
         Parameters
         ----------
         market_data_generator : MarketDataGenerator
             Used for downloading market data
 
@@ -92,64 +92,68 @@
         self._fx_forwards_tenor_for_interpolation = fx_forwards_tenor_for_interpolation
         self._base_depos_tenor = base_depos_tenor
 
         self._roll_months = roll_months
         self._cum_index = cum_index
         self._output_calcultion_fields = output_calculation_fields
 
+        self._field = field
+
     def generate_key(self):
         from findatapy.market.ioengine import SpeedCache
 
         # Don't include any "large" objects in the key
         return SpeedCache().generate_key(self, ['_market_data_generator', '_calculations', '_calendar', '_filter'])
 
     def fetch_continuous_time_series(self, md_request, market_data_generator, fx_forwards_trading_tenor=None,
                                      roll_days_before=None, roll_event=None,
                                      construct_via_currency=None, fx_forwards_tenor_for_interpolation=None, base_depos_tenor=None,
-                                     roll_months=None, cum_index=None, output_calculation_fields=False):
+                                     roll_months=None, cum_index=None, output_calculation_fields=False, field=None):
 
         if market_data_generator is None: market_data_generator = self._market_data_generator
         if fx_forwards_trading_tenor is None: fx_forwards_trading_tenor = self._fx_forwards_trading_tenor
         if roll_days_before is None: roll_days_before = self._roll_days_before
         if roll_event is None: roll_event = self._roll_event
         if construct_via_currency is None: construct_via_currency = self._construct_via_currency
         if fx_forwards_tenor_for_interpolation is None: fx_forwards_tenor_for_interpolation = self._fx_forwards_tenor_for_interpolation
         if base_depos_tenor is None: base_depos_tenor = self._base_depos_tenor
         if roll_months is None: roll_months = self._roll_months
         if cum_index is None: cum_index = self._cum_index
-        if output_calculation_fields is None: output_calculation_fields
+        if output_calculation_fields is None: output_calculation_fields = self._output_calcultion_fields
+        if field is None: field = self._field
 
         # Eg. we construct EURJPY via EURJPY directly (note: would need to have sufficient forward data for this)
         if construct_via_currency == 'no':
             # Download FX spot, FX forwards points and base depos etc.
             market = Market(market_data_generator=market_data_generator)
 
             md_request_download = MarketDataRequest(md_request=md_request)
 
             fx_conv = FXConv()
 
             # CAREFUL: convert the tickers to correct notation, eg. USDEUR => EURUSD, because our data
             # should be fetched in correct convention
             md_request_download.tickers = [fx_conv.correct_notation(x) for x in md_request.tickers]
             md_request_download.category = 'fx-forwards-market'
-            md_request_download.fields = 'close'
+            md_request_download.fields = field
             md_request_download.abstract_curve = None
             md_request_download.fx_forwards_tenor = fx_forwards_tenor_for_interpolation
             md_request_download.base_depos_tenor = base_depos_tenor
 
             forwards_market_df = market.fetch_market(md_request_download)
 
             # Now use the original tickers
             return self.construct_total_return_index(md_request.tickers, forwards_market_df,
                                                      fx_forwards_trading_tenor=fx_forwards_trading_tenor,
                                                      roll_days_before=roll_days_before, roll_event=roll_event,
                                                      fx_forwards_tenor_for_interpolation=fx_forwards_tenor_for_interpolation,
                                                      roll_months=roll_months,
                                                      cum_index=cum_index,
-                                                     output_calculation_fields=output_calculation_fields)
+                                                     output_calculation_fields=output_calculation_fields,
+                                                     field=field)
         else:
             # eg. we calculate via your domestic currency such as USD, so returns will be in your domestic currency
             # Hence AUDJPY would be calculated via AUDUSD and JPYUSD (subtracting the difference in returns)
             total_return_indices = []
 
             for tick in md_request.tickers:
                 base = tick[0:3]
@@ -165,25 +169,27 @@
                 base_vals = self.fetch_continuous_time_series(md_request_base, market_data_generator,
                                      fx_forwards_trading_tenor=fx_forwards_trading_tenor,
                                      roll_days_before=roll_days_before, roll_event=roll_event,
                                      fx_forwards_tenor_for_interpolation=fx_forwards_tenor_for_interpolation,
                                      base_depos_tenor=base_depos_tenor,
                                      roll_months=roll_months, output_calculation_fields=False,
                                      cum_index=cum_index,
-                                     construct_via_currency='no')
+                                     construct_via_currency='no',
+                                     field=field)
 
                 terms_vals = self.fetch_continuous_time_series(md_request_terms, market_data_generator,
                                      fx_forwards_trading_tenor=fx_forwards_trading_tenor,
                                      roll_days_before=roll_days_before, roll_event=roll_event,
                                      fx_forwards_tenor_for_interpolation=fx_forwards_tenor_for_interpolation,
                                      base_depos_tenor=base_depos_tenor,
                                      roll_months=roll_months,
                                      cum_index=cum_index,
                                      output_calculation_fields=False,
-                                     construct_via_currency='no')
+                                     construct_via_currency='no',
+                                     field=field)
 
                 # Special case for USDUSD case (and if base or terms USD are USDUSD
                 if base + terms == construct_via_currency + construct_via_currency:
                     base_rets = self._calculations.calculate_returns(base_vals)
                     cross_rets = pd.DataFrame(0, index=base_rets.index, columns=base_rets.columns)
                 elif base + construct_via_currency == construct_via_currency + construct_via_currency:
                     cross_rets = -self._calculations.calculate_returns(terms_vals)
@@ -195,19 +201,19 @@
 
                     cross_rets = base_rets.sub(terms_rets.iloc[:, 0], axis=0)
 
                 # First returns of a time series will by NaN, given we don't know previous point
                 cross_rets.iloc[0] = 0
 
                 cross_vals = self._calculations.create_mult_index(cross_rets)
-                cross_vals.columns = [tick + '-forward-tot.close']
+                cross_vals.columns = [tick + '-forward-tot.' + field]
 
                 total_return_indices.append(cross_vals)
 
-            return self._calculations.pandas_outer_join(total_return_indices)
+            return self._calculations.join(total_return_indices, how='outer')
 
     def unhedged_asset_fx(self, assets_df, asset_currency, home_curr, start_date, finish_date, spot_df=None):
         pass
 
     def hedged_asset_fx(self, assets_df, asset_currency, home_curr, start_date, finish_date, spot_df=None,
                         total_return_indices_df=None):
         pass
@@ -221,25 +227,27 @@
     def construct_total_return_index(self, cross_fx, forwards_market_df,
                                      fx_forwards_trading_tenor=None,
                                      roll_days_before=None,
                                      roll_event=None,
                                      roll_months=None,
                                      fx_forwards_tenor_for_interpolation=None,
                                      cum_index=None,
-                                     output_calculation_fields=False):
+                                     output_calculation_fields=None,
+                                     field=None):
 
         if not (isinstance(cross_fx, list)):
             cross_fx = [cross_fx]
 
         if fx_forwards_trading_tenor is None: fx_forwards_trading_tenor = self._fx_forwards_trading_tenor
         if roll_days_before is None: roll_days_before = self._roll_days_before
         if roll_event is None: roll_event = self._roll_event
         if roll_months is None: roll_months = self._roll_months
         if fx_forwards_tenor_for_interpolation is None: fx_forwards_tenor_for_interpolation = self._fx_forwards_tenor_for_interpolation
         if cum_index is None: cum_index = self._cum_index
+        if field is None: field = self._field
 
         total_return_index_df_agg = []
 
         # Remove columns where there is no data (because these points typically aren't quoted)
         forwards_market_df = forwards_market_df.dropna(how='all', axis=1)
 
         fx_forwards_pricer = FXForwardsPricer()
@@ -271,15 +279,15 @@
                 new_trade = np.full(len(horizon_date), False, dtype=bool)
 
                 asset_holidays = self._calendar.get_holidays(cal=cross)
 
                 # Get first delivery date
                 delivery_date.append(
                     self._calendar.get_delivery_date_from_horizon_date(horizon_date[0],
-                                                                       fx_forwards_trading_tenor, cal=cross, asset_class='fx')[0])
+                        fx_forwards_trading_tenor, cal=cross, asset_class='fx')[0])
 
                 # For first month want it to expire within that month (for consistency), hence month_adj=0 ONLY here
                 roll_date.append(get_roll_date(horizon_date[0], delivery_date[0], asset_holidays, month_adj=0))
 
                 # New trade => entry at beginning AND on every roll
                 new_trade[0] = True
 
@@ -302,15 +310,15 @@
                         roll_date.append(get_roll_date(horizon_date[i], delivery_date[i], asset_holidays))
                     else:
                         # Otherwise use previous delivery and roll dates, because we're still holding same contract
                         delivery_date.append(delivery_date[i-1])
                         roll_date.append(roll_date[i-1])
 
                 interpolated_forward = fx_forwards_pricer.price_instrument(cross, horizon_date, delivery_date, market_df=forwards_market_df,
-                         fx_forwards_tenor_for_interpolation=fx_forwards_tenor_for_interpolation)[cross + '-interpolated-outright-forward.close'].values
+                         fx_forwards_tenor_for_interpolation=fx_forwards_tenor_for_interpolation)[cross + '-interpolated-outright-forward.' + field].values
 
                 # To record MTM prices
                 mtm = np.copy(interpolated_forward)
 
                 # Note: may need to add discount factor when marking to market forwards?
 
                 # Special case: for very first trading day
@@ -319,15 +327,15 @@
                 # On rolling dates, MTM will be the previous forward contract (interpolated)
                 # otherwise it will be the current forward contract
                 for i in range(1, len(horizon_date)):
                     if new_trade[i]:
                         mtm[i] = fx_forwards_pricer.price_instrument(cross, horizon_date[i], delivery_date[i-1],
                             market_df=forwards_market_df,
                             fx_forwards_tenor_for_interpolation=fx_forwards_tenor_for_interpolation) \
-                                [cross + '-interpolated-outright-forward.close'].values
+                                [cross + '-interpolated-outright-forward.' + field].values
                     # else:
                     #    mtm[i] = interpolated_forward[i]
 
                 # Eg. if we asked for USDEUR, we first constructed spot/forwards for EURUSD
                 # and then need to invert it
                 if old_cross != cross:
                     mtm = 1.0 / mtm
@@ -337,21 +345,21 @@
                 forward_rets[0] = 0
 
                 if cum_index == 'mult':
                     cum_rets = 100 * np.cumprod(1.0 + forward_rets)
                 elif cum_index == 'add':
                     cum_rets = 100 + 100 * np.cumsum(forward_rets)
 
-                total_return_index_df = pd.DataFrame(index=horizon_date, columns=[cross + "-forward-tot.close"])
-                total_return_index_df[cross + "-forward-tot.close"] = cum_rets
+                total_return_index_df = pd.DataFrame(index=horizon_date, columns=[cross + "-forward-tot." + field])
+                total_return_index_df[cross + "-forward-tot." + field] = cum_rets
 
                 if output_calculation_fields:
-                    total_return_index_df[cross + '-interpolated-outright-forward.close'] = interpolated_forward
+                    total_return_index_df[cross + '-interpolated-outright-forward.' + field] = interpolated_forward
                     total_return_index_df[cross + '-mtm.close'] = mtm
                     total_return_index_df[cross + '-roll.close'] = new_trade
                     total_return_index_df[cross + '.roll-date'] = roll_date
                     total_return_index_df[cross + '.delivery-date'] = delivery_date
-                    total_return_index_df[cross + '-forward-return.close'] = forward_rets
+                    total_return_index_df[cross + '-forward-return.' + field] = forward_rets
 
                 total_return_index_df_agg.append(total_return_index_df)
 
-        return self._calculations.pandas_outer_join(total_return_index_df_agg)
+        return self._calculations.join(total_return_index_df_agg, how='outer')
```

### Comparing `finmarketpy-0.11.8/finmarketpy/curve/fxoptionscurve.py` & `finmarketpy-0.11.9/finmarketpy/curve/fxoptionscurve.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,15 +282,15 @@
                 cross_rets.iloc[0] = 0
 
                 cross_vals = self._calculations.create_mult_index(cross_rets)
                 cross_vals.columns = [tick + '-option-tot.close']
 
                 total_return_indices.append(cross_vals)
 
-            return self._calculations.pandas_outer_join(total_return_indices)
+            return self._calculations.join(total_return_indices, how='outer')
 
     def unhedged_asset_fx(self, assets_df, asset_currency, home_curr, start_date, finish_date, spot_df=None):
         pass
 
     def hedged_asset_fx(self, assets_df, asset_currency, home_curr, start_date, finish_date, spot_df=None,
                         total_return_indices_df=None):
         pass
@@ -663,18 +663,19 @@
                     total_return_index_df[cross + '-delta-pnl-return.close'] = delta_hedging_pnl
                     total_return_index_df[cross + '-delta-pnl-index.close'] = cum_delta_rets
                     total_return_index_df[cross + '-option-delta-return.close'] = option_delta_rets
                     total_return_index_df[cross + '-option-delta-tot.close'] = cum_option_delta_rets
 
                 total_return_index_df_agg.append(total_return_index_df)
 
-        return self._calculations.pandas_outer_join(total_return_index_df_agg)
+        return self._calculations.join(total_return_index_df_agg, how='outer')
 
-    def apply_tc_to_total_return_index(self, cross_fx, total_return_index_orig_df, option_tc_bp, spot_tc_bp, cum_index=None):
+    def apply_tc_signals_to_total_return_index(self, cross_fx, total_return_index_orig_df, option_tc_bp, spot_tc_bp, signal_df=None, cum_index=None):
 
+        # TODO signal not implemented yet
         if cum_index is None: cum_index = self._cum_index
 
         total_return_index_df_agg = []
 
         if not (isinstance(cross_fx, list)):
             cross_fx = [cross_fx]
 
@@ -715,13 +716,13 @@
 
             total_return_index_df[cross + "-option-tot-with-tc.close"] = cum_rets
             total_return_index_df[cross + '-delta-pnl-index-with-tc.close'] = cum_delta_rets
             total_return_index_df[cross + '-option-delta-tot-with-tc.close'] = cum_option_delta_rets
 
             total_return_index_df_agg.append(total_return_index_df)
 
-        return self._calculations.pandas_outer_join(total_return_index_df_agg)
+        return self._calculations.join(total_return_index_df_agg, how='outer')
```

### Comparing `finmarketpy-0.11.8/finmarketpy/curve/fxspotcurve.py` & `finmarketpy-0.11.9/finmarketpy/curve/fxspotcurve.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,35 +54,37 @@
 class FXSpotCurve(object):
     """Construct total return (spot) indices for FX. In future will also convert assets from local currency to foreign currency
     denomination and construct indices from forwards series.
 
     """
 
     def __init__(self, market_data_generator=None, depo_tenor=market_constants.spot_depo_tenor, construct_via_currency='no',
-                 output_calculation_fields=market_constants.output_calculation_fields):
+                 output_calculation_fields=market_constants.output_calculation_fields, field='close'):
         self._market_data_generator = market_data_generator
         self._calculations = Calculations()
 
         self._depo_tenor = depo_tenor
         self._construct_via_currency = construct_via_currency
         self._output_calculation_fields = output_calculation_fields
+        self._field = field
 
     def generate_key(self):
         from findatapy.market.ioengine import SpeedCache
 
         # Don't include any "large" objects in the key
         return SpeedCache().generate_key(self, ['_market_data_generator', '_calculations'])
 
     def fetch_continuous_time_series(self, md_request, market_data_generator, depo_tenor=None, construct_via_currency=None,
-                                     output_calculation_fields=None):
+                                     output_calculation_fields=None, field=None):
 
         if market_data_generator is None: market_data_generator = self._market_data_generator
         if depo_tenor is None: depo_tenor = self._depo_tenor
         if construct_via_currency is None: construct_via_currency = self._construct_via_currency
         if output_calculation_fields is None: output_calculation_fields = self._output_calculation_fields
+        if field is None: field = self._field
 
         # Eg. we construct AUDJPY via AUDJPY directly
         if construct_via_currency == 'no':
             base_depo_tickers = [x[0:3] + self._depo_tenor for x in md_request.tickers]
             terms_depo_tickers = [x[3:6] + self._depo_tenor for x in md_request.tickers]
 
             depo_tickers = list(set(base_depo_tickers + terms_depo_tickers))
@@ -90,28 +92,28 @@
             market = Market(market_data_generator=market_data_generator)
 
             # Deposit data for base and terms currency
             md_request_download = MarketDataRequest(md_request=md_request)
 
             md_request_download.tickers = depo_tickers
             md_request_download.category = 'base-depos'
-            md_request_download.fields = 'close'
+            md_request_download.fields = field
             md_request_download.abstract_curve = None
 
             depo_df = market.fetch_market(md_request_download)
 
             # Spot data
             md_request_download.tickers = md_request.tickers
             md_request_download.category = 'fx'
 
             spot_df = market.fetch_market(md_request_download)
 
             return self.construct_total_return_index(md_request.tickers,
-                    self._calculations.pandas_outer_join([spot_df, depo_df]), depo_tenor=depo_tenor,
-                                                     output_calculation_fields=output_calculation_fields)
+                    self._calculations.join([spot_df, depo_df], how='outer'), depo_tenor=depo_tenor,
+                                                     output_calculation_fields=output_calculation_fields, field=field)
         else:
             # eg. we calculate via your domestic currency such as USD, so returns will be in your domestic currency
             # Hence AUDJPY would be calculated via AUDUSD and JPYUSD (subtracting the difference in returns)
             total_return_indices = []
 
             for tick in md_request.tickers:
                 base = tick[0:3]
@@ -119,16 +121,16 @@
 
                 md_request_base = MarketDataRequest(md_request=md_request)
                 md_request_base.tickers = base + construct_via_currency
 
                 md_request_terms = MarketDataRequest(md_request=md_request)
                 md_request_terms.tickers = terms + construct_via_currency
 
-                base_vals = self.fetch_continuous_time_series(md_request_base, market_data_generator, construct_via_currency='no')
-                terms_vals = self.fetch_continuous_time_series(md_request_terms, market_data_generator, construct_via_currency='no')
+                base_vals = self.fetch_continuous_time_series(md_request_base, market_data_generator, construct_via_currency='no', field=field)
+                terms_vals = self.fetch_continuous_time_series(md_request_terms, market_data_generator, construct_via_currency='no', field=field)
 
                 # Special case for USDUSD case (and if base or terms USD are USDUSD
                 if base + terms == construct_via_currency + construct_via_currency:
                     base_rets = self._calculations.calculate_returns(base_vals)
                     cross_rets = pd.DataFrame(0, index=base_rets.index, columns=base_rets.columns)
                 elif base + construct_via_currency == construct_via_currency + construct_via_currency:
                     cross_rets = -self._calculations.calculate_returns(terms_vals)
@@ -144,29 +146,29 @@
                 cross_rets.iloc[0] = 0
 
                 cross_vals = self._calculations.create_mult_index(cross_rets)
                 cross_vals.columns = [tick + '-tot.close']
 
                 total_return_indices.append(cross_vals)
 
-            return self._calculations.pandas_outer_join(total_return_indices)
+            return self._calculations.join(total_return_indices, how='outer')
 
     def unhedged_asset_fx(self, assets_df, asset_currency, home_curr, start_date, finish_date, spot_df=None):
         pass
 
     def hedged_asset_fx(self, assets_df, asset_currency, home_curr, start_date, finish_date, spot_df=None, total_return_indices_df=None):
         pass
 
     def get_day_count_conv(self, currency):
         if currency in market_constants.currencies_with_365_basis:
             return 365.0
 
         return 360.0
 
-    def construct_total_return_index(self, cross_fx, market_df, depo_tenor=None, output_calculation_fields=False):
+    def construct_total_return_index(self, cross_fx, market_df, depo_tenor=None, output_calculation_fields=None, field=None):
         """Creates total return index for selected FX crosses from spot and deposit data
 
         Parameters
         ----------
         cross_fx : String
             Crosses to construct total return indices (can be a list)
         tenor : String
@@ -180,47 +182,49 @@
         -------
         pd.DataFrame
         """
         if not (isinstance(cross_fx, list)):
             cross_fx = [cross_fx]
 
         if depo_tenor is None: depo_tenor = self._depo_tenor
+        if output_calculation_fields is None: output_calculation_fields = self._output_calculation_fields
+        if field is None: field = self._field
 
         total_return_index_df_agg = []
 
         for cross in cross_fx:
             # Get the spot series, base deposit
-            base_deposit = market_df[cross[0:3] + depo_tenor + ".close"].to_frame()
-            terms_deposit = market_df[cross[3:6] + depo_tenor + ".close"].to_frame()
+            base_deposit = market_df[cross[0:3] + depo_tenor + "." + field].to_frame()
+            terms_deposit = market_df[cross[3:6] + depo_tenor + "." + field].to_frame()
 
             # Eg. if we specify USDUSD
             if cross[0:3] == cross[3:6]:
                 total_return_index_df_agg.append(pd.DataFrame(100, index=base_deposit.index, columns=[cross + "-tot.close"]))
             else:
                 carry = base_deposit.join(terms_deposit, how='inner')
 
-                spot = market_df[cross + ".close"].to_frame()
+                spot = market_df[cross + "." + field].to_frame()
 
                 base_daycount = self.get_day_count_conv(cross[0:3])
                 terms_daycount = self.get_day_count_conv(cross[4:6])
 
                 # Align the base & terms deposits series to spot (this should already be done by construction)
                 # spot, carry = spot.align(carry, join='left', axis=0)
 
                 # Sometimes depo data can be patchy, ok to fill down, given not very volatile (don't do this with spot!)
                 carry = carry.fillna(method='ffill') / 100.0
 
                 # In case there are values missing at start of list (fudge for old data!)
                 carry = carry.fillna(method='bfill')
 
-                spot = spot[cross + ".close"].to_frame()
+                spot = spot[cross + "." + field].to_frame()
 
-                spot_vals = spot[cross + ".close"].values
-                base_deposit_vals = carry[cross[0:3] + depo_tenor + ".close"].values
-                terms_deposit_vals = carry[cross[3:6] + depo_tenor + ".close"].values
+                spot_vals = spot[cross + "." + field].values
+                base_deposit_vals = carry[cross[0:3] + depo_tenor + "." + field].values
+                terms_deposit_vals = carry[cross[3:6] + depo_tenor + "." + field].values
 
                 # Calculate the time difference between each data point (flooring it to whole days, because carry
                 # is accured when there's a new day)
                 spot['index_col'] = spot.index.floor('D')
                 time = spot['index_col'].diff()
                 spot = spot.drop('index_col', 1)
 
@@ -229,14 +233,14 @@
 
                 # Use Numba to do total return index calculation given has many loops
                 total_return_index_df = pd.DataFrame(index=spot.index, columns=[cross + "-tot.close"],
                     data=_spot_index_numba(spot_vals, time_diff, base_deposit_vals, terms_deposit_vals,
                                      base_daycount, terms_daycount))
 
                 if output_calculation_fields:
-                    total_return_index_df[cross + '-carry.close'] = carry
-                    total_return_index_df[cross + '-tot-return.close'] = total_return_index_df / total_return_index_df.shift(1) - 1.0
-                    total_return_index_df[cross + '-spot-return.close'] = spot / spot.shift(1) - 1.0
+                    total_return_index_df[cross + '-carry.' + field] = carry
+                    total_return_index_df[cross + '-tot-return.' + field] = total_return_index_df / total_return_index_df.shift(1) - 1.0
+                    total_return_index_df[cross + '-spot-return.' + field] = spot / spot.shift(1) - 1.0
 
                 total_return_index_df_agg.append(total_return_index_df)
 
-        return self._calculations.pandas_outer_join(total_return_index_df_agg)
+        return self._calculations.join(total_return_index_df_agg, how='outer')
```

### Comparing `finmarketpy-0.11.8/finmarketpy/curve/rates/fxforwardspricer.py` & `finmarketpy-0.11.9/finmarketpy/curve/rates/fxforwardspricer.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy/curve/volatility/abstractvolsurface.py` & `finmarketpy-0.11.9/finmarketpy/curve/volatility/abstractvolsurface.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,9 +87,12 @@
         extremes_dict = {'min_x': min_x, 'max_x': max_x, 'min_z': min_z, 'max_z': max_z}
 
         return vol_surface_dict, extremes_dict
 
     def _get_tenor_index(self, tenor):
         return self._tenors.index(tenor)
 
+    def _get_tenor_expiry(self, tenor):
+        return
+
     def _findate(self, date):
         return FinDate(date.day, date.month, date.year)
```

### Comparing `finmarketpy-0.11.8/finmarketpy/curve/volatility/fxoptionspricer.py` & `finmarketpy-0.11.9/finmarketpy/curve/volatility/fxoptionspricer.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,31 +42,72 @@
         self._fx_vol_surface = fx_vol_surface
         self._fx_forwards_pricer = FXForwardsPricer()
         self._premium_output = premium_output
         self._delta_output = delta_output
 
     def price_instrument(self, cross, horizon_date, strike, expiry_date=None, vol=None, notional=1000000,
                          contract_type='european-call', tenor=None,
-                         fx_vol_surface=None, premium_output=None, delta_output=None, depo_tenor=None, return_as_df=True):
+                         fx_vol_surface=None, premium_output=None, delta_output=None, depo_tenor=None, use_atm_quoted=False,
+                         return_as_df=True):
         """Prices FX options for horizon dates/expiry dates given by the user from FX spot rates, FX volatility surface
         and deposit rates.
 
         Parameters
         ----------
         cross : str
             Currency pair
 
         horizon_date : DateTimeIndex
             Horizon dates for options
 
-        expiry_date : DateTimeIndex
-            expiry dates for options
+        strike : np.ndarray, float or str
+            Strike of option
 
-        market_df : DataFrame
-            Contains FX spot, FX vol surface quotes, FX forwards and base depos
+            eg. 'atm' - at-the-money
+            eg. 'atmf' - at-the-money forward
+            eg. 'atms' - at-the-money spot
+            eg. '25d-otm' - out-of-the-money 25d
+            eg. '10d-otm
+
+        expiry_date : DateTimeIndex (optional)
+            Expiry dates for options
+
+        vol : np.ndarray (optional)
+            Umplied vol for options
+
+        notional : float
+            Notional in base currency of the option
+
+        contract_type : str
+            What type of option are we pricing?
+
+            eg. 'european-call'
+
+        tenor : str (optional)
+            Tenor of option
+
+        fx_vol_surface : FXVolSurface
+            Interpolates FX vol surface
+
+        premium_output : str
+            'pct-for' (in base currency pct) or 'pct-dom' (in terms currency pct)
+
+        delta_output : bool
+            Also output delta of options
+
+        depo_tenor : str
+            Tenor of the deposit to use in the option pricing
+
+        use_atm_quoted : bool
+            True - takes the direct market quote
+            False - uses interpolated version
+
+        return_as_df : bool
+            True - returns output as DataFrame
+            False - returns output as np.ndarray
 
         Returns
         -------
         DataFrame
         """
 
         # if market_df is None: market_df = self._market_df
@@ -133,32 +174,39 @@
                         built_vol_surface = True
 
                     # Delta neutral strike/or whatever strike is quoted as ATM
                     # usually this is ATM delta neutral strike, but can sometimes be ATMF for some Latam
                     # Take the vol directly quoted, rather than getting it from building vol surface
                     if strike[i] == 'atm':
                         strike[i] = fx_vol_surface.get_atm_strike(tenor)
-                        vol[i] = fx_vol_surface.get_atm_quoted_vol(tenor) / 100.0
-                        # vol[i] = fx_vol_surface.get_atm_vol(tenor) / 100.0 # interpolated
+
+                        if use_atm_quoted:
+                            vol[i] = fx_vol_surface.get_atm_quoted_vol(tenor) / 100.0
+                        else:
+                            vol[i] = fx_vol_surface.get_atm_vol(tenor) / 100.0 # interpolated
                     elif strike[i] == 'atms':
                         strike[i] = fx_vol_surface.get_spot() # Interpolate vol later
                     elif strike[i] == 'atmf':
                         # Quoted tenor, no need to interpolate
                         strike[i] = float(fx_vol_surface.get_all_market_data()[cross + ".close"][horizon_date[i]]) \
                                           + (float(fx_vol_surface.get_all_market_data()[cross + tenor + ".close"][horizon_date[i]]) \
                                     / self._fx_forwards_pricer.get_forwards_divisor(cross[3:6]))
 
                         # Interpolate vol later
+
+                    # TODO: work on 25d and 10d strikes
                     elif strike[i] == '25d-otm':
                         if 'call' in contract_type_:
                             strike[i] = fx_vol_surface.get_25d_call_strike(tenor)
+
                             vol[i] = fx_vol_surface.get_25d_call_vol(tenor) / 100.0
                         elif 'put' in contract_type_:
                             strike[i] = fx_vol_surface.get_25d_put_strike(tenor)
                             vol[i] = fx_vol_surface.get_25d_put_vol(tenor) / 100.0
+
                     elif strike[i] == '10d-otm':
                         if 'call' in contract_type_:
                             strike[i] = fx_vol_surface.get_10d_call_strike(tenor)
                             vol[i] = fx_vol_surface.get_10d_call_vol(tenor) / 100.0
                         elif 'put' in contract_type_:
                             strike[i] = fx_vol_surface.get_10d_put_strike(tenor)
                             vol[i] = fx_vol_surface.get_10d_put_vol(tenor) / 100.0
```

### Comparing `finmarketpy-0.11.8/finmarketpy/curve/volatility/fxvolsurface.py` & `finmarketpy-0.11.9/finmarketpy/curve/volatility/fxvolsurface.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,22 +21,22 @@
 # Future versions of FinancePy will roll FXFinVolSurfacePlus into FinFXVolSurface
 try:
     from financepy.market.volatility.FinFXVolSurfacePlus import FinFXVolSurfacePlus as FinFXVolSurface
     from financepy.market.volatility.FinFXVolSurfacePlus import FinFXATMMethod
     from financepy.market.volatility.FinFXVolSurfacePlus import FinFXDeltaMethod
     from financepy.market.volatility.FinFXVolSurfacePlus import volFunction
     from financepy.market.volatility.FinFXVolSurfacePlus import FinVolFunctionTypes
-    from financepy.finutils.FinGlobalTypes import FinSolverTypes
 except:
     from financepy.market.volatility.FinFXVolSurface import FinFXVolSurface
     from financepy.market.volatility.FinFXVolSurface import FinFXATMMethod
     from financepy.market.volatility.FinFXVolSurface import FinFXDeltaMethod
     from financepy.market.volatility.FinFXVolSurface import volFunction
     from financepy.market.volatility.FinFXVolSurface import FinVolFunctionTypes
-    from financepy.finutils.FinGlobalTypes import FinSolverTypes
+
+from financepy.finutils.FinGlobalTypes import FinSolverTypes
 
 from findatapy.util.dataconstants import DataConstants
 
 from finmarketpy.curve.volatility.abstractvolsurface import AbstractVolSurface
 from finmarketpy.util.marketconstants import MarketConstants
 from finmarketpy.util.marketutil import MarketUtil
 
@@ -50,15 +50,16 @@
 
     def __init__(self, market_df=None, asset=None, field='close', tenors=market_constants.fx_options_tenor_for_interpolation,
                  vol_function_type=market_constants.fx_options_vol_function_type,
                  atm_method=market_constants.fx_options_atm_method,
                  delta_method=market_constants.fx_options_delta_method,
                  depo_tenor=market_constants.fx_options_depo_tenor,
                  solver=market_constants.fx_options_solver,
-                 alpha=market_constants.fx_options_alpha):
+                 alpha=market_constants.fx_options_alpha,
+                 tol=market_constants.fx_options_tol):
         """Initialises object, with market data and various market conventions
 
         Parameters
         ----------
         market_df : DataFrame
             Market data with spot, FX volatility surface, FX forwards and base depos
 
@@ -67,15 +68,15 @@
 
         field : str
             Market data field to use
 
             default - 'close'
 
         tenors : str(list)
-            Tenors to be used
+            Tenors to be used (we need to avoid tenors, where there might be NaNs)
 
         vol_function_type : str
             What type of interpolation scheme to use
             default - 'CLARK5' (also 'CLARK', 'BBG' and 'SABR')
 
         atm_method : str
             How is the ATM quoted? Eg. delta neutral, ATMF etc.
@@ -164,14 +165,15 @@
             self._solver = FinSolverTypes.NELDER_MEAD
         elif solver == 'nelmer-mead-numba':
             self._solver = FinSolverTypes.NELDER_MEAD_NUMBA
         elif solver == 'cg':
             self._solver = FinSolverTypes.CONJUGATE_GRADIENT
 
         self._alpha = alpha
+        self._tol = tol
 
     def build_vol_surface(self, value_date):
         """Builds the implied volatility surface for a particular value date and calculates the benchmark strikes etc.
 
         Before we do any sort of interpolation later, we need to build the implied_vol vol surface.
 
         Parameters
@@ -221,15 +223,16 @@
                                        self._risk_reversal25DeltaVols[date_index][0],
                                        self._market_strangle10DeltaVols[date_index][0],
                                        self._risk_reversal10DeltaVols[date_index][0],
                                        self._alpha,
                                        atmMethod=self._atm_method,
                                        deltaMethod=self._delta_method,
                                        volatilityFunctionType=self._vol_function_type,
-                                       finSolverType=self._solver)
+                                       finSolverType=self._solver,
+                                       tol=self._tol) # TODO add tol
 
     def calculate_vol_for_strike_expiry(self, K, expiry_date=None, tenor='1M'):
         """Calculates the implied_vol volatility for a given strike and tenor (or expiry date, if specified). The
         expiry date/broken dates are intepolated linearly in variance space.
 
         Parameters
         ----------
@@ -279,15 +282,15 @@
         """
         if expiry_date is not None:
             expiry_date = self._findate(self._market_util.parse_date(expiry_date))
             return self._fin_fx_vol_surface.volatilityFromDeltaDate(delta_call, expiry_date)
 
         return None
 
-    def extract_vol_surface(self, num_strike_intervals=60):
+    def extract_vol_surface(self, num_strike_intervals=60, low_K_pc=0.95, high_K_pc=1.05):
         """Creates an interpolated implied vol surface which can be plotted (in strike space), and also in delta
         space for key strikes (ATM, 25d call and put). Also for key strikes converts from delta to strike space.
 
         Parameters
         ----------
         num_strike_intervals : int
             Number of points to interpolate
@@ -312,16 +315,16 @@
         df_vol_surface_quoted_points = pd.DataFrame(columns=self._fin_fx_vol_surface._tenors)
 
         # Note, at present we're not using 10d strikes
         quoted_strikes_names = ['ATM', 'STR_25D_MS', 'RR_25D_P', 'STR_10D_MS', 'RR_10D_P']
         key_strikes_names = ['K_10D_P', 'K_10D_P_MS', 'K_25D_P', 'K_25D_P_MS', 'ATM', 'K_25D_C', 'K_25D_C_MS', 'K_10D_C', 'K_10D_C_MS']
 
         # Get max/min strikes to interpolate (from the longest dated tenor)
-        low_K = self._fin_fx_vol_surface._K_25D_P[-1] * 0.95
-        high_K = self._fin_fx_vol_surface._K_25D_C[-1] * 1.05
+        low_K = self._fin_fx_vol_surface._K_25D_P[-1] * low_K_pc
+        high_K = self._fin_fx_vol_surface._K_25D_C[-1] * high_K_pc
 
         if num_strike_intervals is not None:
             # In case using old version of FinancePy
             try:
                 implied_pdf_fin_distribution = self._fin_fx_vol_surface.impliedDbns(low_K, high_K, num_strike_intervals)
             except:
                 pass
@@ -409,14 +412,26 @@
 
         params = self._fin_fx_vol_surface._parameters[tenor_index]
         t = self._fin_fx_vol_surface._texp[tenor_index]
         f = self._fin_fx_vol_surface._F0T[tenor_index]
 
         return volFunction(self._vol_function_type.value, params, np.array([K]), gaps, f, K, t)
 
+    def get_vol_strike_from_delta_tenor(self, call_delta, tenor=None, expiry_date=None):
+
+        if tenor is not None:
+            if not (isinstance(tenor, int)):
+                tenor_index = self._get_tenor_index(tenor)
+            else:
+                tenor_index = tenor
+
+            expiry_date = self._fin_fx_vol_surface._expiryDates[tenor_index]
+
+        return self._fin_fx_vol_surface.volatilityFromDeltaDate(call_delta, expiryDate=expiry_date)
+
     def get_atm_method(self):
         return self._atm_method
 
     def get_delta_method(self):
         return self._delta_method
 
     def get_all_market_data(self):
```

### Comparing `finmarketpy-0.11.8/finmarketpy/curve/volatility/volstats.py` & `finmarketpy-0.11.9/finmarketpy/curve/volatility/volstats.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy/economics/eventstudy.py` & `finmarketpy-0.11.9/finmarketpy/economics/eventstudy.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,31 +9,30 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and limitations under the License.
 #
 
 import math
-
+import numpy as np
 from pandas.tseries.offsets import CustomBusinessDay
 
 from findatapy.timeseries import Calculations, Timezone, Filter, Calendar
 
 class EventStudy(object):
     """Provides functions for doing event studies on price action on an intraday basis and daily basis.
 
     """
 
     def __init__(self):
         self.logger = LoggerManager().getLogger(__name__)
         return
 
     def get_economic_event_ret_over_custom_event_day(self, data_frame_in, event_dates, name, event, start, end,
-                                                     lagged=False,
-                                                     NYC_cutoff=10):
+                                                     lagged=False, NYC_cutoff=10):
 
         filter = Filter()
         event_dates = filter.filter_time_series_by_date(start, end, event_dates)
 
         data_frame = data_frame_in.copy(deep=True)  # because we change the dates!
 
         timezone = Timezone()
@@ -42,15 +41,15 @@
         bday = CustomBusinessDay(weekmask='Mon Tue Wed Thu Fri')
 
         event_dates_nyc = timezone.convert_index_from_UTC_to_new_york_time(event_dates)
         average_hour_nyc = numpy.average(event_dates_nyc.index.hour)
 
         event_dates = calendar.floor_date(event_dates)
 
-        # realised is traditionally on later day eg. 3rd Jan realised ON is 2nd-3rd Jan realised
+        # Realised is traditionally on later day eg. 3rd Jan realised ON is 2nd-3rd Jan realised
         # so if Fed meeting is on 2nd Jan later, then we need realised labelled on 3rd (so minus a day)
         # implied_vol expires on next day eg. 3rd Jan implied_vol ON is 3rd-4th Jan implied_vol
 
         # TODO smarter way of adjusting dates, as sometimes events can be before/after 10am NY cut
         if (lagged and average_hour_nyc >= NYC_cutoff):
             data_frame.index = data_frame.index - bday
         elif (not lagged and average_hour_nyc < NYC_cutoff):  # ie. implied_vol
@@ -58,83 +57,126 @@
 
         # set as New York time and select only those ON vols at the 10am NY cut just before the event
         data_frame_events = data_frame[event_dates.index]
         data_frame_events.columns = data_frame.columns.values + '-' + name + ' ' + event
 
         return data_frame_events
 
+    def get_daily_moves_over_custom_event(self, data_frame_rets, ef_time_frame, vol=False,
+                                             day_start=20, days=20, day_offset=0, create_index=False,
+                                             resample=False, cumsum=True, adj_cumsum_zero_point=False,
+                                             adj_zero_point=2):
+
+        return self.get_intraday_moves_over_custom_event(data_frame_rets, ef_time_frame, vol=vol,
+                                                         minute_start=day_start, mins=days, min_offset=day_offset,
+                                                         create_index=create_index, resample=resample, freq='days',
+                                                         cumsum=cumsum, adj_cumsum_zero_point=adj_cumsum_zero_point,
+                                                         adj_zero_point=adj_zero_point)
+
+    def get_weekly_moves_over_custom_event(self, data_frame_rets, ef_time_frame, vol=False,
+                                             day_start=20, days=20, day_offset=0, create_index=False,
+                                             resample=False, cumsum=True, adj_cumsum_zero_point=False,
+                                             adj_zero_point=2):
+
+        return self.get_intraday_moves_over_custom_event(data_frame_rets, ef_time_frame, vol=vol,
+                                                         minute_start=day_start, mins=days, min_offset=day_offset,
+                                                         create_index=create_index, resample=resample, freq='weeks',
+                                                         cumsum=cumsum, adj_cumsum_zero_point=adj_cumsum_zero_point,
+                                                         adj_zero_point=adj_zero_point)
+
     def get_intraday_moves_over_custom_event(self, data_frame_rets, ef_time_frame, vol=False,
                                              minute_start=5, mins=3 * 60, min_offset=0, create_index=False,
-                                             resample=False, freq='minutes', cumsum=True):
-
+                                             resample=False, freq='minutes', cumsum=True, adj_cumsum_zero_point=False,
+                                             adj_zero_point=2):
         filter = Filter()
 
         ef_time_frame = filter.filter_time_series_by_date(data_frame_rets.index[0], data_frame_rets.index[-1],
                                                           ef_time_frame)
         ef_time = ef_time_frame.index
 
         if freq == 'minutes':
             ef_time_start = ef_time - timedelta(minutes=minute_start)
             ef_time_end = ef_time + timedelta(minutes=mins)
             ann_factor = 252 * 1440
         elif freq == 'days':
             ef_time = ef_time_frame.index.normalize()
-            ef_time_start = ef_time - timedelta(days=minute_start)
-            ef_time_end = ef_time + timedelta(days=mins)
+            ef_time_start = ef_time - pandas.tseries.offsets.BusinessDay() * minute_start
+            ef_time_end = ef_time + pandas.tseries.offsets.BusinessDay() * mins
             ann_factor = 252
+        elif freq == 'weeks':
+            ef_time = ef_time_frame.index.normalize()
+            ef_time_start = ef_time - pandas.tseries.offsets.Week() * minute_start
+            ef_time_end = ef_time + pandas.tseries.offsets.Week() * mins
+            ann_factor = 52
 
-        ords = range(-minute_start + min_offset, mins + min_offset)
+        ords = list(range(-minute_start + min_offset, mins + min_offset))
+        lst_ords = list(ords)
 
-        # all data needs to be equally spaced
+        # All data needs to be equally spaced
         if resample:
-            # make sure time series is properly sampled at 1 min intervals
-            data_frame_rets = data_frame_rets.resample('1min')
-            data_frame_rets = data_frame_rets.fillna(value=0)
-            data_frame_rets = filter.remove_out_FX_out_of_hours(data_frame_rets)
-
-        data_frame_rets['Ind'] = numpy.nan
+            # Make sure time series is properly sampled at 1 min intervals
+            if freq == 'minutes':
+                data_frame_rets = data_frame_rets.resample('1min').last()
+                data_frame_rets = data_frame_rets.fillna(value=0)
+                data_frame_rets = filter.remove_out_FX_out_of_hours(data_frame_rets)
+            elif freq == 'daily':
+                data_frame_rets = data_frame_rets.resample('B').last()
+                data_frame_rets = data_frame_rets.fillna(value=0)
+            elif freq == 'weekly':
+                data_frame_rets = data_frame_rets.resample('W').last()
+                data_frame_rets = data_frame_rets.fillna(value=0)
 
         start_index = data_frame_rets.index.searchsorted(ef_time_start)
         finish_index = data_frame_rets.index.searchsorted(ef_time_end)
 
-        # not all observation windows will be same length (eg. last one?)
+        data_frame = pandas.DataFrame(index=ords, columns=ef_time_frame.index)
 
-        # fill the indices which represent minutes
-        # TODO vectorise this!
         for i in range(0, len(ef_time_frame.index)):
-            try:
-                data_frame_rets['Ind'][start_index[i]:finish_index[i]] = ords
-            except:
-                data_frame_rets['Ind'][start_index[i]:finish_index[i]] = ords[0:(finish_index[i] - start_index[i])]
-
-        data_frame_rets['Rel'] = numpy.nan
-
-        # Set the release dates
-        data_frame_rets['Rel'][start_index] = ef_time  # set entry points
-        data_frame_rets['Rel'][finish_index + 1] = numpy.zeros(len(start_index))  # set exit points
-        data_frame_rets['Rel'] = data_frame_rets['Rel'].fillna(method='pad')  # fill down signals
 
-        data_frame_rets = data_frame_rets[pandas.notnull(data_frame_rets['Ind'])]  # get rid of other
+            vals = data_frame_rets.iloc[start_index[i]:finish_index[i]].values
+
+            st = ef_time_start[i]
+            en = ef_time_end[i]
 
-        data_frame = data_frame_rets.pivot(index='Ind',
-                                           columns='Rel', values=data_frame_rets.columns[0])
+            # Add extra "future" history in case we are doing an event study which goes outside our data window
+            # (will just be filled with NaN)
+            if len(vals) < len(lst_ords):
+                extend = np.zeros((len(lst_ords) - len(vals), 1)) * np.nan
+
+                # If start window date is before we have data
+                if st < data_frame_rets.index[0]:
+                    vals = np.append(extend, vals)
+
+                # If end date window is after we have data
+                else:
+                    vals = np.append(vals, extend)
+
+            data_frame[ef_time_frame.index[i]] = vals
 
         data_frame.index.names = [None]
 
         if create_index:
             calculations = Calculations()
             data_frame.iloc[-minute_start + min_offset] = numpy.nan
             data_frame = calculations.create_mult_index(data_frame)
         else:
             if vol is True:
-                # annualise (if vol)
+                # Annualise (if vol)
                 data_frame = data_frame.rolling(center=False, window=5).std() * math.sqrt(ann_factor)
             elif cumsum:
+
                 data_frame = data_frame.cumsum()
 
+                # Adjust DataFrame so zero point shows zero returns
+                if adj_cumsum_zero_point:
+                    ind = abs(minute_start) - adj_zero_point
+
+                    for i, c in enumerate(data_frame.columns):
+                        data_frame[c] = data_frame[c] - data_frame[c].values[ind]
+
         return data_frame
 
     def get_surprise_against_intraday_moves_over_custom_event(
             self, data_frame_cross_orig, ef_time_frame, cross, event_fx, event_name, start, end,
             offset_list=[1, 5, 30, 60], add_surprise=False, surprise_field='survey-average', freq='minutes'):
 
         ticker = event_fx + "-" + event_name + ".release-date-time-full"
@@ -422,15 +464,15 @@
 
         # return super(EventsFactory, self).get_economic_event_ret_over_event_day(vol_in, name, event, start, end, lagged = realised)
 
     def get_daily_moves_over_event(self):
         # TODO
         pass
 
-    # return only US events etc. by dates
+    # Return only US events etc. by dates
     def get_intraday_moves_over_event(self, data_frame_rets, cross, event_fx, event_name, start, end, vol, mins=3 * 60,
                                       min_offset=0, create_index=False, resample=False, freq='minutes'):
 
         ef_time_frame = self.get_economic_event_date_time_dataframe(event_fx, event_name)
         ef_time_frame = self.filter.filter_time_series_by_date(start, end, ef_time_frame)
 
         return self.get_intraday_moves_over_custom_event(data_frame_rets, ef_time_frame,
```

### Comparing `finmarketpy-0.11.8/finmarketpy/economics/marketliquidity.py` & `finmarketpy-0.11.9/finmarketpy/economics/marketliquidity.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy/economics/quickchart.py` & `finmarketpy-0.11.9/finmarketpy/economics/quickchart.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy/economics/report.py` & `finmarketpy-0.11.9/finmarketpy/economics/report.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy/economics/seasonality.py` & `finmarketpy-0.11.9/finmarketpy/economics/seasonality.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,31 +28,38 @@
     """
 
     def __init__(self):
         self.config = ConfigManager()
         self.logger = LoggerManager().getLogger(__name__)
         return
 
-    def time_of_day_seasonality(self, data_frame, years=False):
+    def time_of_day_seasonality(self, data_frame, years=False, seconds=False):
 
         calculations = Calculations()
 
         if years is False:
-            return calculations.average_by_hour_min_of_day_pretty_output(data_frame)
+            if seconds:
+                return calculations.average_by_hour_min_sec_of_day_pretty_output(data_frame)
+            else:
+                return calculations.average_by_hour_min_of_day_pretty_output(data_frame)
 
         set_year = set(data_frame.index.year)
         year = sorted(list(set_year))
 
         intraday_seasonality = None
 
         commonman = CommonMan()
 
         for i in year:
-            temp_seasonality = calculations.average_by_hour_min_of_day_pretty_output(
-                data_frame[data_frame.index.year == i])
+            if seconds:
+                temp_seasonality = calculations.average_by_hour_min_sec_of_day_pretty_output(
+                    data_frame[data_frame.index.year == i])
+            else:
+                temp_seasonality = calculations.average_by_hour_min_of_day_pretty_output(
+                    data_frame[data_frame.index.year == i])
 
             temp_seasonality.columns = commonman.postfix_list(temp_seasonality.columns.values, " " + str(i))
 
             if intraday_seasonality is None:
                 intraday_seasonality = temp_seasonality
             else:
                 intraday_seasonality = intraday_seasonality.join(temp_seasonality)
```

### Comparing `finmarketpy-0.11.8/finmarketpy/economics/techindicator.py` & `finmarketpy-0.11.9/finmarketpy/economics/techindicator.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,39 +38,41 @@
         BB - Bollinger bands - buy if spot above upper Bollinger band, sell if below lower Bollinger Band
         ATR - Average True Range - useful for creating stop/take profit levels
         long_only - long only signal
 
     """
 
     def __init__(self):
-        self.logger = LoggerManager().getLogger(__name__)
         self._techind = None
         self._signal = None
 
     def create_tech_ind(
             self,
             data_frame_non_nan,
             name,
             tech_params,
             data_frame_non_nan_early=None):
+
+        logger = LoggerManager().getLogger(__name__)
+
         self._signal = None
         self._techind = None
 
         if tech_params.fillna:
             data_frame = data_frame_non_nan.fillna(method="ffill")
         else:
             data_frame = data_frame_non_nan
 
         if data_frame_non_nan_early is not None:
             data_frame_early = data_frame_non_nan_early.fillna(method="ffill")
 
         if name == "SMA":
 
             if (data_frame_non_nan_early is not None):
-                # calculate the lagged sum of the n-1 point
+                # Calculate the lagged sum of the n-1 point
                 if pd.__version__ < '0.17':
                     rolling_sum = pd.rolling_sum(
                         data_frame.shift(1).rolling,
                         window=tech_params.sma_period - 1)
                 else:
                     rolling_sum = data_frame.shift(1).rolling(
                         center=False, window=tech_params.sma_period - 1).sum()
@@ -89,15 +91,15 @@
                 else:
                     self._techind = data_frame.rolling(
                         window=tech_params.sma_period, center=False).mean()
 
                 narray = np.where(data_frame > self._techind, 1, -1)
 
             self._signal = pd.DataFrame(index=data_frame.index, data=narray)
-            self._signal.loc[0:tech_params.sma_period] = np.nan
+            self._signal.iloc[0:tech_params.sma_period] = np.nan
             self._signal.columns = [
                 x + " SMA Signal" for x in data_frame.columns.values]
 
             self._techind.columns = [
                 x + " SMA" for x in data_frame.columns.values]
 
         elif name == "EMA":
@@ -108,53 +110,55 @@
                 span=tech_params.ema_period,
                 min_periods=0,
                 adjust=True).mean()
 
             narray = np.where(data_frame > self._techind, 1, -1)
 
             self._signal = pd.DataFrame(index=data_frame.index, data=narray)
-            self._signal.loc[0:tech_params.ema_period] = np.nan
+            self._signal.iloc[0:tech_params.ema_period] = np.nan
             self._signal.columns = [
                 x + " EMA Signal" for x in data_frame.columns.values]
 
             self._techind.columns = [
                 x + " EMA" for x in data_frame.columns.values]
 
         elif name == "ROC":
-
+            # Rate of change
             if (data_frame_non_nan_early is not None):
                 self._techind = data_frame_early / \
                     data_frame.shift(tech_params.roc_period) - 1
             else:
                 self._techind = data_frame / \
                     data_frame.shift(tech_params.roc_period) - 1
 
             narray = np.where(self._techind > 0, 1, -1)
 
             self._signal = pd.DataFrame(index=data_frame.index, data=narray)
-            self._signal.loc[0:tech_params.roc_period] = np.nan
+            self._signal.iloc[0:tech_params.roc_period] = np.nan
             self._signal.columns = [
                 x + " ROC Signal" for x in data_frame.columns.values]
 
             self._techind.columns = [
                 x + " ROC" for x in data_frame.columns.values]
 
         elif name == "polarity":
+            # If data is positive or negative
             self._techind = data_frame
 
             narray = np.where(self._techind > 0, 1, -1)
 
             self._signal = pd.DataFrame(index=data_frame.index, data=narray)
             self._signal.columns = [
                 x + " Polarity Signal" for x in data_frame.columns.values]
 
             self._techind.columns = [
                 x + " Polarity" for x in data_frame.columns.values]
 
         elif name == "SMA2":
+            # Double moving average
             sma = data_frame.rolling(
                 window=tech_params.sma_period,
                 center=False).mean()
             sma2 = data_frame.rolling(
                 window=tech_params.sma2_period,
                 center=False).mean()
 
@@ -163,18 +167,20 @@
             self._signal = pd.DataFrame(index=data_frame.index, data=narray)
             self._signal.columns = [
                 x + " SMA2 Signal" for x in data_frame.columns.values]
 
             sma.columns = [x + " SMA" for x in data_frame.columns.values]
             sma2.columns = [x + " SMA2" for x in data_frame.columns.values]
             most = max(tech_params.sma_period, tech_params.sma2_period)
-            self._signal.loc[0:most] = np.nan
+            self._signal.iloc[0:most] = np.nan
             self._techind = pd.concat([sma, sma2], axis=1)
 
         elif name in ['RSI']:
+            # Relative Strength Index
+
             # delta = data_frame.diff()
             #
             # dUp, dDown = delta.copy(), delta.copy()
             # dUp[dUp < 0] = 0
             # dDown[dDown > 0] = 0
             #
             # rolUp = pd.rolling_mean(dUp, tech_params.rsi_period)
@@ -230,20 +236,20 @@
             signal[buys] = 1
             signal[sells] = -1
             signal[~(buys | sells)] = np.nan
             signal = signal.fillna(method='ffill')
 
             self._signal = signal
 
-            self._signal.loc[0:tech_params.rsi_period] = np.nan
+            self._signal.iloc[0:tech_params.rsi_period] = np.nan
             self._signal.columns = [
                 x + " RSI Signal" for x in data_frame.columns.values]
 
         elif name in ["BB"]:
-            # calcuate Bollinger bands
+            # Calcuate Bollinger bands
             mid = data_frame.rolling(
                 center=False, window=tech_params.bb_period).mean()
             mid.columns = [x + " BB Mid" for x in data_frame.columns.values]
             std_dev = data_frame.rolling(
                 center=False, window=tech_params.bb_period).std()
             BB_std = tech_params.bb_mult * std_dev
 
@@ -253,66 +259,79 @@
                 columns=data_frame.columns)
 
             upper = pd.DataFrame(
                 data=mid.values + BB_std.values,
                 index=mid.index,
                 columns=data_frame.columns)
 
-            # calculate signals
+            # Calculate signals (buy/sell)
             signal = data_frame.copy()
 
             buys = signal > upper
             sells = signal < lower
 
             signal[buys] = 1
             signal[sells] = -1
             signal[~(buys | sells)] = np.nan
             signal = signal.fillna(method='ffill')
 
             self._signal = signal
-            self._signal.loc[0:tech_params.bb_period] = np.nan
+            self._signal.iloc[0:tech_params.bb_period] = np.nan
             self._signal.columns = [
                 x + " " + name + " Signal" for x in data_frame.columns.values]
 
             lower.columns = [
                 x + " BB Lower" for x in data_frame.columns.values]
             upper.columns = [x + " BB Mid" for x in data_frame.columns.values]
             upper.columns = [
                 x + " BB Lower" for x in data_frame.columns.values]
 
             self._techind = pd.concat([lower, mid, upper], axis=1)
         elif name == "long-only":
-            # have +1 signals only
+            # Have +1 signals only
             self._techind = data_frame  # the technical indicator is just "prices"
 
             narray = np.ones((len(data_frame.index), len(data_frame.columns)))
 
             self._signal = pd.DataFrame(index=data_frame.index, data=narray)
             self._signal.columns = [
                 x + " Long Only Signal" for x in data_frame.columns.values]
 
             self._techind.columns = [
                 x + " Long Only" for x in data_frame.columns.values]
 
+        elif name == "short-only":
+            # Have -1 signals only
+            self._techind = data_frame  # the technical indicator is just "prices"
+
+            narray = np.ones((len(data_frame.index), len(data_frame.columns)))
+
+            self._signal = pd.DataFrame(index=data_frame.index, data=narray)
+            self._signal.columns = [
+                x + " Short Only Signal" for x in data_frame.columns.values]
+
+            self._techind.columns = [
+                x + " Short Only" for x in data_frame.columns.values]
+
         elif name == "ATR":
-            # get all the asset names (assume we have names 'close', 'low', 'high' in the Data)
+            # Get all the asset names (assume we have names 'close', 'low', 'high' in the Data)
             # keep ordering of assets
             asset_name = list(OrderedDict.fromkeys(
                 [x.split('.')[0] for x in data_frame.columns]))
 
             df = []
 
-            # can improve the performance of this if vectorise more!
+            # Can improve the performance of this if vectorise more!
             for a in asset_name:
 
                 close = [a + '.close']
                 low = [a + '.low']
                 high = [a + '.high']
 
-                # if we don't fill NaNs, we need to remove those rows and then
+                # If we don't fill NaNs, we need to remove those rows and then
                 # calculate the ATR
                 if not(tech_params.fillna):
                     data_frame_short = data_frame[[close[0], low[0], high[0]]]
                     data_frame_short = data_frame_short.dropna()
                 else:
                     data_frame_short = data_frame
 
@@ -332,15 +351,15 @@
                 if (not(tech_params.fillna)):
                     true_range = true_range.reindex(
                         data_frame.index, fill_value=np.nan)
 
                 df.append(true_range)
 
             calc = Calculations()
-            true_range = calc.pandas_outer_join(df)
+            true_range = calc.join(df, how='outer')
 
             self._techind = true_range.rolling(
                 window=tech_params.atr_period, center=False).mean()
             # self._techind = true_range.ewm(ignore_na=False, span=tech_params.atr_period, min_periods=0, adjust=True).mean()
 
             self._techind.columns = [x + ".close ATR" for x in asset_name]
 
@@ -374,15 +393,15 @@
 
                 if not tech_params.fillna:
                     vwap = vwap.reindex(data_frame.index, fill_value=np.nan)
 
                 df.append(vwap)
 
             calc = Calculations()
-            vwap = calc.pandas_outer_join(df)
+            vwap = calc.join(df, how='outer')
 
             self._techind = vwap
 
             self._techind.columns = [x + ".close VWAP" for x in asset_name]
 
         self.create_custom_tech_ind(
             data_frame_non_nan,
@@ -421,15 +440,15 @@
 
     def get_signal(self):
         return self._signal
 
 ##########################################################################
 
 
-class TechParams:
+class TechParams(object):
     """Holds parameters for calculation of technical indicators.
 
     """
 
     def __init__(self, fillna=True, atr_period=14, sma_period=20,
                  green_n=4, green_count=9, red_n=2, red_count=13):
         self.fillna = fillna
```

### Comparing `finmarketpy-0.11.8/finmarketpy/network_analysis/learn_network_structure.py` & `finmarketpy-0.11.9/finmarketpy/network_analysis/learn_network_structure.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy/network_analysis/plot_network_structure.py` & `finmarketpy-0.11.9/finmarketpy/network_analysis/plot_network_structure.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy/util/marketconstants.py` & `finmarketpy-0.11.9/finmarketpy/util/marketconstants.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = 'saeedamen'  # Saeed Amen
 
 #
-# Copyright 2016-2020 Cuemacro - https://www.cuemacro.com / @cuemacro
+# Copyright 2016-2021 Cuemacro - https://www.cuemacro.com / @cuemacro
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the
 # License. You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
@@ -127,18 +127,32 @@
     fx_options_premium_output = 'pct-for'
     fx_options_delta_output = 'pct-fwd-delta-prem-adj'
 
     # 'nelmer-mead' or 'nelmer-mead-numba' (faster but less accurate) or 'cg' (conjugate gradient tends to be slower, but more accurate)
     fx_options_solver = 'nelmer-mead-numba'
     fx_options_pricing_engine = 'financepy' # 'financepy' or 'finmarketpy'
 
-    # overwrite field variables with those listed in MarketCred
-    def __init__(self):
+    fx_options_tol = 1e-8
+
+    override_fields = {}
+
+    # Overwrite field variables with those listed in MarketCred or we can pass through an override_fields dictionary
+    def __init__(self, override_fields={}):
         try:
             from finmarketpy.util.marketcred import MarketCred
             cred_keys = MarketCred.__dict__.keys()
 
             for k in MarketConstants.__dict__.keys():
                 if k in cred_keys and '__' not in k:
                     setattr(MarketConstants, k, getattr(MarketCred, k))
         except:
-            pass
+            pass
+
+        # Store overrided fields
+        if override_fields == {}:
+            override_fields = MarketConstants.override_fields
+        else:
+            MarketConstants.override_fields = override_fields
+
+        for k in override_fields.keys():
+            if '__' not in k:
+                setattr(MarketConstants, k, override_fields[k])
```

### Comparing `finmarketpy-0.11.8/finmarketpy/util/marketutil.py` & `finmarketpy-0.11.9/finmarketpy/util/marketutil.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy.egg-info/PKG-INFO` & `finmarketpy-0.11.9/finmarketpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: finmarketpy
-Version: 0.11.8
+Version: 0.11.9
 Summary: finmarketpy is a Python based library for backtesting trading strategies
 Home-page: https://github.com/cuemacro/finmarketpy
 Author: Saeed Amen
 Author-email: saeed@cuemacro.com
 License: Apache 2.0
 Description: finmarketpy is a Python based library that enables you to analyze market data and also to backtest 
         trading strategies using a simple to use API, which has prebuilt templates for you to define backtest.
```

### Comparing `finmarketpy-0.11.8/finmarketpy.egg-info/SOURCES.txt` & `finmarketpy-0.11.9/finmarketpy.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 install_extra_packages.bat
 requirements.txt
 setup.py
 .github/FUNDING.yml
 binder/Dockerfile
 doc/__init__.py
 finmarketpy/__init__.py
-finmarketpy/make.py
 finmarketpy.egg-info/PKG-INFO
 finmarketpy.egg-info/SOURCES.txt
 finmarketpy.egg-info/dependency_links.txt
 finmarketpy.egg-info/not-zip-safe
 finmarketpy.egg-info/requires.txt
 finmarketpy.egg-info/top_level.txt
 finmarketpy/backtest/__init__.py
@@ -51,38 +50,35 @@
 finmarketpy/network_analysis/plot_network_structure.py
 finmarketpy/util/__init__.py
 finmarketpy/util/marketconstants.py
 finmarketpy/util/marketutil.py
 finmarketpy_examples/__init__.py
 finmarketpy_examples/backtest_example.py
 finmarketpy_examples/boe-rate.png
-finmarketpy_examples/download_data_ams.py
-finmarketpy_examples/dukascopy_example.py
 finmarketpy_examples/events_examples.py
 finmarketpy_examples/fx_forwards_indices_examples.py
 finmarketpy_examples/fx_forwards_pricing_examples.py
 finmarketpy_examples/fx_options_indices_examples.py
 finmarketpy_examples/fx_options_pricing_examples.py
 finmarketpy_examples/fx_spot_indices_examples.py
 finmarketpy_examples/fx_vol_surface_animation.py
 finmarketpy_examples/fx_vol_surface_interpolation_examples.py
 finmarketpy_examples/gold seasonality.png
-finmarketpy_examples/new_dukascopy.py
 finmarketpy_examples/quandl_examples.py
 finmarketpy_examples/quickchart_examples.py
 finmarketpy_examples/returns_examples.py
 finmarketpy_examples/seasonality_examples.py
 finmarketpy_examples/technicals_example.py
 finmarketpy_examples/tradingmodelfxtrend_bbg_example.py
 finmarketpy_examples/tradingmodelfxtrend_example.py
 finmarketpy_examples/vol_stats_examples.py
 finmarketpy_examples/vwap_example.py
 finmarketpy_examples/finmarketpy_notebooks/__init__.py
 finmarketpy_examples/finmarketpy_notebooks/backtest_example.ipynb
-finmarketpy_examples/finmarketpy_notebooks/quandl_example.ipynb
+finmarketpy_examples/finmarketpy_notebooks/market_data_example.ipynb
 finmarketpy_examples/gallery/__init__.py
 finmarketpy_examples/gallery/fx-trend-cumulative.png
 finmarketpy_examples/gallery/fx-trend-leverage.png
 finmarketpy_examples/gallery/fx-trend-trade-returns.png
 finmarketpy_examples/gallery/fx-vol-seasonality.png
 finmarketpy_examples/gallery/gold-seasonality.png
 finmarketpy_examples/gallery/usdjpy-nfp.png
```

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/backtest_example.py` & `finmarketpy-0.11.9/finmarketpy_examples/backtest_example.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/boe-rate.png` & `finmarketpy-0.11.9/finmarketpy_examples/boe-rate.png`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/events_examples.py` & `finmarketpy-0.11.9/finmarketpy_examples/events_examples.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,29 +43,29 @@
 
     from datetime import timedelta
 
     ###### Get intraday data for USD/JPY from the past few months from Bloomberg, NFP date/times from Bloomberg
     ###### then plot intraday price action around NFP for EUR/USD
 
     start_date = datetime.date.today() - timedelta(days=180)
-    finish_date = datetime.datetime.utcnow()
+    finish_date = datetime.datetime.utcnow().date()
 
     market = Market(market_data_generator=MarketDataGenerator())
 
     # Fetch NFP times from Bloomberg
     md_request = MarketDataRequest(
         start_date=start_date,              # start date
         finish_date=finish_date,            # finish date
         category="events",
         freq='daily',                       # daily data
         data_source='bloomberg',            # use Bloomberg as data source
         tickers=['NFP'],
         fields=['release-date-time-full'],  # which fields to download
         vendor_tickers=['NFP TCH Index'],   # ticker (Bloomberg)
-        cache_algo='internet_load_return')  # how to return data
+        cache_algo='cache_algo_return')  # how to return data
 
     df_event_times = market.fetch_market(md_request)
     df_event_times = pandas.DataFrame(index=df_event_times['NFP.release-date-time-full'])
 
     # Need same timezone for event times as market data (otherwise can cause problems with Pandas)
     df_event_times = df_event_times.tz_localize('utc')
 
@@ -74,15 +74,15 @@
         start_date=start_date,      # start date
         finish_date=finish_date,    # finish date
         category='fx',
         freq='intraday',                # intraday
         data_source='bloomberg',        # use Bloomberg as data source
         tickers=['USDJPY'],             # ticker (finmarketpy)
         fields=['close'],               # which fields to download
-        cache_algo='internet_load_return')  # how to return data
+        cache_algo='cache_algo_return')  # how to return data
 
     df = None
     df = market.fetch_market(md_request)
 
     calc = Calculations()
     df = calc.calculate_returns(df)
```

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/finmarketpy_notebooks/backtest_example.ipynb` & `finmarketpy-0.11.9/finmarketpy_examples/finmarketpy_notebooks/backtest_example.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.8.8'}}"}*

```diff
@@ -331,15 +331,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.9"
+            "version": "3.8.8"
         },
         "toc": {
             "base_numbering": 1,
             "nav_menu": {},
             "number_sections": true,
             "sideBar": true,
             "skip_h1_title": false,
```

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/finmarketpy_notebooks/quandl_example.ipynb` & `finmarketpy-0.11.9/finmarketpy_examples/finmarketpy_notebooks/market_data_example.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8764063404405709%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Downloading market data examples\\n'), (2, 'Saeed "*

 * *            'Amen - saeed@cuemacro.com\\n\'), (3, \'\\n\'), (4, "Getting market data using '*

 * *            'findatapy for a number of different data sources. findatapy is used extensively in '*

 * *            'finmarketpy. The idea is that we use a common API for all these different data '*

 * *            "sources, which makes it easier to combine them together in our analysis. Here we'll "*

 * *            'show some examples […]*

```diff
@@ -1,195 +1,602 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Quandl Examples\n",
-                "Getting data from Quandl API.\n",
+                "# Downloading market data examples\n",
                 "\n",
-                "This notebook extracts data from the Quandl API and dispays it in a graph."
+                "Saeed Amen - saeed@cuemacro.com\n",
+                "\n",
+                "Getting market data using findatapy for a number of different data sources. findatapy is used extensively in finmarketpy. The idea is that we use a common API for all these different data sources, which makes it easier to combine them together in our analysis. Here we'll show some examples of downloading data from `quandl` and `bloomberg`.\n",
+                "\n",
+                "findatapy also has ticker mapping functionality that allows you to use your own nicknames for tickers, rather than the vendor tickers. There are lots of in built ticker mappings already (defined in CSV files which you can edit in the config folder). Later we show, how to download our predefined ticker mappings and also how to query them, to extract the original vendor tickers. Most of the predefined tickers involve FX markets, given the focus of Cuemacro.\n",
+                "\n",
+                "Let's first do some imports for objects we'll use later from `chartpy`, `findatapy` and `finmarketpy`. We'll also disable the log output."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
-            "metadata": {},
+            "execution_count": 3,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2021-06-01T11:43:54.457449Z",
+                    "start_time": "2021-06-01T11:43:44.153477Z"
+                }
+            },
             "outputs": [],
             "source": [
                 "import datetime\n",
                 "\n",
-                "from findatapy.util.loggermanager import LoggerManager\n",
                 "from chartpy import Chart, Style\n",
-                "from findatapy.market import Market, MarketDataGenerator, MarketDataRequest"
+                "from findatapy.market import Market, MarketDataGenerator, MarketDataRequest\n",
+                "\n",
+                "# So we don't see deprecated warnings... when you're coding it's usually good to leave these!\n",
+                "import warnings\n",
+                "warnings.filterwarnings('ignore')\n",
+                "\n",
+                "# Disable logging messages, to make output tidier\n",
+                "import logging\n",
+                "import sys\n",
+                "\n",
+                "logging.disable(sys.maxsize)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This is a wrapper for logging errors/output."
+                "Set the engine to output the chart. One of the engines we can use is `matplotlib` and `plotly` is also supported. Create the `Market` object for fetching data in conjunction with `MarketDataRequest` objects."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
-            "metadata": {},
+            "execution_count": 4,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2021-06-01T11:43:55.283797Z",
+                    "start_time": "2021-06-01T11:43:54.459444Z"
+                }
+            },
             "outputs": [],
             "source": [
-                "logger = LoggerManager().getLogger(__name__)"
+                "chart = Chart(engine='matplotlib')\n",
+                "market = Market(market_data_generator=MarketDataGenerator())"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Set the engine to output the chart. The possible engines currently is only matplotlib"
+                "## What is the MarketDataRequest?\n",
+                "\n",
+                "`MarketDataRequest` is used to request market data from a data vendor/external source. Below we mention some of the properties.\n",
+                "\n",
+                "`freq` represents the frequency of the data we want to download. Note that not every data vendor will provide high frequency data for every ticker.\n",
+                "\n",
+                "* `daily` - daily data (default)\n",
+                "* `tick` - tick data (eg. `dukascopy`, `fxcm`, `bloomberg`, `eikon`)\n",
+                "* `intraday` - minute data (eg. `bloomberg`, `eikon`)\n",
+                "\n",
+                "findatapy supports many different `data_source` from a number of different vendors (both traditional market data and cryptocurrencies). Here we write a selection. We are continually adding more sources. If you'd like to sponsor the addition of a new data source let us know!\n",
+                "\n",
+                "* `bloomberg` - Bloomberg terminal/blpapi (paid) \n",
+                "* `eikon` - Refinitiv Eikon (paid)\n",
+                "* `quandl` - Quandl has a mix of free and premium data\n",
+                "* `dukascopy` - retail FX tick data (free) \n",
+                "* `fxcm` - retail FX tick data (free)\n",
+                "* `alfred` - ALFRED/FRED mostly economic data (free)\n",
+                "* `yahoo` - equities data (free)\n",
+                "* `bitcoincharts`, `poloniex`, `binance`, `bitfinex`, `gdax`, `kraken`, `bitmex`, `alphavantage`, `huobi` - crypto data\n",
+                "\n",
+                "Or  we can give `MarketDataRequest` a `csv` or `parquet` file as a source\n",
+                "\n",
+                "* `tickers`: (can be list) eg. `EURUSD` - our nickname for tickers to use internally in findatapy\n",
+                "* `vendor_tickers`: (can be list) eg. `EURUSD Curncy` - the particular vendor ticker to use for that same asset\n",
+                "* `fields`: (can be list) eg. `close` - our nickname for the field\n",
+                "* `vendor_fields`: (can be list) eg. `PX_LAST` - the particular vendor field\n",
+                "* `cache_algo` (eg. internet, memory) eg. `internet_load_return` - internet will forcibly download from the internet\n",
+                "* `quandl_api_key`: insert API key from Quandl (freely available from their website)"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 20,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "chart = Chart(engine='matplotlib')"
+                "## Downloading from Quandl example\n",
+                "\n",
+                "In the below example, we download the monthly average interest rate for UK resident monetary financial institutions, using Quandl."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
-            "metadata": {},
+            "execution_count": 3,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2021-05-04T16:36:51.312494Z",
+                    "start_time": "2021-05-04T16:36:51.299494Z"
+                }
+            },
             "outputs": [],
             "source": [
-                "market = Market(market_data_generator=MarketDataGenerator())"
+                "try:\n",
+                "    import os\n",
+                "    QUANDL_API_KEY = os.environ['QUANDL_API_KEY']\n",
+                "except:\n",
+                "    QUANDL_API_KEY = 'TYPE_YOUR_KEY_HERE'\n",
+                "\n",
+                "# Monthly average of UK resident monetary financial institutions' (excl. Central Bank) sterling\n",
+                "# Weighted average interest rate, other loans, new advances, on a fixed rate to private non-financial corporations (in percent)\n",
+                "# not seasonally adjusted\n",
+                "md_request = MarketDataRequest(\n",
+                "    start_date=\"01 Jan 2005\",  # start date\n",
+                "    data_source='quandl',      # use Quandl as data source\n",
+                "    tickers=['Weighted interest rate'],\n",
+                "    fields=['close'],         # which fields to download\n",
+                "    vendor_tickers=['BOE/CFMBJ84'],  # ticker (Bloomberg)\n",
+                "    vendor_fields=['close'],  # which Bloomberg fields to download\n",
+                "    cache_algo='internet_load_return',\n",
+                "    quandl_api_key=QUANDL_API_KEY)  # how to return data"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "MarketDataRequest is requesting data from a source.\n",
-                "\n",
-                "Data Scource: Quandl, ONS, boe, dukascopy,fxcm,alfred, yahoo, google, fred, oecd, eurostat, edgar-index, bitcoincharts, poloniex, binance, bitfinex, gdax, kraken,bitmex, alphavantage,huobi or a .csv\n",
-                "\n",
-                "Tickers: (can be list) eg. EURUSD\n",
-                "cache_algo (eg. internet, disk, memory) - internet will forcibly download from the internet\n",
-                "Quandl API Key: insert API key from Quandl. Make sure you verify your email!"
+                "We've defined the `MarketDataRequest` and now we can download it."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 4,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2021-05-04T16:36:52.213414Z",
+                    "start_time": "2021-05-04T16:36:51.314494Z"
+                }
+            },
+            "outputs": [],
+            "source": [
+                "df = market.fetch_market(md_request)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "metadata": {},
+            "source": [
+                "Set style for graph, axis labels and plot. Creates an object with essentially the same characteristics as a matplotlib graph."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2021-05-04T16:36:52.228419Z",
+                    "start_time": "2021-05-04T16:36:52.215417Z"
+                }
+            },
             "outputs": [],
             "source": [
-                "QUANDL_API_KEY = 'TYPE_YOUR_API_KEY_HERE'\n",
+                "style = Style()\n",
                 "\n",
-                "run_example = 0\n",
+                "style.title = 'BoE weighted interest rate'\n",
+                "style.scale_factor = 3\n",
+                "style.file_output = \"boe-rate.png\"\n",
+                "style.source = 'Quandl/BoE'"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Now plot it!"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2021-05-04T16:36:52.635473Z",
+                    "start_time": "2021-05-04T16:36:52.230418Z"
+                }
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAABmMAAARoCAYAAAD5BqAGAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAPYQAAD2EBqD+naQAAADh0RVh0U29mdHdhcmUAbWF0cGxvdGxpYiB2ZXJzaW9uMy4yLjIsIGh0dHA6Ly9tYXRwbG90bGliLm9yZy+WH4yJAAAgAElEQVR4nOzdd3hU1do28HtaJslkMimkkwJJIEBo0kRKhGBAFBCsoCgcXwuKYtfPBuLxRVFU9IByFEGPoogoeFCaUiT0ooSEEEgoQkjvder+/uBLPiZ7J5mWTID7d11zXcyaWc9+Zs/eM2E/s9aSCYIggIiIiIiIiIiIiIiIiNqE3N0JEBERERERERERERERXc1YjCEiIiIiIiIiIiIiImpDLMYQERERERERERERERG1IRZjiIiIiIiIiIiIiIiI2hCLMURERERERERERERERG2IxRgiIiIiIiIiIiIiIqI2xGIMERERERERERERERFRG2IxhoiIiIiIiIiIiIiIqA0p3Z0AEREREZGj1q1bh7/++suq7amnnoKfn5+bMiJb7NixAzt27LBq4/tGRERERERXM5kgCIK7kyAiIiIicsSMGTPw5ZdfWrWdOXMGMTEx7kmIbDJv3jy88cYbVm1834iIiIiI6GrGacqIiIiIrnFmsxnPPfccQkND0alTJzz++OOor693d1pELnfy5EncdNNN0Gq1SEhIwA8//ODulIiIiIiI6BrBacqIiOiasmPHDowaNcquPiqVCh4eHvD19UVgYCA6d+6M2NhY9OnTB8OGDUPPnj0hk8naKOP258g+spVOp0N5eXmbxCbHLV26FIsWLbK67+fnh7feesuNWRG53tSpU3HkyBEAQFZWFqZNm4aePXuiZ8+ebs6MiIiIiIiudizGEBERtcJoNMJoNKKmpgZ5eXlIT0+3ejwyMhJTp07F7NmzERkZ6aYsiRzXdO0OANiyZQuLMXRVqaqqaizENDAajdi+fTuLMURERERE1OY4TRkREZGTzp8/j4ULFyI+Ph7//Oc/weXY6EojNbLrahrtRdQSHutERERERNQeWIwhIiJyEb1ej9deew3Tp0+HwWBwdzpENhszZoyobdy4cW7I5Orx2muvQSaTQSaTYeXKle5OhwBotVoMGTLEqk2lUmH06NFuysg1oqKiGo81oqb4WdR+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gnPnzrUYR6VSISAgACaTCcXFxXbnwWIMEREREdll7NixeOWVV/DWW29ZtVssFmzYsAEbNmxwKr5arcYnn3yC+++/36k4REREREREzmqYusvRQkBzampq7O7TMKWZXO76Ca8EQbA5bsMInfbmyD67vJ+Pj4/osfz8fJuLMcHBwZDL5SgoKHDoWGAxhoiIiIjs9s9//hOhoaF4/vnnnV4v5nJjx47FwoULRVOhERERERERuYO3tzcAxwsBzXFkvZWG0SgymczmPmq1GgEBAdBoNPD29oZSqYRCoRAVXmwdFQPA7rVSXMVoNDrUr66uDsClfdFUbW0tqqqqoNVq4evri8rKymbjODNFGcBiDBERERE5aPbs2Zg4cSLmzZuH77//3uH/nAQEBGD8+PF49NFHMWzYMBdnSURERERE5LiGIoWrF6tvGOXSVrRaLbp06QI/Pz+7ije28iV3SAAAIABJREFUaOvcXb3dy/splUrRe5mfnw+tVouQkJBmizEajQZarRa1tbUtFmxawmIMERERETksKioKX3zxBZYsWYJNmzZhz549SE9Px6lTp1BRUYHq6moYjUZ4e3vDx8cHPj4+CA8PR0JCAhISEjBgwADccMMNUCgU7n4pREREREREIg3FGHcVIBwRGRmJLl26QCaTobq6GsXFxaisrER9fT0MBgMsFotozZekpCSb47tjvRhnttvwemUymeRUbIWFhYiNjUVQUBCys7Mlt9MwKqagoMChHAAWY4iIiIjIBby8vDB58mRMnjzZ3akQERERERG5TFuu09IWwsLC0LVrV5jNZmRlZaGoqMjdKbmMoz/ik8vljaODpIpqJpMJJSUlCAoKQmBgIIqLi0XPCQkJgSAIDk9RBgBXxhFERERERERERERERNTOGqa0smdNFXdRKBTo2rUrACAzM9PmQoyrpzFrK44WxBqKOIIgNDvCqWHES8MImMv5+/vDw8MDZWVlMBgMDuUAsBhDRERERERERERERCSpvr4eAODj4+PmTFoXGBgIpVKJqqoqlJSU2NzvSig0AYBarXaon7e3NwBAr9c3+5zS0lIYDAYEBASI9ocrpigDWIwhIiIiIiIiIiIiIpJUVVUF4NIC7h19qrKGglFFRYVd/RqKFR2do3lqtVoA//+9lCIIAgoLCyGXyxEUFNTYLpfLERgYCJPJJDl9mT069tFDREREREREREREROQmtbW10Ov1UCgUVhfpO6KG6bgaplazlb+/f1ukIyIIAgDHp0XTaDQOjeJpeN9aK1I1jHwJDg5ubGsYbVRYWAiLxWL3ti/HYgwRERERERERERERUTMuXrwIAIiMjOzQ66s0FGFUKpXNfeRyOcLCwtoqJSsN67XYk9/lmo5asYVWq4Wvry8sFgsKCwtbfG51dTWqq6uh0+ng4eEB4P8XZpydogxgMYaIiIiIiIiIiIiIqFkXL16EwWCARqNBly5d3J1Os6qrqwHYN9IlLi7O4eKIvVyx/k50dLTN08XJZDLExcUBuFRMMRqNrfYpKCiATCZDUFAQFAoFAgICUFtbi8rKSodzbsBiDBERERERERERERFRM0wmE7KysgBcGh3TUQsypaWlMBqN8Pb2RkRERIvPbShUhIWFISsry6ZChbOqqqogCALUajUCAgLs7l9UVAQPDw8kJiY2TsnWHLlcjh49esDX1xd6vR45OTk2baOgoACCIKBTp04IDAyEXC53yagYgMUYIiIiIiIiIiIiIqIWlZaWIisrC4IgICoqCgMHDkRoaKhoVIlMJoNGo0F4eDj69u3batHAlcxmM86cOQMAiI2NRVxcHDw9Pa2eo1arERYWhkGDBiEiIgKnT59GQUFB46iVtmQwGFBcXAwA6N69u6ggI5PJWhylU1JSgnPnzsHf3x+DBw9G586d4eXlZfUchUKBkJAQDBgwAEFBQTAajUhPT2+cIq01RqMRpaWl0Ol0CA8PhyAIyM/Pt/OVSrN/tRsiIiIiIiIiIiIiomtMfn4+6uvrERsbCx8fH3Tv3h3ApSKI0WiEXC6HSqVy67oyeXl5UCqV6NKlCyIiIhAREQGTyQSz2QylUtlYHDIajcjMzGxcR6W+vh5arbbN88vOzoaPjw+8vLzQu3dvmEwmmEwmKBQKKJVKFBQUNI5CknLu3DnU1dUhPj4esbGxiI2NhcVisdr/DSoqKnDy5EnU1tbalWNBQQECAwOh0+lQWloKg8Hg8Ou9HIsxREREREREREREREQ2KC8vx+HDhxEYGIiAgAD4+vrCw8MDarUaFosFer0edXV1qKysRGFhoc0jMlzp/PnzKCkpQXh4OPz8/KBWq6FSqaDX61FfX4+ioiIUFRXBZDI19mmPkTHApdExhw8fRufOnREYGAgvLy94eHjAZDKhoqICZWVlrcYoLCxEaWkpgoKCEBQUBE9PT3h4eEAQhMb1XYqLi1FSUuJQjsXFxTCbzVAoFC4bFQMAMkEQBJdFIyIiIiIiIiIiIiK6ghUXFyMjI8PdadD/Ex0djZiYGJw4ccJl67e0xMvLC4MHD4bJZMKePXvQWgklMTERgYGBrcblmjFEREREREREREREREQAQkJCAFwagePKsSwsxhAREREREREREREREQEIDg4GAJePwmExhoiIiIiIiIiIiIiIrnk6nQ5eXl6Na8+4EosxRERERERERERERER0zQsPDwcA5OXluTw2izFERERERERERERERHRN8/LyQlBQEMxmM/Lz810en8UYIiIiIiIiIiIiIiK6psXHx0MmkyE/Px8mk8nl8ZUuj0hERERERERERERERNQByeVyyGQymM1mAIBarUZcXBz8/f1hNBpx7ty5NtkuizFERERERERERERERHRN0Gq16Nu3L0wmEwRBgEqlgkwmg8lkQnp6OoxGY5tsVyYIgtAmkYmIiIiIiIiIiIiIrjDl5eXQ6/XuToP+H41GAx8fH1RUVKC+vt7peAqFAr6+vlAqlZDJZLBYLNDr9aipqYHFYrE7nqenJ3Q6XavPYzGGiIiIiIiIiIiIiIioDcndnQAREREREREREREREdHVjMUYIiIiIiIiIiIiIiKiNsRiDBERERERERERERERURtiMYaIiIiIiIiIiIiIiKgNsRhDRERERERERERERETUhliMISIiIiIiIiIiIiIiakMsxhAREREREREREREREbUhFmOIiIiIiIiIiIiIiIjaEIsxRP+XvTuPj6q6/z/+nslMFgJJSMgeFiEIiMgiIAp8CcgiiPtSsGKp+rUL1trWWtHWDe2vWivU2rrUpbhRBYsriIBAVJRFAVGUTRIIELJCQkjILOf3B9+ZGiHJTDJb4PV8PHi0TO495zN37rmR+55zLgAAAAAAAAAAQUQYAwAAAAAAAAAAEESEMQAAAAAAAAAAAEFEGAMAAAAAAAAAABBEhDEAAAAAAAAAAABBRBgDAAAAAAAAAAAQRIQxAAAAAAAAAAAAQUQYAwAAAAAAAAAAEESEMQAAAAAAAAAAAEFEGAMAAAAAAAAAABBEhDEAAAAAAAAAAABBRBgDAAAAAAAAAAAQRIQxAAAAAAAAAAAAQUQYAwAAAAAAAAAAEESEMQAAAAAAAAAA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OnbsaFJTU43FYvG+PnLkSLN79+5mj43nWD/99NPGGGO++uorc9pppzUYdxkZGd7PqqKi4oTtBHrMHjlyxEyfPr3Be4qOjjbp6ekmMzPTxMbGHjcep06d6t1/z549DY5rVFSUkWQyMjJOeNx/8IMfNFtTcySZ8847zxhjTH19vfnhD3/YYOxkZWV5x+r3P+eamhoza9asBtcezzUmMzPTdOrUqcFxPPvss01RUdEJ62gr1wZfHT161Nxzzz0N+mvsvJdkbr/99uPa8FyHu3bt6lOfdXV15vbbb29wjYqKijIZGRnHXae7d+9u3nnnHZ/abe153Zji4mJz9dVXN9gvPj7eZGRkGJvN1uC6s3LlSp9qRdtHGIMmnQz/mMHJ6/CKxWb3pLO9/+so2R/WehgvgO8YL4DvGC+A706G8fLcc88ZSebcc89tdtsFCxYYSebaa69t8PrPfvYzI8nMmzev2TbuvvtuI8n87ne/a3K7zZs3m7S0NCPJ9OrVy/zrX/8ypaWl3p/X1dWZt956ywwcONBIMikpKWbTpk1NtulrGPPBBx94b75ffvnlZvXq1cbpdHp/XlJSYp555hnTtWtXb4Dw7bffNtnmd8OYwsJCk5OTY6xWq7nyyivN4sWLzaFDh47b/sEHH/Te8Lv00kubbN8YY+655x4jydxwww3Nbvt9brfb/PznPzeSjM1mMz/96U/NmjVrGpzbO3bsMDNnzjTR0dFGkrnxxht9anv16tXem7jdu3c3zz77rCkrK2uwzY4dO8ycOXNMVlaWkWTuvPPOsIcxq1evNpdddpmRZPr06WOeeuops3PnzgbbVldXm//85z9mwIABRpJJSkoyhYWFTbbvOReioqJa9D4++OAD065dOyPJDB061CxYsMBUVVU1qOnll1823bt3N5LMaaed1uyNds+xnj17ttm7d6/35u3vfvc7s2vXLu92brfb7Nix44RtBHrMulwub2DZqVMn88ADD5ivvvqqwTnpdrtNQUGBefXVV8306dNNYmKieeihhxpt0zNmP/zwwyaPR2t8N3S97rrrjCSTl5dnli9f3qD20tLS40Kt+vp607lzZxMXF2euvvpq8/jjj5vt27c3CDeqqqrMa6+9Znr16mUkmQEDBpi6uroma4rUa4OvKisrTV5enjeYuvXWW01+fr6pr6/3blNfX2+2b99unn76aXPV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azVu3Dj179/f5/3OPvts9e3bV1VVVVq5cmVAakFkCu9vUgBoIVdZiczRo7LldJMkRWVky7lnV3iLAgAACDJ3XZ2cRQXhLiNiud1umfJy1R8+KKvV9+8e2nK6yerHzdRgGzVqlGJiYrRt2zbt3r37hN8Efu+99yQd+yb2iUycOFG33367Fi9erN///vcn3MYT9jTWhiS9++67kqRLL73Ur/dgt9s1ZMgQLV26VGvXrlXfvn392t+jsrJSkpSSkuLzPp5vax89etSn7c8991y/68rIyNC+fftUUVER0Bu8S5cuVX19vYYMGeL3N7U9N0fXrl17wp/n5+dLki6//HK/60pOTlb//v312Wef+b1voLT0c5KkioqKgNbidDr1/vvvS/J/bKSlpSk3N1fbt2/X+vXrNXr06Ea3jYmJ0cSJE/1qP1hj9tJLL9Xzzz+vRx99VNdcc406d+7sV/vh5u/xaKnk5GRJx2aRBFIwrw2+WrRokaRjQV+oLF++XNKx65avs0y+68orr9T//u//aufOndq1a9dxgW6gz+uWjj/p2Of01Vdfae3atbrwwgtbVQciF2EMgDbJubdAkmT/vzA0uMDUAAAgAElEQVTGlpGtunUfha8gAACAEHAWFejAL68NdxkRr9TP7dP/+pKic3sHpZaWaNeunc477zytWLFCS5cu1Q033NDg53V1dcrPz1e7du00YsSIE7Zx5plnKicnR2vWrFFlZaU6duzY4OdFRUXaunWrOnfurN69T/zey8vLtWPHDklqtJ+m9OrVS0uXLtXOnTv93tcjPj5ehw4dUlVVlfcmZ3M8N0E7derU7LY2m02nn36633W1b99ekgK+nMynn34qqeXHW5J2794tp9N53EyWDRs2SJLfs2I8evfuHdYw5owzzvB7n2B9Tps2bVJtba06duzYorp69eql7du3a+fOnU2GMWeddZZfN6CDOWYnT56syZMn65133tGwYcP097//PWQBRyAMGTIkJP14xl1dXV1A2w3mtcEXbrdba9askdSyYLSlPH16Zrn5Ky4uTv369dP69eu1Zs2a48KYQJ7XxhitW7dOUus+p9b8zkTkI4wB0CY59hRINrui0jIlHQtj3Icq5T5SI2u7+PAWBwAAECS2nG5K/+tL4S4jYrndbpWXlyslJcXvmTGRZvz48Y2GMStXrlRdXZ0mTZqkmJiY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InIckzFERETtmLZbLAQvn1qtypTsTEiR0ey1TkRERK2eFNEBltxTULIzYT5+BF4XXerpkIiIiIicwqcwRERE7ZggStAl9IZx/+6a15TsTLYoIyIiojahujKmcutGQCtDP+BiT4dERERE5BQmY4iIiNo5uVcyjAf3QLVYAABKdgaTMURERNQmiJHRsJaWoPL/voW+3yBovLw9HRIRERGRUyRXFygrK8P27duxe/dunDx5EiUlJTAajfD19UWHDh2QmJiI4cOHIyQkxB3xEhERkYN0ickoXfUuzCfToO0cAyUnC1JktKfDIiIiImpS9b9ZzMePwHfsRA9HQ0REROQ8p5Mx5eXlWLduHX788UcYDIaa1729veHj44OysjIcOHAABw4cwFdffYVx48ZhwoQJ0LA/PRERUYuSeyQBkgTj/l3Q+PgBipmVMURERNQm1LyBRKOB16Bhng2GiIiIyAVOJWMOHDiAxYsXo6CgADqdDiNGjMCAAQOQkJAAWZYBAGazGQcPHsQ333yDPXv24IsvvkBeXh7uv/9+t34CRERE1DiNXg85NgGm/buh7RQDAEzGEBERUZugCQiCoNNDjkuEGBDk6XCIiIiInOZwMkZVVXz66acoLCzEiBEjMGHCBPj7+9c5T6vVok+fPujTpw+++eYbrFq1Cps3b0ZiYiIuv/xytwRPRERE9tElJqNy0w/QJV8ICAKkiA6eDomIiIioSYIgwGfU9dAn9fd0KEREREQucTgZIwgCZs6ciZycHCQlJdl1zTXXXIO8vDz88MMPWLNmDVJSUtiujIiIqAXpeiWjbO0qGPdshxgWCUErezokIiIiIrsETZvl6RCIiIiIXOZURiQ0NNTuREy1G2+8EaIooqCgAOnp6c5sS0RERE6SE/sCAKq2bmSLMiIiIiIiIiKiFtZi5Sl+fn7o0aMHAOD48eMttS0REREBEP0DIXWOgWoyQopkMoaIiIiIiIiIqCW1aK+wkJAQAEBZWVlLbktEREQAdGeqY6SoaA9HQkRERERERER0fmnRZIyiKLZNOS+GiIioxel6JQMA25QREREREREREbWwFs2KFBUVAQCCg4NbclsiIiICoO83GNru8ZDjHZv7RkRERERERERErmmxZIzRaERaWhoAICYmpqW2JSIiojPEoBBELloNKSzS06EQERERERERuUQQBCxfvrzO67t3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Qant161bR3R0NKtXr+aNN96guLiY0NBQ+vXrx/79+2nZsiXXr1+3+We21Lx58xg6dChLly5l6dKlpKSkUKtWLcLDw3nttdeYPHkyHh4eNG/e3OI+16xZQ7du3QgLC7OqlrfeeuuB19zd3alTpw4RERFMnTqVCRMm0LBhwzL7MBgMzJ8/n+HDh7NkyRKWLl3KpUuX8PLyIjw8nLfffpupU6eWOsF5t6NHjzJ06NAKax4zZgxffPFFxT+cPHIGk8lkquoipPoyGo2kpKQQEhKCi4vVWwyJOBXlRcRyyouI5ZQXEcspLyKWU15ELPeo85KSkkL37t1xcXFh165dZS5NJiI1i75tRURERERERERERKqJkJAQtm3bRmZmJn369OHKlStVXZKIPASajBERERERERERERGpRsLDw9m4cSOXL1+mT58+XL16tapLEpFK0mSMiIiIiIiIiIiISDUTFRXFunXrSEpKom/fviQnJ1d1SSJSCZqMEREREREREREREamGhg8fTkxMDGPHjmXXrl1VXY6IVIJbVRcgIiIiIiIiIiIiIqUbMWIEI0aMqOoyRKSS9GSMiIiIiIiIiIiIiIiIHWkyRkRERERERERERERExI40GSMiIiIiIiIiIiIiImJHmowRERERERERERERERGxI03GiIiIiIiIiIiIiIiI2JEmY0REREREREREREREROxIkzEiIiIiIiIiIiIiIiJ2pMkYERERERERERERERERO9JkjIiIiIiIiIiIiIiIiB1pMkZERERERERERERERMSONBkjIiIiIiIiIiIiIiJiR5qMERERERERERERERERsSNNxkiF3N3dq7oEkRpDeRGxnPIiYjnlRcRyyouI5ZQXEcspLyJSWQaTyWSq6iJEREREREREREREREQclZ6MkXLdvn2bt956i9u3b1d1KSLVnvIiYjnlRcRyyouI5ZQXEcspLyKWU15E5GHQZIyUy2Qyce7cOfQAlUjFlBcRyykvIpZTXkQsp7yIWE55EbGc8iIiD4MmY0REREREREREREREROxIkzEiIiIiIiIiIiIiIiJ25Dp79uzZVV2EVG8uLi60atUKV1fXqi5FpNpTXkQsp7yIWE55EbGc8iJiOeVFxHLKi4hUlsGkxQ5FRERERERERERERETsRsuUiYiIiIiIiIiIiIiI2JEmY0RERERERERERERE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YcIEvL29LT6/0Wjkn//8J+vXry/ZVMzNzQ1fX997Nhpzd3dnzJgxDBkyxKpNX00mE9u2beOLL74oWd/Tzc0NPz8/8vPzyc3NLTm2RYsWTJkyRX+cOSDlpWInT55k5cqVXLlypeQ1d3d3fHx8AB6oPywsjMmTJ9OwYUOL65eawVHyUpalS5eya9cupkyZQu/evW3uJycnh5UrV7Jv376S17y8vPDw8ODWrVslr9WtW5dXX32V9u3bV6ZsqYaUldJt3LiRtWvXAlCnTh08PDxsruEPf/iDlpJxEMrLw2U+36xZs2jVqpXdzyePlvJiGY31BZQXS2isL+KYtAD0I5aXl1fyz9evX7frubp06UJERARxcXHs37+f1NRUMjIy8Pb2pkGDBkRGRhIdHU2zZs2s7tvFxYWRI0fSs2dPdu7cydGjR0lLSyM7O5u6desSGBhIp06d6Nmzp03rVBoMBgYNGkT37t358ccfOXjwICkpKWRmZuLp6UloaCjh4eF07dqVjh07Wt2/1AzKS8VatmzJn//8Z+Lj4zlw4ABJSUmkpaWRk5MDgLe3N8HBwYSFhdGtWzfCw8Otrl9qBkfJi735+PjwxhtvkJiYyM6dOzl16hTp6enk5eURHBxMaGgoXbt2pVu3bg9lICbVj7JSurs/l8zMzEr1VVxcXNlypJpQXkQsp7xYRmN9AeXFEhrrizgmPRkjIiIiIiIiIiIiIiJiR5avGyUiIiIiIiIiIiIiIiJW02SMiIiIiIiIiIiIiIiIHWkyRkRERERERERERERExI40GSMiIiIiIiIiIiIiImJHmowRERERERERERERERGxI03GiIiIiIiIiIiIiIiI2JEmY0REREREREREREREROxIkzEiIiIiIiIiIiIiIiJ2pMkYERERERERERERERERO9JkjIiIiIiIiIiIiIiIiB1pMkZERERERERERERERMSONBkjIiIiIiIiIiIiIiJiR5qMERERERERERERERERsSNNxoiIiIiIiIiIiIiIiNiRJmNERERERERERERERETsSJMxIiIiIiIiIiIiIiIidqTJGBERERERERERERERETvSZIyIiIiIiIiIiIiIiIgdaTJGRERERERERERERETEjv4/eOrVZxM9PQ8AAAAASUVORK5CYII=\n",
+                        "text/plain": [
+                            "<Figure size 1800x1200 with 1 Axes>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "chart.plot(df, style=style)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Using strings to make data requests\n",
                 "\n",
-                "###### fetch data from Quandl for BoE rate (using Bloomberg data)\n",
-                "if run_example == 1 or run_example == 0:\n",
-                "    # Monthly average of UK resident monetary financial institutions' (excl. Central Bank) sterling\n",
-                "    # Weighted average interest rate, other loans, new advances, on a fixed rate to private non-financial corporations (in percent)\n",
-                "    # not seasonally adjusted\n",
-                "    md_request = MarketDataRequest(\n",
-                "        start_date=\"01 Jan 2005\",  # start date\n",
-                "        data_source='quandl',  # use Quandl as data source\n",
-                "        tickers=['Weighted interest rate'],\n",
-                "        fields=['close'],  # which fields to download\n",
-                "        vendor_tickers=['BOE/CFMBJ84'],  # ticker (Bloomberg)\n",
-                "        vendor_fields=['close'],  # which Bloomberg fields to download\n",
-                "        cache_algo='internet_load_return',\n",
-                "        quandl_api_key=QUANDL_API_KEY)  # how to return data"
+                "We noted that we have predefined tickers already in our ticker mapping framework. We also showed how to use `MarketDataRequest` to download market data, whether it is predefined or not. Here we are downloading EURUSD data from Bloomberg with NY close, but rather than using a `MarketDataRequest` we just use a single string, which obviously has a lot less boilerplate code. By default it will select one week. Note for this section to work, you will need to run this on a machine with `blpapi` installed, and a Bloomberg Terminal subscription on there."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 7,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2021-05-04T16:36:54.375641Z",
+                    "start_time": "2021-05-04T16:36:52.637473Z"
+                }
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "            EURUSD.close\n",
+                        "Date                    \n",
+                        "2020-05-05        1.0840\n",
+                        "2020-05-06        1.0795\n",
+                        "2020-05-07        1.0834\n",
+                        "2020-05-08        1.0839\n",
+                        "2020-05-11        1.0807\n",
+                        "...                  ...\n",
+                        "2021-04-28        1.2126\n",
+                        "2021-04-29        1.2121\n",
+                        "2021-04-30        1.2020\n",
+                        "2021-05-03        1.2064\n",
+                        "2021-05-04        1.2013\n",
+                        "\n",
+                        "[261 rows x 1 columns]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "df = market.fetch_market(\"fx.bloomberg.daily.NYC.EURUSD.close\")\n",
+                "print(df)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "metadata": {},
+            "source": [
+                "Let's download intraday EURUSD data in the same way, which is a predefined ticker (underneath this will map to `vendor_tickers` for Bloomberg `EURUSD CMPN Curncy`."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2021-05-04T16:36:56.657212Z",
+                    "start_time": "2021-05-04T16:36:54.378641Z"
+                }
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "2019-11-02 16:11:20,240 - findatapy.market.datavendorweb - INFO - Request Quandl data\n",
-                        "2019-11-02 16:11:21,092 - findatapy.market.datavendorweb - INFO - Completed request from Quandl for ['Weighted interest rate.close']\n",
-                        "2019-11-02 16:11:23,201 - findatapy.market.ioengine - WARNING - Couldn't push MarketDataRequest_419__abstract_curve_key-None__category-None__category_key-backtest_default-cat_quandl_daily_NYC__cut-NYC__data_source-quandl__environment-backtest__expiry_date-NaT__fields-close__finish_date-2019-11-02 14:21:50_116819__freq-daily__freq_mult-1__gran_freq-None__resample-None__resample_how-last__start_date-2005-01-01 00:00:00__tickers-Weighted interest rate__trade_side-trade__vendor_fields-close__vendor_tickers-BOE_CFMBJ84 to Redis: Error 10061 connecting to 127.0.0.1:6379. No connection could be made because the target machine actively refused it.\n"
+                        "                           EURUSD.close\n",
+                        "Date                                   \n",
+                        "2021-04-27 16:37:00+00:00        1.2071\n",
+                        "2021-04-27 16:38:00+00:00        1.2072\n",
+                        "2021-04-27 16:39:00+00:00        1.2072\n",
+                        "2021-04-27 16:40:00+00:00        1.2072\n",
+                        "2021-04-27 16:41:00+00:00        1.2073\n",
+                        "...                                 ...\n",
+                        "2021-05-04 16:32:00+00:00        1.2015\n",
+                        "2021-05-04 16:33:00+00:00        1.2014\n",
+                        "2021-05-04 16:34:00+00:00        1.2015\n",
+                        "2021-05-04 16:35:00+00:00        1.2013\n",
+                        "2021-05-04 16:36:00+00:00        1.2012\n",
+                        "\n",
+                        "[7200 rows x 1 columns]\n"
                     ]
                 }
             ],
             "source": [
-                "    df = market.fetch_market(md_request)"
+                "df = market.fetch_market(\"fx.bloomberg.intraday.NYC.EURUSD.close\", start_date='week')\n",
+                "print(df)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Set style for graph, axis labels and plot"
+                "We can download arbitary tickers, which are not predefined too in our CSV files, using the `raw` keyword, and select whatever tickers we want. We haven't specified all the parameters like `freq` or `fields`, in which case the defaults we use. Here it would be `daily` and `close` on Bloomberg which corresponds to `PX_LAST`."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2021-06-01T11:44:11.043778Z",
+                    "start_time": "2021-06-01T11:44:09.307217Z"
+                }
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "            VIX.close\n",
+                        "Date                 \n",
+                        "2021-05-26  17.360001\n",
+                        "2021-05-27  16.740000\n",
+                        "2021-05-28  16.760000\n",
+                        "2021-06-01  17.150000\n"
+                    ]
+                }
+            ],
+            "source": [
+                "df = market.fetch_market(\"raw.data_source.bloomberg.tickers.VIX.vendor_tickers.VIX Index\", start_date='week')\n",
+                "\n",
+                "print(df)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Creates an object with essentially the same characteristics as a matplotlib graph."
+                "# Querying for predefined tickers\n",
+                "\n",
+                "We can also download all the tickers in our predefined tickers list (which are defined in our CSV files), which has this format, and will likely contain many tickers.\n",
+                "\n",
+                "`category.data_source.freq.cut`\n",
+                "\n",
+                "We can also specify individual predefined tickers and fields as follows:\n",
+                "\n",
+                "`category.data_source.freq.cut.tickers.fields`\n",
+                "\n",
+                "Let's get all the predefined tickers/categories, which are from `quandl` and a few from `bloomberg`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 3,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2021-05-04T17:05:47.233735Z",
+                    "start_time": "2021-05-04T17:05:47.220735Z"
+                }
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "['fx.quandl.daily.NYC', 'fx-spot-volume.quandl.daily.LOC']\n",
+                        "['fx.bloomberg.daily.BGN', 'fx.bloomberg.daily.BSTP', 'fx.bloomberg.daily.NYC', 'fx.bloomberg.daily.TOK', 'fx.bloomberg.daily.LDN', 'fx.bloomberg.daily.10AM', 'fx-tot.bloomberg.daily.NYC', 'fx-tot-forwards.bloomberg.daily.NYC', 'fx.bloomberg.intraday.NYC', 'fx.bloomberg.intraday.BGNE']\n"
+                    ]
+                }
+            ],
+            "source": [
+                "from findatapy.util import ConfigManager\n",
+                "cm = ConfigManager().get_instance()\n",
+                "\n",
+                "# Get all the categories for raw data (note this won't include generated categories like fx-vol-market,\n",
+                "# which aggregate from many other categories)\n",
+                "categories = list(cm.get_categories_from_tickers())\n",
+                "\n",
+                "# Filter those categories which include quandl\n",
+                "quandl_category = [x for x in categories if 'quandl' in x]\n",
+                "print(quandl_category)\n",
+                "\n",
+                "# Filter those categories which include bloomberg and print the first few\n",
+                "bloomberg_category = [x for x in categories if 'bloomberg' in x][0:10]\n",
+                "print(bloomberg_category)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "style = Style()"
+                "Let's download all the tickers in the category/data_source/freq/cut for `fx.quandl.daily.NYC`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 11,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2021-05-04T16:36:59.346197Z",
+                    "start_time": "2021-05-04T16:36:58.401542Z"
+                }
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "            EURUSD.close  GBPUSD.close  AUDUSD.close  NZDUSD.close  \\\n",
+                        "Date                                                                 \n",
+                        "2020-05-05        1.0844        1.2449        0.6458        0.6065   \n",
+                        "2020-05-06        1.0806        1.2347        0.6414        0.6019   \n",
+                        "2020-05-07        1.0815        1.2349        0.6500        0.6086   \n",
+                        "2020-05-08        1.0854        1.2436        0.6543        0.6147   \n",
+                        "2020-05-11        1.0818        1.2330        0.6472        0.6065   \n",
+                        "\n",
+                        "            USDCAD.close  USDCHF.close  USDNOK.close  USDSEK.close  \\\n",
+                        "Date                                                                 \n",
+                        "2020-05-05        1.4025        0.9721       10.2603        9.8296   \n",
+                        "2020-05-06        1.4143        0.9745       10.2799        9.8486   \n",
+                        "2020-05-07        1.3972        0.9746       10.2274        9.8128   \n",
+                        "2020-05-08        1.3910        0.9699       10.1864        9.7590   \n",
+                        "2020-05-11        1.4024        0.9722       10.2850        9.8649   \n",
+                        "\n",
+                        "            USDJPY.close  \n",
+                        "Date                      \n",
+                        "2020-05-05    106.519997  \n",
+                        "2020-05-06    106.070000  \n",
+                        "2020-05-07    106.360001  \n",
+                        "2020-05-08    106.500000  \n",
+                        "2020-05-11    107.699997  \n"
+                    ]
+                }
+            ],
+            "source": [
+                "try:\n",
+                "    import os\n",
+                "    QUANDL_API_KEY = os.environ['QUANDL_API_KEY']\n",
+                "except:\n",
+                "    QUANDL_API_KEY = 'TYPE_YOUR_KEY_HERE'\n",
+                "\n",
+                "df = market.fetch_market(md_request_str=\"fx.quandl.daily.NYC\", start_date='year',\n",
+                "                         md_request=MarketDataRequest(quandl_api_key=QUANDL_API_KEY))\n",
+                "print(df.head(5))"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "metadata": {},
+            "source": [
+                "We can also query this category combination too for all available tickers/fields/vendor tickers."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 17,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2021-05-04T16:41:51.164251Z",
+                    "start_time": "2021-05-04T16:41:51.149255Z"
+                }
+            },
             "outputs": [
                 {
-                    "ename": "SyntaxError",
-                    "evalue": "invalid syntax (<ipython-input-25-81e8e8912071>, line 1)",
-                    "output_type": "error",
-                    "traceback": [
-                        "\u001b[1;36m  File \u001b[1;32m\"<ipython-input-25-81e8e8912071>\"\u001b[1;36m, line \u001b[1;32m1\u001b[0m\n\u001b[1;33m    Setting styles above.\u001b[0m\n\u001b[1;37m                 ^\u001b[0m\n\u001b[1;31mSyntaxError\u001b[0m\u001b[1;31m:\u001b[0m invalid syntax\n"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "For category fx.quandl.daily.NYC\n",
+                        "tickers = ['EURUSD', 'GBPUSD', 'AUDUSD', 'NZDUSD', 'USDCAD', 'USDCHF', 'USDNOK', 'USDSEK', 'USDJPY']\n",
+                        "vendor_tickers = ['FRED/DEXUSEU', 'FRED/DEXUSUK', 'FRED/DEXUSAL', 'FRED/DEXUSNZ', 'FRED/DEXCAUS', 'FRED/DEXSZUS', 'FRED/DEXNOUS', 'FRED/DEXSDUS', 'FRED/DEXJPUS']\n",
+                        "fields = ['close']\n"
                     ]
                 }
             ],
             "source": [
-                "Setting styles above."
+                "# For this category, get all the tickers, vendor_tickers and fields which are available\n",
+                "tickers = cm.get_tickers_list_for_category_str(categories[0])\n",
+                "fields = cm.get_fields_list_for_category_str(categories[0])\n",
+                "vendor_tickers = cm.get_vendor_tickers_list_for_category_str(\"fx.quandl.daily.NYC\")\n",
+                "\n",
+                "# We don't need to add the environment (eg. backtest)\n",
+                "print(\"For category \" + quandl_category[0])\n",
+                "print(\"tickers = \" + str(tickers))\n",
+                "print(\"vendor_tickers = \" + str(vendor_tickers))\n",
+                "print(\"fields = \" + str(fields))"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Let's download EURUSD from Quandl, using our predefined mapping."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 13,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2021-05-04T16:36:59.692074Z",
+                    "start_time": "2021-05-04T16:36:59.363195Z"
+                }
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "            EURUSD.close\n",
+                        "Date                    \n",
+                        "2020-05-05        1.0844\n",
+                        "2020-05-06        1.0806\n",
+                        "2020-05-07        1.0815\n",
+                        "2020-05-08        1.0854\n",
+                        "2020-05-11        1.0818\n"
+                    ]
+                }
+            ],
+            "source": [
+                "df = market.fetch_market(md_request_str=\"fx.quandl.daily.NYC.EURUSD\", start_date='year',\n",
+                "                         md_request=MarketDataRequest(quandl_api_key=QUANDL_API_KEY))\n",
+                "print(df.head(5))"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "metadata": {},
+            "source": [
+                "We can extract the `vendor_tickers` for our predefined ticker, not just for large categories."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 18,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2021-05-04T16:42:00.631540Z",
+                    "start_time": "2021-05-04T16:42:00.622540Z"
+                }
+            },
             "outputs": [
                 {
-                    "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAABnAAAARlCAYAAACJAYkzAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAPYQAAD2EBqD+naQAAADh0RVh0U29mdHdhcmUAbWF0cGxvdGxpYiB2ZXJzaW9uMy4xLjEsIGh0dHA6Ly9tYXRwbG90bGliLm9yZy8QZhcZAAAgAElEQVR4nOzdeVyU1f4H8M8M+zLsq7jgCuIGLrmjYHbTNLcsTU1bvJUtmi23LEvTLL1leW0xt9t2sywXrqXlLoY7iLsiKqKsArIMg8zAPL8//MFleJ6BWWHAz/v1mlfNmTnf5zwzhwGf75zzlQmCIICIiIiIiIiIiIiIiIhshryxB0BERERERERERERERES6mMAhIiIiIiIiIiIiIiKyMUzgEBERERERERERERER2RgmcIiIiIiIiIiIiIiIiGwMEzhEREREREREREREREQ2hgkcIiIiIiIiIiIiIiIiG8MEDhERERERERERERERkY1hAoeIiIiIiIiIiIiIiMjGMIFDRERERERERERERERkY5jAISIiImpmZsyYAZlMpnObMWNGYw/LLM3xnO51tvKepqWlicYhk8mQlpbW4GMhIiIiIiKqiQkcIiIiIiIiIiIiIiIiG8MEDhERNZr9+/dLfuvZkJudnR28vLzQpk0bREVFYdq0afj000+RmJjY2KdlNd98843Jr5extwULFjT26RIRERERERER3dPsG3sAREREptBqtSgqKkJRURHS09ORnJyMH374AQAQERGBmTNnYtasWXB0dGzkkRJRc5WcnIytW7fqtHl5eWHOnDmNNCKi//nss89QWFio0zZ27FhERkY20oioqVu+fDmKi4t12saPH4/u3bs30oho/fr1SE9P12mLjY1FdHR0I42IiIiILI0JHCIianbOnz+PV155BatXr8aaNWswcODAxh4SETVDycnJWLhwoU5bmzZtmMAhm/DZZ5/h+vXrOm2hoaFM4JDJli9fjoyMDJ22Dh06MIHTiNavX4+EhASdNnt7eyZwiIiImhFuoUZERM3WhQsXEBsbi99++62xh0JERERERERERGQUrsAhIiKbExMTg9jY2Dqfo1arUVxcjPT0dCQlJYm+ZVzzeRMmTMCBAwfQr18/awy30Y0fPx5RUVEWjclvbhIRERERERERNS4mcIiIyOZER0fjnXfe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KpGWlqaz5ZwpsrKy0Lp1a52aO5mZmWbFlCITBEGweFQiIiIiIiIiIiIiIhuVn5+Ps2fPGvRcV1fX6u3S7O3todVqodFoUFZWBqVSadGaJ5bi4OAAT09PODk5wc7ODmq1Gmq1GsXFxUbXfLFFQ4YMqf7/wsJCnDp1SufxqvfM0dERMpkMarUaJSUlKCsrs8jx7ezs0L9//+pkk1qtxpEjR2BIusXDwwPh4eFwcXGp97lcgUNEREREREREREREpEdVPZWmRKPRIC8vr7GH0Wis/Z4FBgbqrBTKzs42KHljLHn9TyEiIiIiIiIiIiIiIiIACA4Orv5/QRCQlZVlleMwgUNERERERERERERERGQAHx8fnRo7+fn5uHPnjlWOxQQOERERERERERERERFRPeRyOdq1a6fTdvPmTasdjzVwiIiIiIiIiIiIiIiIanFycgIA2NnZwdXVFa1bt4abm1v14wUFBSgqKrLa8ZnAISIiIiIiIiIiIiIiqqVfv356H6usrERqaqpVj88EDhERERERERERERHdU+RyOdq0adPYwyALcHZ2bvD3UqvVIi8vDwEBAUb3dXBwgEwmM+i5MkEQBKOPQERERERERERERETURAmCAK1W29jDIBPZ2dlV/78138vax6n6r7lpFblcblAShwkcIiIiIiIiIiIiIiIiGyNv7AEQERERERERERERERGRLiZwiIiIiIiIiIiIiIiIbAwTOERERERERERERERERDaGCRwiIiIiIiIiIiIiIiIbwwQOERERERERERERERGRjWECh4iIiIiIiIiIiIiIyMYwgUNERERERERERERERGRjmMAhIiIiIiIiIiIiIiKyMUzgEBERERERERERERER2RgmcIiIiIiIiIiIiIiIiGwMEzhEREREREREREREREQ2hgkcIiIiIiIiIiIiIiIiG8MEDhERERERERERERERkY1hAoeIiIiIiIiIiIiIiMjGMIFDRERERERERERERERkY5jAISIiIiIiIiIiIiIisjFM4BAREREREREREREREdkYJnCIiIiIiIiIiIiIiIhsDBM4RERERERERERERERENoYJHCIiIiIiIiIiIiIiIhvDBA4R0f+xd+fxUVX3/8ffk5kJIWSBBEIgQYJsgXxFQFkFA7ig7G6AotVqa7H1p19trbZupe7V2qpYbbWuFYtVpGLBlUVZ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FPXu3VsDBgxo0WUim6Oqqkpr167VoUOHlJubK0k666yzdOmll9Zbx+Fw6Pvvv9euXbuUl5en48ePq3379urUqZN69+6tYcOGqX379qF6Co0K5vXRXFVVVdq4caMOHDigwsJCnThxQjExMUpNTVVGRob69+/f7M9RXxQWFmrNmjXKy8vz/M3t0qWLBg8e3Oy/c6EYQ3v37tWWLVtUUFCg4uJidezYUcnJyRo9erSSk5ObFT/aOAPwg8vlMnJycgyXy9XSoQD1qtiywfhh0jnGkbt+YuTefl1Lh8O4AZqAcQM0DWMHrc2TTz5pSPL8XHHFFY3WSU9P95SfN2+eYRiGsXz5cs85q9VqFBcXN9jG448/bup30qRJPo+bkydPGs8995wxcOBAUxu1f9LT042///3vhtPp9KndZcuWmeo/9thjPtUzDMN4++23jf79+9cby7Bhw4xFixZ5yo8YMcLzWLt27Rps++677za1tW7dOsMwDKO8vNy45557jKSkJK99RkREGJdffrmxe/fuBtuvGYs/P768Ph9++KGRmZlp2Gy2ettJSkoy7r333kavGW+cTqfx9NNPG927d/fats1mM6ZOnWps3rzZMAzDqKioMD0+ceJEv/tszAsvvGDq4+233663bEPxrFq1yhg/frxhsVi8Prfu3bsbjz76aIPXd+1r2tefxq5JwzCM/Px8484776z3ta/+LMjMzDRWrFjh8+s3a9YsUxu5ubmGYRjG/v37jdmzZxvR0dF1+pk1a1aDbX733XfGrFmzjNjY2HpjjY6ONubMmWPs3bvX51gNwzBycnKMW265xUhISGj0dY2JiTEuueQS480336zTTjDHoS/q+5wpKCgwbr75ZqNTp051+h4xYkSddrKzs40//elPxgUXXOD1var5Y7fbjenTpxtr1671Oz5ff2qPcW//Tgvm9dFca9asMaZNm9boa9m1a1fjpptuMtavX19vW/WNLV/8+9//NkaOHGlERETUG0NaWprx2GOPGeXl5X49x0CNofqUlpYav//9741evXo12PY555xj+jsN1EQCB37hpgBag9Il7xg/TBthFL/1NyN71oSWDodxAzQB4wZoGsYOWptNmzaZbmB07tzZcLvd9ZbPzc01lV+5cqVhGKeSCZGRkZ7zS5YsabDfiRMnmtp5+OGHfRo369atM3r27OnXDbxhw4b5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rXlz/sEHHzQ99sknn5hubh07dsxrG48++qipv5kzZzY4bhwOR52kgC/LBp08edKYPHmyqd7ChQvrLe9PAic3N9do166dqfxf/vKXRuO55JJLTHWaksCRZPTo0aPem+zV1qxZY7qBFRcX1+DeBIFYXqx2YmX69OlGRUVFo/UeeeQRU71bbrml3rKrV6+uc3Pz448/brD9bdu2ed1fIdwSONU/DzzwQIN9uN1ur8sQNqS+PU58tXv3btM13759e59uYOfk5JiWPbTb7V4TPtVq32SWZPTr18+v/TreeOMNU/0+ffo02Ge1FStWmG7SDxw40OuSklVVVabX4n/+5398Wh6uWrDHYVN4+5xJSkoydu7c6Vc73pJpDfnwww9NS5j58nz9WYKyNpfLZTzzzDNBvT6a44477jDF1rFjR2PVqlU+129onPiTwFm4cKGprN1uNz788MMG+z506JCRlpZmqnfttdd6LRvMMXTs2DFP0r763yP/+Mc/Gm2zpKTEOOecc0zxb9iwweeY0LaxhBqANsVdWSFXQZ7sqWmKiImTpUOMnLnZLR0WAABoAndlpZzZWS0dRptjS01TRFRUS4fhUXu5qi+++EKGYchisZjO5+bmmpZ0GTdunOnx8847T3a7XQ6HQ263W1988YWmTZtWp7+ay7B5a6e2f/7zn6Z+f/SjH/m0dE1kZKTeeustnXnmmTp69Kgk6amnntLMmTMbrduYl156ybSM1WWXXaZbbrml0XjeeOMNDRgwwLS0VFO89dZb6tmzZ4NlRo8ercmTJ+vDDz+UdGrZsU2bNmns2LHN6rs+WVlZeuONNzzH/fr108KFC9WuXbtG6/72t7/V8uXL9fnnn0uSXnvtNT300ENKTEysU/aZZ54xHd911126+OKLG2w/IyNDzz77rK699lpfnkqLuuCCC/S73/2uwTIWi0UPPfSQafm+5cuX69577w1aXE888YTpmn/++ec1YcKERut1795db775ps4//3xJp5agevbZZ+ssw1Yfi8WiN9980+flD91utx5++GHPcWRkpJYsWaLU1NRG644bN0733XefHnjgAUmnlnhatmyZJk2aZCqXl5dnei2mT58uu93uU3zSqSWoWoP58+erf//+ftVJS0vzq/zkyZN144036uWXX5YkffzxxyosLFTnzp39asdXbrfb9BkSjOujqfLz8/Xiiy+azr366queseOLQC0T+vTTT5uOf/3rX2vy5MkN1klNTfWMdcMwJEkLFy7U448/rpSUFFPZYI6h+fPnm/7G3nfffZozZ06jbcbFxXmWpKxesvGpp57SO++843NcaLtI4ABoU5w5ByWdujFhsVhkS06VMy+nkVoAACAcObOzdOT28L/h2dp0feYfiuyT3tJheAwaNEgJCQmeJEdRUZG+/fZbnX322aZyNRMv7dq18+x/Uy06Olrnnnuu1q1bJ+nUPji1EzgOh6PO/jeN7Xfy7LPPen6PiIjQo48+6tsT06l9V2666SY9+eSTkk7th5OXl9fsm1xvv/226fi+++7zqV6XLl00d+5cPfLII03uOzMz0+ckzJQpUzwJHEnasmVL0BI4f/nLX0z7E8ybN8+n5E21O++805PAqaio0KeffqrZs2ebyhw/flyLFy/2HEdHR+vuu+/2qf05c+bokUce0Y4dO3yOqSXcd999dZKn3pxzzjlKSkpSfn6+pFPvbbAUFxfrzTff9Bynp6frhhtu8Ln+2LFjNWzYMG3cuFGS9MEHH/icwJkwYYKGDx/uc18fffSRKeH74x//WOnpvn8CQhUnAAAgAElEQVTe3nbbbXrooYc8N3A/+OCDRm/QV78HbUmfPn105ZVXhqSvK664wpPAkaR169Zp6tSpQenro48+0v79+z3Hobg+fPXaa6959tqRpIkTJ2rGjBkBadsfO3fu1IYNGzzHsbGx+s1vfuNT3TFjxpi+OOBwOPTWW2/p17/+dYP1AjWGDMPQ/PnzPccdO3b0a6+iM888UzNmzNC//vUvSaf2w3E6nbLZuH1/uuMKANCmOLNPJXDsqae+EWjrlipnHjNwAABojWypaer6zD9aOow2x5aa1tIhmFgsFmVmZur999/3nFu5cmWdBE7NzZ5HjBihKC+ziDIzMz0JnNozbaRTCZQTJ054jlNSUtSvXz/l5eV5ja24uFibN2/2HI8ZM6bON3kbM378eE8CRzq1KfpVV13lVxs1HTt2TDt37vQc9+7dW0OHDvW5/syZM5uVwGnsW9A1DRgwwHQczBvNn376qef3du3a+X3jsfZMrC+//LJOAmfDhg2eG6fSqQRVbGysz31cc801uv/++/2KK5RiY2P9SrD16dPH854eO3YsaDcaV61aZdpofObMmT4lmWoaP368J4Gza9cu5efn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pw/z4n0A0Eo5DmVJktcZOBHtoxXRMVHOPGbgAAAAhLvx48fX2YRYMu9r44vMzEw999xzXttviksvvVQbN27U7NmzTd+Sdjqd+vrrr/X111832kagZ2BceumlWr58uX7yk5/o+++/b7Ds0KFD9c4776h3796mmSKxsbEBjak5evbsqQULFuhHP/qR30vUVevVq5c2bdqkn/70p3rnnXdMj+3du1d79+5ttI3G3qe4uDgtX77cc01UKysr02effVanvNVq1fz5803755yOnnzySe3bt08fffRRk9t44IEHNGTIEN10000qKCjwnD9x4oTPSz3V3o8nGNq1a6clS5bokUce0UMPPWRaPik/P7/RZfekU8tt1ZxV0pCTJ0/69Bk0btw4vfvuu/UunyYFZhy2hPvvv1/79u0zLYHodDq1fv16rV+/vk75pKQkLV682O/PZYvFonfffVdTpkzRnj17mhRrqK8Pf/To0UPr16/XddddV2dpt+3bt2v79u0B79Obzp07a82aNbryyiu1fPlyz/ny8nLTcW0pKSl6//33NWzYML/6C+QYkk7NxBswYIDmzJmjAwcOmPrZsGGDTzGdzrM2YcYSagDaBGfOQVkTuygiuoPXx23JKSyhBgAA0ArUl2DxZ9kzSTr//PM9++D40r4v+vfvr6+//lrvv/++xo8f73UT8NoyMjJ0++23a+3atXr77beb3Hd9Ro0apa1bt2rBggW64oordOaZZyo6Olrx8fEaMGCAZs2apQ8//FAbNmxQ7969JUnFxcWe+vHx8QGPqTmmT5+uXbt26Q9/+IMuueQS9ezZUzExMYqI8P32RVxcnBYuXKjNmzfr6quv9uk5pqam6rrrrtOiRYu8LuFVW2JiotatW6c//vGP6t69u9cyVqtVkyZN0tq1azV37lyf42+r2rdvr2XLlunjjz/WT37yEw0dOlSJiYk+jaOapk6dqqysLD3zzDM666yzvI7zmiIjIzVmzBg99NBD2rdvX8jeC4vFovvuu08HDhzQr371K/Xo0aPROnFxcZoyZYpefPFF5eXladCgQXXKTJ06Ve+++65+/OMfm/bnqk9ERIQyMzO1cOFCrVixQomJiY3WCcQ4DDWLxaLXX39dr776aoOvS9euXXX77bdr27ZtGjVqVJP66tevn7755hu9/vrruuqqq5Senq74+Pg6m9w3Fm8w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\n",
-                        "text/plain": [
-                            "<Figure size 1800x1200 with 1 Axes>"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "FRED/DEXUSEU\n"
+                    ]
                 }
             ],
             "source": [
-                "style.title = 'BoE weighted interest rate'\n",
-                "style.scale_factor = 3\n",
-                "style.file_output = \"boe-rate.png\"\n",
-                "style.source = 'Quandl/BoE'\n",
+                "vendor_tickers = cm.convert_library_to_vendor_ticker_str(\"fx.quandl.daily.NYC.EURUSD\")\n",
                 "\n",
-                "chart.plot(df, style=style)"
+                "print(vendor_tickers)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "We can convert from our predefined fields to the vendor field. Here we show that our `close` field for `bloomberg` is `PX_LAST` on Bloomberg."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 21,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2021-05-04T16:42:34.354010Z",
+                    "start_time": "2021-05-04T16:42:34.348012Z"
+                }
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "PX_LAST\n"
+                    ]
+                }
+            ],
+            "source": [
+                "vendor_fields = cm.convert_library_to_vendor_field('bloomberg', 'close')\n",
+                "print(vendor_fields)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
@@ -201,13 +608,26 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.4"
+            "version": "3.8.8"
+        },
+        "toc": {
+            "base_numbering": 1,
+            "nav_menu": {},
+            "number_sections": true,
+            "sideBar": true,
+            "skip_h1_title": false,
+            "title_cell": "Table of Contents",
+            "title_sidebar": "Contents",
+            "toc_cell": false,
+            "toc_position": {},
+            "toc_section_display": true,
+            "toc_window_display": false
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/fx_forwards_indices_examples.py` & `finmarketpy-0.11.9/finmarketpy_examples/fx_forwards_indices_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,17 +104,17 @@
 
     df_bbg_tot_forwards = market.fetch_market(md_request)
     df_bbg_tot_forwards.columns = [x + '-bbg' for x in df_bbg_tot_forwards.columns]
 
     # Combine into a single data frame and plot, we note that the Cuemacro constructed indices track the Bloomberg
     # indices relatively well (both from spot and forwards). Also note the large difference with spot indices
     # CAREFUL to fill down, before reindexing because forwards indices are likely to have different publishing dates
-    df = calculations.pandas_outer_join([pd.DataFrame(df_cuemacro_tot_1M[cross + '-forward-tot-1M-cuemacro.close']),
+    df = calculations.join([pd.DataFrame(df_cuemacro_tot_1M[cross + '-forward-tot-1M-cuemacro.close']),
                                          pd.DataFrame(df_cuemacro_tot_3M[cross + '-forward-tot-3M-cuemacro.close']),
-                                         df_bbg_tot, df_spot, df_bbg_tot_forwards]).fillna(method='ffill')
+                                         df_bbg_tot, df_spot, df_bbg_tot_forwards], how='outer').fillna(method='ffill')
 
     df = calculations.create_mult_index_from_prices(df)
 
     chart.plot(df)
 
 ###### Create total return indices plot for AUDJPY using the underlying USD legs (ie. AUDUSD & JPYUSD)
 if run_example == 2 or run_example == 0:
@@ -167,13 +167,13 @@
 
     df_bbg_tot_forwards = market.fetch_market(md_request)
     df_bbg_tot_forwards.columns = [x + '-bbg' for x in df_bbg_tot_forwards.columns]
 
     # Combine into a single data frame and plot, we note that the Cuemacro constructed indices track the Bloomberg
     # indices relatively well (both from spot and forwards). Also note the large difference with spot indices
     # CAREFUL to fill down, before reindexing because forwards indices are likely to have different publishing dates
-    df = calculations.pandas_outer_join([pd.DataFrame(df_cuemacro_tot_1M[cross + '-forward-tot-1M-cuemacro.close']),
-                                         df_bbg_tot, df_spot, df_bbg_tot_forwards]).fillna(method='ffill')
+    df = calculations.join([pd.DataFrame(df_cuemacro_tot_1M[cross + '-forward-tot-1M-cuemacro.close']),
+                                         df_bbg_tot, df_spot, df_bbg_tot_forwards], how='outer').fillna(method='ffill')
 
     df = calculations.create_mult_index_from_prices(df)
 
     chart.plot(df)
```

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/fx_forwards_pricing_examples.py` & `finmarketpy-0.11.9/finmarketpy_examples/fx_forwards_pricing_examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,9 +118,9 @@
                                    data_source='bloomberg', cut='NYC',
                                    tickers=tickers,
                                    vendor_tickers= [x + " CMPN Curncy" for x in tickers],
                                    cache_algo='cache_algo_return')
 
     implied_depo_bbg_df = market.fetch_market(md_request=md_request)
 
-    chart.plot(calculations.pandas_outer_join([implied_depo_bbg_df, implied_depo_df]))
+    chart.plot(calculations.join([implied_depo_bbg_df, implied_depo_df]), how='outer')
```

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/fx_options_indices_examples.py` & `finmarketpy-0.11.9/finmarketpy_examples/fx_options_indices_examples.py`

 * *Files 11% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         df_list.append(pd.DataFrame(df_option_tc[cross + '-option-tot-with-tc.close']))
         df_list.append(pd.DataFrame(df_option_tc[cross + '-option-delta-tot-with-tc.close']))
         df_list.append(pd.DataFrame(df_option_tc[cross + '-delta-pnl-index-with-tc.close']))
 
     if df_spot_tot is not None:
         df_list.append(df_spot_tot)
 
-    df = calculations.pandas_outer_join(df_list).fillna(method='ffill')
+    df = calculations.join(df_list, how='outer').fillna(method='ffill')
 
     return calculations.create_mult_index_from_prices(df)
 
 ###### Fetch market data for pricing AUDUSD options in 2007 (ie. FX spot, FX forwards, FX deposits and FX vol quotes)
 ###### Construct volatility surface using FinancePy library underneath, using polynomial interpolation
 ###### Enters a long 1M call, and MTM every day, and at expiry rolls into another long 1M call
 if run_example == 1 or run_example == 0:
@@ -82,87 +82,102 @@
 
     # Download the whole all market data for AUDUSD for pricing options (FX vol surface + spot + FX forwards + depos)
     md_request = MarketDataRequest(start_date=start_date, finish_date=finish_date,
                                    data_source='bloomberg', cut='BGN', category='fx-vol-market',
                                    tickers=cross, fx_vol_tenor=['1W', '1M', '3M'],
                                    cache_algo='cache_algo_return', base_depos_currencies=[cross[0:3], cross[3:6]])
 
-    df = market.fetch_market(md_request)
-    df = df.fillna(method='ffill')
+    df_vol_market = market.fetch_market(md_request)
+    df_vol_market = df_vol_market.fillna(method='ffill')
 
     # Remove New Year's Day and Christmas
-    df = Filter().filter_time_series_by_holidays(df, cal='FX')
+    df_vol_market = Filter().filter_time_series_by_holidays(df_vol_market, cal='FX')
+
+    # Get a total return index for trading spot
+    # This way we can take into account carry when calculating delta hedging P&L
+    md_request = MarketDataRequest(start_date=start_date, finish_date=finish_date,
+                                   data_source='bloomberg', cut='NYC', category='fx-tot',
+                                   tickers=cross,
+                                   cache_algo='cache_algo_return')
+
+    df_tot = market.fetch_market(md_request)
+
+    df_vol_market = df_vol_market.join(df_tot, how='left')
+    df_vol_market = df_vol_market.fillna(method='ffill')
 
     # We want to roll long 1M ATM call at expiry
-    # We'll mark to market the price through the month by interpolating between 1W and 1M (and using whole vol curve
+    # We'll mark to market the option price through the month by interpolating between 1W and 1M (and using whole vol curve
     # at each tenor)
     fx_options_curve = FXOptionsCurve(fx_options_trading_tenor=fx_options_trading_tenor,
         roll_days_before=0,
         roll_event='expiry-date',
         roll_months=1,
         fx_options_tenor_for_interpolation=['1W', '1M'],
         strike='atm',
         contract_type='european-call',
         depo_tenor_for_option='1M',
         position_multiplier=1.0,
+        tot_label='tot',
         output_calculation_fields=True)
 
     # Let's trade a long 1M call, and we roll at expiry
-    df_cuemacro_option_call_tot = fx_options_curve.construct_total_return_index(cross, df)
+    df_cuemacro_option_call_tot = fx_options_curve.construct_total_return_index(cross, df_vol_market)
 
     # Add transaction costs to the option index (bid/ask bp for the option premium and spot FX)
-    df_cuemacro_option_call_tc = fx_options_curve.apply_tc_to_total_return_index(cross, df_cuemacro_option_call_tot,
+    df_cuemacro_option_call_tc = fx_options_curve.apply_tc_signals_to_total_return_index(cross, df_cuemacro_option_call_tot,
                                                                             option_tc_bp=5, spot_tc_bp=2)
 
     # Let's trade a long 1M OTM put, and we roll at expiry
     df_cuemacro_option_put_tot = fx_options_curve.construct_total_return_index(
-        cross, df, contract_type='european-put', strike='10d-otm', position_multiplier=1.0)
+        cross, df_vol_market, contract_type='european-put', strike='10d-otm', position_multiplier=1.0)
 
     # Add transaction costs to the option index (bid/ask bp for the option premium and spot FX)
-    df_cuemacro_option_put_tc = fx_options_curve.apply_tc_to_total_return_index(cross, df_cuemacro_option_put_tot,
+    df_cuemacro_option_put_tc = fx_options_curve.apply_tc_signals_to_total_return_index(cross, df_cuemacro_option_put_tot,
                                                                                  option_tc_bp=5, spot_tc_bp=2)
 
 
     # Get total returns for spot
-    md_request.abstract_curve = None
-
-    # Get Bloomberg calculated total return indices (for spot)
-    md_request.category = 'fx-tot'
-    md_request.cut = 'NYC'
-
-    df_bbg_tot = market.fetch_market(md_request)
+    df_bbg_tot = df_tot # from earlier!
     df_bbg_tot.columns = [x + '-bbg' for x in df_bbg_tot.columns]
 
     # Calculate a hedged portfolio of spot + 2*options (can we reduce drawdowns?)
     calculations = Calculations()
 
     ret_stats = RetStats()
 
-    df_hedged = calculations.pandas_outer_join([df_bbg_tot[cross + '-tot.close-bbg'].to_frame(), df_cuemacro_option_put_tc[cross + '-option-tot-with-tc.close'].to_frame()])
+    df_hedged = calculations.join([df_bbg_tot[cross + '-tot.close-bbg'].to_frame(), df_cuemacro_option_put_tc[cross + '-option-tot-with-tc.close'].to_frame()], how='outer')
     df_hedged = df_hedged.fillna(method='ffill')
     df_hedged = df_hedged.pct_change()
 
-    df_hedged['Spot + 2*option hedge'] = df_hedged[cross + '-tot.close-bbg'] + df_hedged[cross + '-option-tot-with-tc.close']
+    df_hedged['Spot + 2*option put hedge'] = df_hedged[cross + '-tot.close-bbg'] + df_hedged[cross + '-option-tot-with-tc.close']
 
     df_hedged.columns = RetStats(returns_df=df_hedged, ann_factor=252).summary()
 
     # Plot everything
+
+    # P&L from call
     chart.plot(calculations.create_mult_index_from_prices(
         prepare_indices(cross=cross, df_option_tot=df_cuemacro_option_call_tot,
                         df_option_tc=df_cuemacro_option_call_tc, df_spot_tot=df_bbg_tot)))
 
+    # P&L from put option, put option + TC and total returns from spot
     chart.plot(calculations.create_mult_index_from_prices(
         prepare_indices(cross=cross,df_option_tot=df_cuemacro_option_put_tot,
                         df_option_tc=df_cuemacro_option_put_tc, df_spot_tot=df_bbg_tot)))
 
+    # P&L from put option + TC and total returns from spot
     chart.plot(calculations.create_mult_index_from_prices(
-        prepare_indices(cross=cross,df_option_tc=df_cuemacro_option_put_tc, df_spot_tot=df_bbg_tot)))
+        prepare_indices(cross=cross, df_option_tc=df_cuemacro_option_put_tc, df_spot_tot=df_bbg_tot)))
 
+    # P&L for total returns from spot and total returns from + 2*put option + TC (ie. hedged portfolio)
     chart.plot(calculations.create_mult_index(df_hedged))
 
+    # Plot delta from put option
+    chart.plot(df_cuemacro_option_put_tot[cross + '-delta.close'])
+
 
 ###### Fetch market data for pricing EURUSD options from 2006-2020 (ie. FX spot, FX forwards, FX deposits and FX vol quotes)
 ###### Construct volatility surface using FinancePy library underneath, using polynomial interpolation
 ###### Enters a short 1W straddle, and MTM every day, and at expiry rolls into another 1W straddle
 if run_example == 2 or run_example == 0:
 
     # Warning make sure you choose dates, where there is full vol surface! If vol points in the tenors you are looking at
@@ -210,15 +225,15 @@
 
     # Let's trade a short straddle, and we roll at expiry
     df_cuemacro_option_straddle_tot = fx_options_curve.construct_total_return_index(cross, df,
                                                                                     depo_tenor_for_option=fx_options_trading_tenor)
 
     # Add transaction costs to the option index (bid/ask bp for the option premium and spot FX)
     # Have wider spread for straddle (because adding call + put)
-    df_cuemacro_option_straddle_tc = fx_options_curve.apply_tc_to_total_return_index(cross, df_cuemacro_option_straddle_tot,
+    df_cuemacro_option_straddle_tc = fx_options_curve.apply_tc_signals_to_total_return_index(cross, df_cuemacro_option_straddle_tot,
                                                                                  option_tc_bp=10, spot_tc_bp=2)
 
     # Get total returns for spot
     md_request.abstract_curve = None
 
     # Get Bloomberg calculated total return indices (for spot)
     md_request.category = 'fx-tot'
```

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/fx_options_pricing_examples.py` & `finmarketpy-0.11.9/finmarketpy_examples/fx_options_pricing_examples.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and limitations under the License.
 #
 
 """
-Shows how to use finmarketpy to price FX options (uses FinancePy underneath).
+Shows how to use finmarketpy to price FX options (uses FinancePy underneath - it is recommended you pull the latest
+version of FinancePy from GitHub).
 
 Note, you will need to have a Bloomberg terminal (with blpapi Python library) to download the FX market data in order
 to plot these vol surface (FX spot, FX forwards, FX implied_vol volatility quotes and deposits)
 """
 
 import pandas as pd
 
@@ -25,14 +26,15 @@
 from chartpy import Chart, Style
 
 # For loading market data
 from findatapy.market import Market, MarketDataGenerator, MarketDataRequest
 
 from findatapy.util.loggermanager import LoggerManager
 
+from finmarketpy.curve.rates.fxforwardspricer import FXForwardsPricer
 from finmarketpy.curve.volatility.fxvolsurface import FXVolSurface
 from finmarketpy.curve.volatility.fxoptionspricer import FXOptionsPricer
 
 logger = LoggerManager().getLogger(__name__)
 
 chart = Chart(engine='plotly')
 market = Market(market_data_generator=MarketDataGenerator())
@@ -40,16 +42,17 @@
 # Choose run_example = 0 for everything
 # run_example = 1 - price GBPUSD options
 # run_example = 2 - price USDJPY options
 # run_example = 3 - price AUDUSD options
 # run_example = 4 - more pricing of AUDUSD options
 # run_example = 5 - pricing of EURUSD options
 # run_example = 6 - another USDJPY option
+# run_example = 7 - price USDBRL options
 
-run_example = 6
+run_example = 7
 
 ###### Fetch market data for pricing GBPUSD FX options over Brexit vote (ie. FX spot, FX forwards, FX deposits and FX vol quotes)
 ###### Construct volatility surface using FinancePy library underneath, using polynomial interpolation and
 ###### Then price some options over these dates eg. atm, 25d-call etc.
 if run_example == 1 or run_example == 0:
 
     horizon_date = '23 Jun 2016'
@@ -111,15 +114,15 @@
                                  tenor='1W', depo_tenor='1W').to_string())
 
     print("25d 3M european call")
     print(fx_op.price_instrument(cross, horizon_date, '25d-otm', contract_type='european-call',
                                  tenor='3M', depo_tenor='3M').to_string())
 
     print("10d 1M european put")
-    print(fx_op.price_instrument(cross, horizon_date, '10d-put', contract_type='european-put',
+    print(fx_op.price_instrument(cross, horizon_date, '10d-otm', contract_type='european-put',
                                  tenor='1M', depo_tenor='1M').to_string())
 
 ###### Fetch market data for pricing AUDUSD options on 18 Apr 2007, just before credit crisis
 ###### Construct volatility surface using FinancePy library underneath, using polynomial interpolation and
 ###### Then price some options over these dates eg. atm, 25d-call etc.
 if run_example == 3 or run_example == 0:
 
@@ -155,22 +158,24 @@
                                    data_source='bloomberg', cut='BGN', category='fx-vol-market',
                                    tickers=cross, base_depos_currencies=[cross[0:3], cross[3:6]],
                                    cache_algo='cache_algo_return')
 
     df = market.fetch_market(md_request)
 
     fx_vol_surface = FXVolSurface(market_df=df, asset=cross, tenors=['1W', '1M', '3M'])
+    fx_vol_surface.build_vol_surface(pd.Timestamp(horizon_date))
 
     fx_op = FXOptionsPricer(fx_vol_surface=fx_vol_surface)
 
     # Price several different options
 
     # Try a broken date 15D option (note, for broken dates, currently doesn't interpolate key strikes)
     # Specify expiry date instead of the tenor for broken dates
     print("atm 15D european call")
+
     print(fx_op.price_instrument(cross, pd.Timestamp(horizon_date), 0.8535,
             expiry_date=pd.Timestamp('05 Sep 2007'), contract_type='european-call').to_string())
 
 ###### Fetch market data for pricing EURUSD options during start of 2006
 if run_example == 5 or run_example == 0:
 
     horizon_date = '04 Jan 2006'
@@ -225,8 +230,47 @@
     fx_vol_surface.extract_vol_surface(num_strike_intervals=None)
 
     print("ATM vol " + str(fx_vol_surface.get_atm_vol(tenor='1W')))
 
     # Specify expiry date instead of the tenor for broken dates
     print("atm 1W european straddle")
     print(fx_op.price_instrument(cross, pd.Timestamp(horizon_date), 'atm',
-            tenor="1W", depo_tenor='1W', contract_type='european-straddle').to_string())
+            tenor="1W", depo_tenor='1W', contract_type='european-straddle').to_string())
+
+
+###### Price USDBRL option around 2018 2nd round of presidential election
+if run_example == 7 or run_example == 0:
+
+    horizon_date = '26 Oct 2018'
+    cross = 'USDBRL'
+    non_usd = 'BRL'
+
+    # Download the whole all market data for USDBRL for pricing options (vol surface)
+    md_request = MarketDataRequest(start_date=horizon_date, finish_date=horizon_date,
+                                   data_source='bloomberg', cut='NYC', category='fx-vol-market',
+                                   tickers=cross, base_depos_currencies=[cross[0:3]],
+                                   cache_algo='cache_algo_return')
+
+    df = market.fetch_market(md_request)
+
+    # Compute implied deposit BRL 1M from USDBRL forwards (and USD 1M depo)
+    fx_forwards_price = FXForwardsPricer()
+
+    implied_depo_df = fx_forwards_price.calculate_implied_depo(cross, non_usd, market_df=df,
+                               fx_forwards_tenor=['1W', '1M'],
+                               depo_tenor=['1W', '1M'])
+
+    implied_depo_df.columns = [x.replace('-implied-depo', '') for x in implied_depo_df.columns]
+    df = df.join(implied_depo_df, how='left')
+
+    # USDBRL quoted ATMF implied vol (as opposed to delta neutral) hence 'fwd' parameter
+    fx_op = FXOptionsPricer(fx_vol_surface=FXVolSurface(market_df=df, asset=cross, atm_method='fwd', depo_tenor='1M'))
+
+    # Price several different options
+    print(df)
+
+    print("atm 1M european put")
+    print(fx_op.price_instrument(cross, pd.Timestamp(horizon_date), 'atm', contract_type='european-put', tenor='1M').to_string())
+
+    # TODO: calendar around election results in slightly different pricing
+    # print(fx_op.price_instrument(cross, pd.Timestamp(horizon_date), '25d-otm', contract_type='european-put', tenor='1W').to_string())
+    # print(fx_op.price_instrument(cross, pd.Timestamp(horizon_date), 3.5724, contract_type='european-put', expiry_date=pd.Timestamp('2 Nov 2018')).to_string())
```

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/fx_spot_indices_examples.py` & `finmarketpy-0.11.9/finmarketpy_examples/fx_spot_indices_examples.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     df_bbg_tot_forwards = market.fetch_market(md_request)
     df_bbg_tot_forwards.columns = [x + '-bbg' for x in df_bbg_tot_forwards.columns]
 
     # Combine into a single data frame and plot, we note that the Cuemacro constructed indices track the Bloomberg
     # indices relatively well (both from spot and 1M forwards). Also note the large difference with spot indices
     # CAREFUL to fill down, before reindexing because 1M forwards indices are likely to have different publishing dates
-    df = calculations.pandas_outer_join([df_tot, df_bbg_tot, df_spot, df_bbg_tot_forwards]).fillna(method='ffill')
+    df = calculations.join([df_tot, df_bbg_tot, df_spot, df_bbg_tot_forwards], how='outer').fillna(method='ffill')
     df = calculations.create_mult_index_from_prices(df)
 
     chart.plot(df)
 
 ###### Create total return indices plot for GBPUSD with intraday and daily data (from perspective of a USD investor)
 ###### Compare intraday and daily total return indices
 if run_example == 2 or run_example == 0:
@@ -132,11 +132,11 @@
 
     df_intraday_tot = FXSpotCurve().construct_total_return_index('GBPUSD', df_intraday_market, depo_tenor='ON')
 
     df_intraday_spot.columns = [x + '-intraday-spot' for x in df_intraday_spot.columns]
     df_intraday_tot.columns = [x + '-intraday-tot' for x in df_intraday_spot.columns]
 
     # Combine into a single data frame and plot
-    df = calculations.pandas_outer_join([df_bbg_tot, df_tot, df_intraday_tot, df_intraday_spot]).fillna(method='ffill')
+    df = calculations.join([df_bbg_tot, df_tot, df_intraday_tot, df_intraday_spot], how='outer').fillna(method='ffill')
     df = calculations.create_mult_index_from_prices(df)
 
     chart.plot(df)
```

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/fx_vol_surface_animation.py` & `finmarketpy-0.11.9/finmarketpy_examples/fx_vol_surface_animation.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/fx_vol_surface_interpolation_examples.py` & `finmarketpy-0.11.9/finmarketpy_examples/fx_vol_surface_interpolation_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 # Choose run_example = 0 for everything
 # run_example = 1 - plot GBPUSD 1W implied vol
 # run_example = 2 - get GBPUSD vol surface for a date and plot interpolated vol surface and implied PDF
 # run_example = 3 - do an animation of GBPUSD implied vol surface over this period
 # run_example = 4 - get implied vol for a particular strike, interpolating the surface
 # run_example = 5 - get USDJPY vol surface around US presidential election and plot
 
-run_example = 3
+run_example = 2
 
 ###### Fetch market data for pricing GBPUSD FX options over Brexit vote (ie. FX spot, FX forwards, FX deposits and FX vol quotes)
 ###### Show how to plot ATM 1M implied_vol vol time series
 if run_example == 1 or run_example == 0:
 
     # Download the whole all market data for GBPUSD for pricing options (vol surface)
     md_request = MarketDataRequest(start_date='01 May 2016', finish_date='01 Aug 2016',
@@ -64,30 +64,31 @@
     chart.plot(df['GBPUSDV1M.close'], style=style)
 
 ###### Fetch market data for pricing GBPUSD FX options over Brexit vote (ie. FX spot, FX forwards, FX deposits and FX vol quotes)
 ###### Construct volatility surface using FinancePy library underneath, using polynomial interpolation
 if run_example == 2 or run_example == 0:
 
     horizon_date = '23 Jun 2016'
+    cross = 'GBPUSD'
 
     # Download the whole all market data for GBPUSD for pricing options (vol surface)
     md_request = MarketDataRequest(start_date=horizon_date, finish_date=horizon_date,
                                    data_source='bloomberg', cut='LDN', category='fx-vol-market',
-                                   tickers=['GBPUSD'],
+                                   tickers=cross,
                                    cache_algo='cache_algo_return')
 
     df = market.fetch_market(md_request)
 
-    fx_vol_surface = FXVolSurface(market_df=df, vol_function_type='BBG', asset='GBPUSD')
+    fx_vol_surface = FXVolSurface(market_df=df, vol_function_type='BBG', asset=cross)
 
     fx_vol_surface.build_vol_surface(horizon_date)
 
     # Note for unstable vol surface dates (eg. over Brexit date) you may need to increase tolerance in FinancePy
     # FinFXVolSurface.buildVolSurface method to get it to fill, or choose different vol_function_type (eg. 'CLARK5')
-    df_vol_dict = fx_vol_surface.extract_vol_surface()
+    df_vol_dict = fx_vol_surface.extract_vol_surface(low_K_pc=0.80, high_K_pc=1.1)
 
     # Print out the various vol surface and data produced
     print(df_vol_dict['vol_surface_implied_pdf'])
     print(df_vol_dict['vol_surface_strike_space'])
     print(df_vol_dict['vol_surface_delta_space'])
     print(df_vol_dict['vol_surface_delta_space_exc_ms'])
     print(df_vol_dict['deltas_vs_strikes'])
```

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/gallery/fx-trend-cumulative.png` & `finmarketpy-0.11.9/finmarketpy_examples/gallery/fx-trend-cumulative.png`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/gallery/fx-trend-leverage.png` & `finmarketpy-0.11.9/finmarketpy_examples/gallery/fx-trend-leverage.png`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/gallery/fx-trend-trade-returns.png` & `finmarketpy-0.11.9/finmarketpy_examples/gallery/fx-trend-trade-returns.png`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/gallery/fx-vol-seasonality.png` & `finmarketpy-0.11.9/finmarketpy_examples/gallery/fx-vol-seasonality.png`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/gallery/gold-seasonality.png` & `finmarketpy-0.11.9/finmarketpy_examples/gallery/gold-seasonality.png`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/gallery/usdjpy-nfp.png` & `finmarketpy-0.11.9/finmarketpy_examples/gallery/usdjpy-nfp.png`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/gold seasonality.png` & `finmarketpy-0.11.9/finmarketpy_examples/gold seasonality.png`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/quandl_examples.py` & `finmarketpy-0.11.9/finmarketpy_examples/quandl_examples.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/quickchart_examples.py` & `finmarketpy-0.11.9/finmarketpy_examples/quickchart_examples.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/returns_examples.py` & `finmarketpy-0.11.9/finmarketpy_examples/returns_examples.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/seasonality_examples.py` & `finmarketpy-0.11.9/finmarketpy_examples/seasonality_examples.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/technicals_example.py` & `finmarketpy-0.11.9/finmarketpy_examples/technicals_example.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/tradingmodelfxtrend_bbg_example.py` & `finmarketpy-0.11.9/finmarketpy_examples/tradingmodelfxtrend_bbg_example.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/tradingmodelfxtrend_example.py` & `finmarketpy-0.11.9/finmarketpy_examples/tradingmodelfxtrend_example.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/vol_stats_examples.py` & `finmarketpy-0.11.9/finmarketpy_examples/vol_stats_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and limitations under the License.
 #
 
-
 """
 Here we show how to use VolStats to calculate various volatility metrics (like realized volatility, volatility risk 
 premium and the implied volatility addons)
 
 Note, you will need to have a Bloomberg terminal (with blpapi Python library) to download the FX market data in order
 to run most of these examples (FX spot, FX forwards, FX implied_vol volatility quotes and deposits)
 """
@@ -120,15 +119,15 @@
                 tenor_label="ON", freq='intraday', freq_min_mult=min,
                 hour_of_day=10, minute_of_day=0, field='close', timezone_hour_minute='America/New_York') * 100
 
         rv.columns=[str(min) + 'min']
 
         realized_vol.append(rv)
 
-    realized_vol = calc.pandas_outer_join(realized_vol)
+    realized_vol = calc.join(realized_vol, how='outer')
     style = Style()
 
     style.title = 'GBPUSD ON realized volatility over Brexit with different minute sampling frequencies'
     style.scale_factor = 3
     style.source = 'Bloomberg'
     style.color = 'Blues'
```

### Comparing `finmarketpy-0.11.8/finmarketpy_examples/vwap_example.py` & `finmarketpy-0.11.9/finmarketpy_examples/vwap_example.py`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/finmarketpy_logo.png` & `finmarketpy-0.11.9/finmarketpy_logo.png`

 * *Files identical despite different names*

### Comparing `finmarketpy-0.11.8/setup.py` & `finmarketpy-0.11.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 long_description = """finmarketpy is a Python based library that enables you to analyze market data and also to backtest 
 trading strategies using a simple to use API, which has prebuilt templates for you to define backtest."""
 
 setup(name='finmarketpy',
-      version='0.11.8',
+      version='0.11.9',
       description='finmarketpy is a Python based library for backtesting trading strategies',
       author='Saeed Amen',
       author_email='saeed@cuemacro.com',
       license='Apache 2.0',
       long_description=long_description,
       keywords=['trading', 'markets', 'currencies', 'pandas', 'data', 'Bloomberg', 'tick', 'stocks', 'equities'],
       url='https://github.com/cuemacro/finmarketpy',
```

### Comparing `finmarketpy-0.11.8/tests/test_techindicator.py` & `finmarketpy-0.11.9/tests/test_techindicator.py`

 * *Files identical despite different names*


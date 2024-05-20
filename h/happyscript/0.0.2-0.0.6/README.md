# Comparing `tmp/happyscript-0.0.2.tar.gz` & `tmp/happyscript-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happyscript-0.0.2.tar", last modified: Mon Apr 22 02:42:45 2024, max compression
+gzip compressed data, was "happyscript-0.0.6.tar", last modified: Mon May 20 00:38:23 2024, max compression
```

## Comparing `happyscript-0.0.2.tar` & `happyscript-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 02:42:45.553816 happyscript-0.0.2/
--rw-rw-rw-   0        0        0      193 2024-04-22 02:42:45.553816 happyscript-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       26 2024-04-22 02:04:12.000000 happyscript-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 02:42:45.539808 happyscript-0.0.2/happyscript/
--rw-rw-rw-   0        0        0   211595 2024-04-22 01:55:54.000000 happyscript-0.0.2/happyscript/happyscript.py
-drwxrwxrwx   0        0        0        0 2024-04-22 02:42:45.553816 happyscript-0.0.2/happyscript.egg-info/
--rw-rw-rw-   0        0        0      193 2024-04-22 02:42:45.000000 happyscript-0.0.2/happyscript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2024-04-22 02:42:45.000000 happyscript-0.0.2/happyscript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 02:42:45.000000 happyscript-0.0.2/happyscript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-22 02:42:45.000000 happyscript-0.0.2/happyscript.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      274 2024-04-22 02:42:29.000000 happyscript-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-22 02:42:45.553816 happyscript-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 00:38:23.810307 happyscript-0.0.6/
+-rw-rw-rw-   0        0        0      193 2024-05-20 00:38:23.810307 happyscript-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2024-04-22 02:04:12.000000 happyscript-0.0.6/README.md
+-rw-rw-rw-   0        0        0     7509 2024-05-19 21:50:01.000000 happyscript-0.0.6/copy_code.py
+drwxrwxrwx   0        0        0        0 2024-05-20 00:38:23.723525 happyscript-0.0.6/happyscript/
+-rw-rw-rw-   0        0        0       65 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 00:38:23.745499 happyscript-0.0.6/happyscript/charts/
+-rw-rw-rw-   0        0        0        0 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/charts/__init__.py
+-rw-rw-rw-   0        0        0     5227 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/charts/chart.py
+-rw-rw-rw-   0        0        0     1417 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/charts/histogram_chart.py
+-rw-rw-rw-   0        0        0     1980 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/charts/histogram_series.py
+-rw-rw-rw-   0        0        0     4518 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/charts/panel_charts.py
+-rw-rw-rw-   0        0        0      992 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/charts/scatter_chart.py
+-rw-rw-rw-   0        0        0      723 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/charts/scatter_series.py
+-rw-rw-rw-   0        0        0     2107 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/charts/time_chart.py
+-rw-rw-rw-   0        0        0      912 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/charts/time_series.py
+drwxrwxrwx   0        0        0        0 2024-05-20 00:38:23.772838 happyscript-0.0.6/happyscript/forms/
+-rw-rw-rw-   0        0        0     1917 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/forms/form_askchoice.py
+-rw-rw-rw-   0        0        0     2553 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/forms/form_askimage.py
+-rw-rw-rw-   0        0        0    10492 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/forms/form_main.py
+-rw-rw-rw-   0        0        0      973 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/forms/form_ontestfailure.py
+-rw-rw-rw-   0        0        0     3962 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/forms/form_serials.py
+-rw-rw-rw-   0        0        0      389 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/forms/form_stop.py
+-rw-rw-rw-   0        0        0    25533 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/forms/formsbase.py
+-rw-rw-rw-   0        0        0    74565 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/imglib.py
+drwxrwxrwx   0        0        0        0 2024-05-20 00:38:23.797340 happyscript-0.0.6/happyscript/panels/
+-rw-rw-rw-   0        0        0     3257 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/panels/panel_log.py
+-rw-rw-rw-   0        0        0     2239 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/panels/panel_messages.py
+-rw-rw-rw-   0        0        0     2653 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/panels/panel_scripts2.py
+-rw-rw-rw-   0        0        0    11540 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/panels/panel_tests.py
+-rw-rw-rw-   0        0        0    17637 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/panels/panelsbase.py
+-rw-rw-rw-   0        0        0     2020 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/scriptartwork.py
+-rw-rw-rw-   0        0        0     1513 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/scriptcontrol.py
+-rw-rw-rw-   0        0        0      327 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/scriptexceptions.py
+-rw-rw-rw-   0        0        0     6753 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/scriptgui.py
+-rw-rw-rw-   0        0        0     3121 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/scriptinfo.py
+-rw-rw-rw-   0        0        0     7699 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/scriptmanager.py
+-rw-rw-rw-   0        0        0     3282 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/scriptparams.py
+-rw-rw-rw-   0        0        0     3449 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/scriptreader.py
+-rw-rw-rw-   0        0        0     4715 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/scriptrunner.py
+drwxrwxrwx   0        0        0        0 2024-05-20 00:38:23.808312 happyscript-0.0.6/happyscript/testlog/
+-rw-rw-rw-   0        0        0     2150 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/testlog/global_log_handler.py
+-rw-rw-rw-   0        0        0     1706 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/testlog/log_to_text.py
+-rw-rw-rw-   0        0        0     1080 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/testlog/logtoxml.py
+-rw-rw-rw-   0        0        0     1506 2024-05-20 00:38:18.000000 happyscript-0.0.6/happyscript/testlog/printredirect.py
+drwxrwxrwx   0        0        0        0 2024-05-20 00:38:23.809309 happyscript-0.0.6/happyscript.egg-info/
+-rw-rw-rw-   0        0        0      193 2024-05-20 00:38:23.000000 happyscript-0.0.6/happyscript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1366 2024-05-20 00:38:23.000000 happyscript-0.0.6/happyscript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 00:38:23.000000 happyscript-0.0.6/happyscript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-20 00:38:23.000000 happyscript-0.0.6/happyscript.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2112 2024-05-20 00:12:29.000000 happyscript-0.0.6/increment_version.py
+-rw-rw-rw-   0        0        0      538 2024-05-20 00:38:18.000000 happyscript-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 00:38:23.811303 happyscript-0.0.6/setup.cfg
```


# Comparing `tmp/fnschool-20240520.80901.843.tar.gz` & `tmp/fnschool-20240520.81132.858.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240520.80901.843.tar", last modified: Mon May 20 01:01:48 2024, max compression
+gzip compressed data, was "fnschool-20240520.81132.858.tar", last modified: Mon May 20 03:33:03 2024, max compression
```

## Comparing `fnschool-20240520.80901.843.tar` & `fnschool-20240520.81132.858.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.093973 fnschool-20240520.80901.843/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240520.80901.843/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-20 01:01:48.092973 fnschool-20240520.80901.843/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240520.80901.843/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240520.80901.843/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-20 01:01:48.093973 fnschool-20240520.80901.843/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.067973 fnschool-20240520.80901.843/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.073973 fnschool-20240520.80901.843/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      380 2024-05-20 01:01:43.000000 fnschool-20240520.80901.843/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3154 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.083973 fnschool-20240520.80901.843/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    13817 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/bill.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     6638 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240520.80901.843/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/config.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/consume.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1521 2024-05-20 00:56:02.000000 fnschool-20240520.80901.843/src/fnschool/canteen/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      268 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/currency.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.084973 fnschool-20240520.80901.843/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   255702 2024-05-19 23:32:21.000000 fnschool-20240520.80901.843/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240520.80901.843/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240520.80901.843/src/fnschool/canteen/data/purchase_list.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/food.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-15 05:52:50.000000 fnschool-20240520.80901.843/src/fnschool/canteen/food_classes.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240520.80901.843/src/fnschool/canteen/food_recount.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240520.80901.843/src/fnschool/canteen/food_recounts.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     5240 2024-05-20 00:57:23.000000 fnschool-20240520.80901.843/src/fnschool/canteen/operator.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      779 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2809 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/profile.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.089973 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4075 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/base.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10382 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/consumingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1886 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/cover.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9302 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9381 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     8254 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/inventory.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10827 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/preconsuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9734 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/purchasing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2704 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/purchasingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4386 2024-05-20 00:46:18.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/unwarehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/warehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/warehouse.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    98394 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/workbook.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240520.80901.843/src/fnschool/canteen/workbook.toml
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.089973 fnschool-20240520.80901.843/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240520.80901.843/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1034 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1374 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      776 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/fnprint.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.069973 fnschool-20240520.80901.843/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.068972 fnschool-20240520.80901.843/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.090973 fnschool-20240520.80901.843/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-20 01:01:42.000000 fnschool-20240520.80901.843/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.069973 fnschool-20240520.80901.843/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.090973 fnschool-20240520.80901.843/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    18750 2024-05-20 01:01:42.000000 fnschool-20240520.80901.843/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.069973 fnschool-20240520.80901.843/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.090973 fnschool-20240520.80901.843/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-20 01:01:43.000000 fnschool-20240520.80901.843/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.069973 fnschool-20240520.80901.843/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.091973 fnschool-20240520.80901.843/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-20 01:01:43.000000 fnschool-20240520.80901.843/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.070973 fnschool-20240520.80901.843/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.091973 fnschool-20240520.80901.843/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-20 01:01:43.000000 fnschool-20240520.80901.843/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)     1217 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/test.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.091973 fnschool-20240520.80901.843/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-20 01:01:48.000000 fnschool-20240520.80901.843/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2218 2024-05-20 01:01:48.000000 fnschool-20240520.80901.843/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-20 01:01:48.000000 fnschool-20240520.80901.843/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-20 01:01:48.000000 fnschool-20240520.80901.843/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-20 01:01:48.000000 fnschool-20240520.80901.843/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-20 01:01:48.000000 fnschool-20240520.80901.843/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 03:33:03.127472 fnschool-20240520.81132.858/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240520.81132.858/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-20 03:33:03.127472 fnschool-20240520.81132.858/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240520.81132.858/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240520.81132.858/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-20 03:33:03.128473 fnschool-20240520.81132.858/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 03:33:03.104471 fnschool-20240520.81132.858/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 03:33:03.111472 fnschool-20240520.81132.858/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      380 2024-05-20 03:32:58.000000 fnschool-20240520.81132.858/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3154 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 03:33:03.119472 fnschool-20240520.81132.858/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    13817 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/bill.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     6638 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240520.81132.858/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/config.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/consume.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1523 2024-05-20 03:20:05.000000 fnschool-20240520.81132.858/src/fnschool/canteen/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      268 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/currency.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 03:33:03.120472 fnschool-20240520.81132.858/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   255702 2024-05-19 23:32:21.000000 fnschool-20240520.81132.858/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240520.81132.858/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240520.81132.858/src/fnschool/canteen/data/purchase_list.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/food.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-15 05:52:50.000000 fnschool-20240520.81132.858/src/fnschool/canteen/food_classes.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240520.81132.858/src/fnschool/canteen/food_recount.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240520.81132.858/src/fnschool/canteen/food_recounts.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     5343 2024-05-20 03:28:40.000000 fnschool-20240520.81132.858/src/fnschool/canteen/operator.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      779 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2809 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/profile.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 03:33:03.124472 fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4075 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/base.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10382 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/consumingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1886 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/cover.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9302 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9381 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     8254 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/inventory.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10827 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/preconsuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9734 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/purchasing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2704 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/purchasingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4386 2024-05-20 00:46:18.000000 fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/unwarehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/warehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/warehouse.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    98394 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/canteen/workbook.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240520.81132.858/src/fnschool/canteen/workbook.toml
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 03:33:03.125472 fnschool-20240520.81132.858/src/fnschool/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240520.81132.858/src/fnschool/data/config0.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1034 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1374 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      776 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/fnprint.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 03:33:03.107472 fnschool-20240520.81132.858/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 03:33:03.105471 fnschool-20240520.81132.858/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 03:33:03.125472 fnschool-20240520.81132.858/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-20 03:32:58.000000 fnschool-20240520.81132.858/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 03:33:03.106471 fnschool-20240520.81132.858/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 03:33:03.125472 fnschool-20240520.81132.858/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    18957 2024-05-20 03:32:58.000000 fnschool-20240520.81132.858/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 03:33:03.106471 fnschool-20240520.81132.858/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 03:33:03.125472 fnschool-20240520.81132.858/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-20 03:32:58.000000 fnschool-20240520.81132.858/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 03:33:03.106471 fnschool-20240520.81132.858/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 03:33:03.126473 fnschool-20240520.81132.858/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-20 03:32:58.000000 fnschool-20240520.81132.858/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 03:33:03.107472 fnschool-20240520.81132.858/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 03:33:03.126473 fnschool-20240520.81132.858/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-20 03:32:58.000000 fnschool-20240520.81132.858/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1217 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-19 23:33:33.000000 fnschool-20240520.81132.858/src/fnschool/test.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 03:33:03.126473 fnschool-20240520.81132.858/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-20 03:33:03.000000 fnschool-20240520.81132.858/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2218 2024-05-20 03:33:03.000000 fnschool-20240520.81132.858/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-20 03:33:03.000000 fnschool-20240520.81132.858/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-20 03:33:03.000000 fnschool-20240520.81132.858/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-20 03:33:03.000000 fnschool-20240520.81132.858/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-20 03:33:03.000000 fnschool-20240520.81132.858/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240520.80901.843/LICENSE` & `fnschool-20240520.81132.858/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/PKG-INFO` & `fnschool-20240520.81132.858/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240520.80901.843
+Version: 20240520.81132.858
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240520.80901.843/README.md` & `fnschool-20240520.81132.858/README.md`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/pyproject.toml` & `fnschool-20240520.81132.858/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/app.py` & `fnschool-20240520.81132.858/src/fnschool/app.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/bill.cp.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/bill.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/bill.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/bill.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/canteen.toml` & `fnschool-20240520.81132.858/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/config.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/consuming.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/consuming.py`

 * *Files 15% similar despite different names*

```diff
@@ -45,14 +45,14 @@
             for f in foods:
                 self._day_m1 = max(
                     [d.day for d, __ in f.consumptions] + [self._day_m1]
                 )
             if self._day_m1 < 1:
                 print_error(
                     _(
-                        "It seems you didn't design the consumption, "
+                        "It seems you didn't design the consumptions, "
                         + "please restart {0} and design "
-                        + "the consumptions"
+                        + "the consumptions."
                     ).format(app_name)
                 )
                 exit()
         return self._day_m1
```

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240520.81132.858/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240520.81132.858/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/data/purchase_list.xlsx` & `fnschool-20240520.81132.858/src/fnschool/canteen/data/purchase_list.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/food.cp.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/food.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/food.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/food_classes.toml` & `fnschool-20240520.81132.858/src/fnschool/canteen/food_classes.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/operator.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,16 @@
             self._dpath = dpath1
             if not self._dpath.exists():
                 os.makedirs(self._dpath, exist_ok=True)
         if not self.dpath_showed:
             print_info(
                 _(
                     "Hey! {0}, all of your files will be" 
-                    +" saved to {1}, show it now? (Yes: 'Y','y')"
+                    +" saved to \"{1}\", show it now? "
+                    + "(Yes: 'Y','y')"
                 ).format(
                     self.name,
                     self._dpath
                 )
             )
             o_input = input(">_").replace(' ','')
             if len(o_input) > 0 and o_input in 'Yy':
@@ -134,19 +135,22 @@
     def get_profile(self, key, info=None):
         profile = self.profile
         if not key in profile.keys():
             print_warning(
                 info or _("Please tell {0} the {1}.").format(app_name, key)
             )
             superior_department = None
-            for __ in range(0, 3):
+            for i in range(0, 3):
                 i_value = input(">_").replace(" ", "")
                 if len(i_value) > 0:
                     break
                 print_error(_("Unexpected value got."))
+                if i >= 2:
+                    exit()
+                    
 
             self.profile[key] = i_value
             self.save_profile()
         return self.profile[key]
 
     @property
     def bill_dpath(self):
```

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/path.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/profile.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/profile.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/base.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/base.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/consuming.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/consuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/consumingsum.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/consumingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/cover.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/cover.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/ctspreadsheet.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/ctspreadsheet.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/food.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/inventory.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/inventory.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/preconsuming.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/preconsuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/purchasing.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/purchasing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/purchasingsum.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/purchasingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/unwarehousing.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/unwarehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/warehousing.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/spreadsheet/warehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/test.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/canteen/workbook.py` & `fnschool-20240520.81132.858/src/fnschool/canteen/workbook.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/entry.py` & `fnschool-20240520.81132.858/src/fnschool/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/external.py` & `fnschool-20240520.81132.858/src/fnschool/external.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/fnprint.py` & `fnschool-20240520.81132.858/src/fnschool/fnprint.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/language.py` & `fnschool-20240520.81132.858/src/fnschool/language.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240520.81132.858/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  fnschool\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-05-20 07:36+0800\n"
-"PO-Revision-Date: 2024-05-20 07:36+0800\n"
+"POT-Creation-Date: 2024-05-20 11:21+0800\n"
+"PO-Revision-Date: 2024-05-20 11:20+0800\n"
 "Last-Translator: larryw3i <larryw3i@163.com>\n"
 "Language: zh_CN\n"
 "Language-Team: Chinese - China <larryw3i@163.com>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -177,17 +177,18 @@
 msgid "Got no purchased foods of time node %s ."
 msgstr "时间节点 %s 没有购入的食材。"
 
 msgid "Hello! helping information is here for you:"
 msgstr "您好！这里是给您的帮助信息："
 
 msgid ""
-"Hey! {0}, all of your files will be saved to {1}, show it now? (Yes: 'Y','y')"
+"Hey! {0}, all of your files will be saved to \"{1}\", show it now? (Yes: "
+"'Y','y')"
 msgstr ""
-"您好～ {0}，您的所有文件将会被保存到 {1} 文件夹，打开它？（打开：“Y”、“y”）"
+"您好～ {0}，您的所有文件将会被保存到 “{1}” 文件夹，打开它？（打开：“Y”、“y”）"
 
 msgid "Hi, your name is \"{0}\"? (Yes: 'Y' 'y' '', or enter your name)"
 msgstr "您好！您是 “{0}” 吗？（是：“Y”、“y”、“”，或者输入您的姓名）"
 
 msgid ""
 "If new Xuelan milks is purchased. you have to add the purchasing information "
 "of them into the end of the purchasing spreadsheet (e.g: the spreadsheets "
@@ -220,14 +221,19 @@
 
 msgid ""
 "It seems the residue foods from last time node are going to be consumed. The "
 "new foods of this time node ({0})aren't purchased."
 msgstr "好像时间节点 {0} 没有新购入的食材，消耗将只从剩余的食材中进行。"
 
 msgid ""
+"It seems you didn't design the consumptions, please restart {0} and design "
+"the consumptions."
+msgstr "好像您没有设计每天的出库，请重新运行 {0} 然后设计每天的出库。"
+
+msgid ""
 "It seems you didn't set the 'negligible' mark for workbook '{0}' , update "
 "this workbook and press ANY key to continue. (Add the 'negligible' column "
 "name even though there is no negligible foods)"
 msgstr ""
 "好像您没有 在 工作簿 “{0}” 添加 “非入库” 列，请添加 “非入库” 列，然后按任意键"
 "继续。（如果没有非入库的食材，只需添加列名）"
```

### Comparing `fnschool-20240520.80901.843/src/fnschool/path.py` & `fnschool-20240520.81132.858/src/fnschool/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool/test.py` & `fnschool-20240520.81132.858/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240520.80901.843/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240520.81132.858/src/fnschool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240520.80901.843
+Version: 20240520.81132.858
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240520.80901.843/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240520.81132.858/src/fnschool.egg-info/SOURCES.txt`

 * *Files identical despite different names*


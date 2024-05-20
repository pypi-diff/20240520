# Comparing `tmp/fnschool-20240519.81611.835.tar.gz` & `tmp/fnschool-20240520.80901.843.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240519.81611.835.tar", last modified: Sun May 19 08:11:38 2024, max compression
+gzip compressed data, was "fnschool-20240520.80901.843.tar", last modified: Mon May 20 01:01:48 2024, max compression
```

## Comparing `fnschool-20240519.81611.835.tar` & `fnschool-20240520.80901.843.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 08:11:38.733592 fnschool-20240519.81611.835/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-04-27 16:06:09.000000 fnschool-20240519.81611.835/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-19 08:11:38.732592 fnschool-20240519.81611.835/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-27 16:06:09.000000 fnschool-20240519.81611.835/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-04-27 16:06:09.000000 fnschool-20240519.81611.835/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-19 08:11:38.733592 fnschool-20240519.81611.835/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 08:11:38.712592 fnschool-20240519.81611.835/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 08:11:38.717592 fnschool-20240519.81611.835/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      380 2024-05-19 08:11:35.000000 fnschool-20240519.81611.835/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240519.81611.835/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3154 2024-05-19 07:36:56.000000 fnschool-20240519.81611.835/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 08:11:38.724592 fnschool-20240519.81611.835/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-12 17:09:24.000000 fnschool-20240519.81611.835/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-12 04:59:07.000000 fnschool-20240519.81611.835/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    13817 2024-05-17 16:00:10.000000 fnschool-20240519.81611.835/src/fnschool/canteen/bill.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     6638 2024-05-17 16:08:29.000000 fnschool-20240519.81611.835/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-08 00:15:03.000000 fnschool-20240519.81611.835/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-17 16:00:10.000000 fnschool-20240519.81611.835/src/fnschool/canteen/config.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240519.81611.835/src/fnschool/canteen/consume.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      949 2024-05-17 16:00:10.000000 fnschool-20240519.81611.835/src/fnschool/canteen/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      268 2024-05-17 16:00:10.000000 fnschool-20240519.81611.835/src/fnschool/canteen/currency.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 08:11:38.726592 fnschool-20240519.81611.835/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   255702 2024-05-19 01:02:43.000000 fnschool-20240519.81611.835/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-04-27 16:06:09.000000 fnschool-20240519.81611.835/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-27 16:06:09.000000 fnschool-20240519.81611.835/src/fnschool/canteen/data/purchase_list.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-12 19:17:55.000000 fnschool-20240519.81611.835/src/fnschool/canteen/food.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-12 09:54:45.000000 fnschool-20240519.81611.835/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-17 16:00:10.000000 fnschool-20240519.81611.835/src/fnschool/canteen/food_classes.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:50:28.000000 fnschool-20240519.81611.835/src/fnschool/canteen/food_recount.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:50:32.000000 fnschool-20240519.81611.835/src/fnschool/canteen/food_recounts.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     5011 2024-05-19 08:09:21.000000 fnschool-20240519.81611.835/src/fnschool/canteen/operator.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1236 2024-05-17 16:33:52.000000 fnschool-20240519.81611.835/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2809 2024-05-17 16:33:53.000000 fnschool-20240519.81611.835/src/fnschool/canteen/profile.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 08:11:38.730592 fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-17 16:00:10.000000 fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4075 2024-05-17 16:33:53.000000 fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/base.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10382 2024-05-17 16:02:00.000000 fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-19 07:36:56.000000 fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/consumingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1886 2024-05-17 16:00:10.000000 fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/cover.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9302 2024-05-17 16:33:53.000000 fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9381 2024-05-17 16:00:10.000000 fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     8254 2024-05-17 16:00:10.000000 fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/inventory.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10827 2024-05-17 16:33:53.000000 fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/preconsuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9734 2024-05-17 16:33:53.000000 fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/purchasing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2704 2024-05-19 07:36:56.000000 fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/purchasingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4492 2024-05-17 16:33:53.000000 fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/unwarehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-12 18:18:03.000000 fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-17 16:00:10.000000 fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/warehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-12 04:59:07.000000 fnschool-20240519.81611.835/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240519.81611.835/src/fnschool/canteen/warehouse.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    98394 2024-05-17 16:33:56.000000 fnschool-20240519.81611.835/src/fnschool/canteen/workbook.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:48:23.000000 fnschool-20240519.81611.835/src/fnschool/canteen/workbook.toml
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 08:11:38.730592 fnschool-20240519.81611.835/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-04-27 16:06:09.000000 fnschool-20240519.81611.835/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1034 2024-05-17 16:08:56.000000 fnschool-20240519.81611.835/src/fnschool/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1302 2024-05-17 16:00:10.000000 fnschool-20240519.81611.835/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      776 2024-05-17 16:00:10.000000 fnschool-20240519.81611.835/src/fnschool/fnprint.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-12 04:59:07.000000 fnschool-20240519.81611.835/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 08:11:38.714592 fnschool-20240519.81611.835/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 08:11:38.713592 fnschool-20240519.81611.835/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 08:11:38.731592 fnschool-20240519.81611.835/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-19 08:11:35.000000 fnschool-20240519.81611.835/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 08:11:38.713592 fnschool-20240519.81611.835/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 08:11:38.731592 fnschool-20240519.81611.835/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    18557 2024-05-19 08:11:35.000000 fnschool-20240519.81611.835/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 08:11:38.714592 fnschool-20240519.81611.835/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 08:11:38.731592 fnschool-20240519.81611.835/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-19 08:11:35.000000 fnschool-20240519.81611.835/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 08:11:38.714592 fnschool-20240519.81611.835/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 08:11:38.731592 fnschool-20240519.81611.835/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-19 08:11:35.000000 fnschool-20240519.81611.835/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 08:11:38.714592 fnschool-20240519.81611.835/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 08:11:38.732592 fnschool-20240519.81611.835/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-19 08:11:35.000000 fnschool-20240519.81611.835/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)     1611 2024-05-17 16:00:10.000000 fnschool-20240519.81611.835/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-12 04:59:07.000000 fnschool-20240519.81611.835/src/fnschool/test.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 08:11:38.732592 fnschool-20240519.81611.835/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-19 08:11:38.000000 fnschool-20240519.81611.835/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2218 2024-05-19 08:11:38.000000 fnschool-20240519.81611.835/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-19 08:11:38.000000 fnschool-20240519.81611.835/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-19 08:11:38.000000 fnschool-20240519.81611.835/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-19 08:11:38.000000 fnschool-20240519.81611.835/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-19 08:11:38.000000 fnschool-20240519.81611.835/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.093973 fnschool-20240520.80901.843/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240520.80901.843/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-20 01:01:48.092973 fnschool-20240520.80901.843/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240520.80901.843/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240520.80901.843/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-20 01:01:48.093973 fnschool-20240520.80901.843/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.067973 fnschool-20240520.80901.843/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.073973 fnschool-20240520.80901.843/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      380 2024-05-20 01:01:43.000000 fnschool-20240520.80901.843/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3154 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.083973 fnschool-20240520.80901.843/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    13817 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/bill.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     6638 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240520.80901.843/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/config.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/consume.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1521 2024-05-20 00:56:02.000000 fnschool-20240520.80901.843/src/fnschool/canteen/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      268 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/currency.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.084973 fnschool-20240520.80901.843/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   255702 2024-05-19 23:32:21.000000 fnschool-20240520.80901.843/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240520.80901.843/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240520.80901.843/src/fnschool/canteen/data/purchase_list.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/food.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-15 05:52:50.000000 fnschool-20240520.80901.843/src/fnschool/canteen/food_classes.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240520.80901.843/src/fnschool/canteen/food_recount.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240520.80901.843/src/fnschool/canteen/food_recounts.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     5240 2024-05-20 00:57:23.000000 fnschool-20240520.80901.843/src/fnschool/canteen/operator.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      779 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2809 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/profile.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.089973 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4075 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/base.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10382 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/consumingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1886 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/cover.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9302 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9381 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     8254 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/inventory.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10827 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/preconsuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9734 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/purchasing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2704 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/purchasingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4386 2024-05-20 00:46:18.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/unwarehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/warehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/warehouse.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    98394 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/canteen/workbook.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240520.80901.843/src/fnschool/canteen/workbook.toml
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.089973 fnschool-20240520.80901.843/src/fnschool/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240520.80901.843/src/fnschool/data/config0.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1034 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1374 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      776 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/fnprint.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.069973 fnschool-20240520.80901.843/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.068972 fnschool-20240520.80901.843/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.090973 fnschool-20240520.80901.843/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-20 01:01:42.000000 fnschool-20240520.80901.843/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.069973 fnschool-20240520.80901.843/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.090973 fnschool-20240520.80901.843/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    18750 2024-05-20 01:01:42.000000 fnschool-20240520.80901.843/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.069973 fnschool-20240520.80901.843/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.090973 fnschool-20240520.80901.843/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-20 01:01:43.000000 fnschool-20240520.80901.843/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.069973 fnschool-20240520.80901.843/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.091973 fnschool-20240520.80901.843/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-20 01:01:43.000000 fnschool-20240520.80901.843/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.070973 fnschool-20240520.80901.843/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.091973 fnschool-20240520.80901.843/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-20 01:01:43.000000 fnschool-20240520.80901.843/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1217 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-19 23:33:33.000000 fnschool-20240520.80901.843/src/fnschool/test.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-20 01:01:48.091973 fnschool-20240520.80901.843/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-20 01:01:48.000000 fnschool-20240520.80901.843/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2218 2024-05-20 01:01:48.000000 fnschool-20240520.80901.843/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-20 01:01:48.000000 fnschool-20240520.80901.843/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-20 01:01:48.000000 fnschool-20240520.80901.843/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-20 01:01:48.000000 fnschool-20240520.80901.843/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-20 01:01:48.000000 fnschool-20240520.80901.843/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240519.81611.835/LICENSE` & `fnschool-20240520.80901.843/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/PKG-INFO` & `fnschool-20240520.80901.843/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240519.81611.835
+Version: 20240520.80901.843
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240519.81611.835/README.md` & `fnschool-20240520.80901.843/README.md`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/pyproject.toml` & `fnschool-20240520.80901.843/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/app.py` & `fnschool-20240520.80901.843/src/fnschool/app.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/bill.cp.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/bill.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/bill.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/bill.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/canteen.toml` & `fnschool-20240520.80901.843/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/config.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240520.80901.843/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240520.80901.843/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/data/purchase_list.xlsx` & `fnschool-20240520.80901.843/src/fnschool/canteen/data/purchase_list.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/food.cp.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/food.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/food.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/food_classes.toml` & `fnschool-20240520.80901.843/src/fnschool/canteen/food_classes.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/operator.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/operator.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class Operator:
     def __init__(self, bill):
         self.bill = bill
         self._name = None
         self._dpath = None
         self._profile = {}
-        self._superior_department_key = _("superior department")
+        self.dpath_showed = False
         pass
 
     def __str__(self):
         return self.name
 
     @property
     def name(self):
@@ -57,30 +57,37 @@
     def dpath(self):
         if not self._dpath:
             dpath0 = user_config_dir / self.name
             dpath1 = user_data_dir / self.name
             self._dpath = dpath1
             if not self._dpath.exists():
                 os.makedirs(self._dpath, exist_ok=True)
-        make_link(self._dpath, self.link_dpath)
+        if not self.dpath_showed:
+            print_info(
+                _(
+                    "Hey! {0}, all of your files will be" 
+                    +" saved to {1}, show it now? (Yes: 'Y','y')"
+                ).format(
+                    self.name,
+                    self._dpath
+                )
+            )
+            o_input = input(">_").replace(' ','')
+            if len(o_input) > 0 and o_input in 'Yy':
+                open_path(self._dpath)
+            self.dpath_showed = True
         return self._dpath
 
     @property
     def preconsuming_dpath(self):
         dpath = self.dpath / _("preconsuming")
         if not dpath.exists():
             os.makedirs(dpath, exist_ok=True)
         return dpath
 
-    @property
-    def link_dpath(self):
-        dpath0 = canteen_links_dpath / self.name
-        dpath1 = user_documents_dpath / app_name / self.name
-        dpath = dpath0
-        return dpath
 
     @property
     def config_dpath(self):
         dpath = self.dpath / _("config")
         if not dpath.exists():
             os.makedirs(dpath, exist_ok=True)
         return dpath
```

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/profile.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             print_info(
                 _(
                     "Profile label for data directory making, "
                     + "it shouldn't contain any space character.\n"
                     + "Supplier names are the supplier's alias."
                 )
             )
-            open_file(self.fpath)
+            open_path(self.fpath)
             print_info(_("Ok! it was configured. (enter any key)"))
             input(">_ ")
 
         with open(self.fpath, "r", encoding="utf-8") as f:
             profile = tomllib.load(f)["profile"]
             profile = Profile(
                 label=profile[0],
```

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/base.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/base.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/consuming.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/consuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/consumingsum.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/consumingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/cover.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/cover.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/ctspreadsheet.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/ctspreadsheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         else:
             self.bwb.save(bill_fpath0)
 
         print_info(
             _('Updated data has been saved to "{0}".').format(bill_fpath0)
         )
 
-        open_file(bill_fpath0)
+        open_path(bill_fpath0)
 
         print_info(_("Updated data was saved."))
 
     def print_summary(self, foods=None):
         bfoods = foods or self.bill.foods
         cfoods = [f for f in bfoods if not f.is_abandoned]
         currency_mark = self.bill.currency.mark
```

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/food.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/inventory.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/inventory.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/preconsuming.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/preconsuming.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
                     "There is no need to design for "
                     + "dates without food consumption. "
                     + "(Ok, I know [press any key to continue])"
                 )
             )
             input(">_ ")
             wb.close()
-            open_file(wb_fpath)
+            open_path(wb_fpath)
             print_info(
                 _(
                     "Ok! I have updated spreadsheet '{0}'. (Press any key)"
                 ).format(wb_fpath)
             )
             input(">_ ")
             wb = load_workbook(wb_fpath)
```

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/purchasing.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/purchasing.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,15 +227,15 @@
                 + "please verify/modify it. "
                 + "Feel free to open new issue if some "
                 + "food with the wrong class ({1}). "
                 + "(Press any key to check it)"
             ).format(self.food_class_col_name, get_new_issue_url())
         )
         input(">_ ")
-        open_file(self.path)
+        open_path(self.path)
         print_info(_("Ok, I checked it, it's ok. (Press any key to continue)"))
         input(">_ ")
         pass
 
     def read_pfoods(self):
         self.update_fclass()
         foods = pd.read_excel(self.path)
```

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/purchasingsum.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/purchasingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/unwarehousing.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/unwarehousing.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,20 +55,15 @@
                     + "Sheet {0} updating skipped."
                 ).format(self.sheet.title)
             )
             return None
 
         foods = sorted(foods, key=lambda f: f.xdate)
 
-        t1 = []
-
-        for bf in self.bfoods:
-            for d, __ in bf.consumptions:
-                t1.append(d)
-        t1 = sorted(t1)[-1]
+        t1 = self.bill.consuming.date_m1
 
         row_indexes = []
         for form_index in form_indexes:
             form_index0, form_index1 = form_index
             unwsheet.cell(form_index0, 1, f" 学校名称：{self.purchaser}")
             unwsheet.cell(
                 form_index0,
```

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/spreadsheet/warehousing.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/spreadsheet/warehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/test.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/canteen/workbook.py` & `fnschool-20240520.80901.843/src/fnschool/canteen/workbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -982,15 +982,15 @@
                     + "for next updating."
                 )
             )
         else:
             self.copy_bill_workbook(wb_fpath=random_spreadsheet_fpath)
             spreadsheet0_fpath = random_spreadsheet_fpath
 
-        open_file(spreadsheet0_fpath)
+        open_path(spreadsheet0_fpath)
         print_info(_("Updated data was saved."))
 
     def get_changsheng_properties_by_dir(self, fdpath=None):
         fd_path = self.purchase_workbook_fd_path or fdpath
         properties = []
         if not Path(fd_path).is_dir():
             return None
@@ -1169,15 +1169,15 @@
                 print_info(
                     _(
                         "Workbook '{0}' was updated, please design the "
                         + "daily foods consumption and press ANY key "
                         + "to continue."
                     ).format(fpath)
                 )
-                open_file(fpath)
+                open_path(fpath)
                 input(">_ ")
                 wb = load_workbook(fpath)
                 sheet = wb[self.pre_consuming_sheet0_name]
                 print_info(_("Workbook %s was read.") % fpath)
 
             for i, _f in enumerate(_foods):
                 row_index = row_index_offset + i
@@ -1275,15 +1275,15 @@
                 if _org_name_col_index < 0:
                     print_warning(
                         _(
                             "{app_name} desn't pick the index of organization name"
                             + " column, input it (0 base) or '{wb_fpath}' will be ignored."
                         ).format(app_name=app_name, wb_fpath=wb_fpath)
                     )
-                    open_file(wb_fpath)
+                    open_path(wb_fpath)
                     _org_name_col_index = input(">_ ")
                     if not _org_name_col_index.isnumeric():
                         continue
                     _org_name_col_index = int(_org_name_col_index)
 
                 _org_names = list(
                     set(
@@ -1335,15 +1335,15 @@
                     print_info(
                         _(
                             "The column names of 'negligible' mark are following:"
                         )
                         + "\n\t"
                         + " | ".join(self.negligible_col_names)
                     )
-                    open_file(wb_fpath)
+                    open_path(wb_fpath)
                     input(">_ ")
                     wb = load_workbook(wb_fpath, read_only=True)
                     sheet = wb[sheetnames[0]]
 
                 print_info(_("Spreadsheet '%s' was used."))
 
                 (
@@ -2013,15 +2013,15 @@
             ).format(sheet.title)
         )
         print_info(
             _("Ok! I have updated spreadsheet '{0}'. (Press any key)").format(
                 wb_fpath
             )
         )
-        open_file(wb_fpath)
+        open_path(wb_fpath)
         input(">_ ")
 
     def set_warehousing_form_index_offset(self, offset=0):
         self.warehousing_form_index_offset = offset
 
     def set_inventory_form_index_offset(self, offset=0):
         self.inventory_form_index_offset = offset
```

### Comparing `fnschool-20240519.81611.835/src/fnschool/entry.py` & `fnschool-20240520.80901.843/src/fnschool/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/external.py` & `fnschool-20240520.80901.843/src/fnschool/external.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,21 +40,23 @@
             + "README.zh_CN.md#%E8%B5%9E%E5%8A%A9"
         )
         if is_zh_CN
         else ("https://github.com/larryw3i/" + "funingschool#support")
     )
 
 
-def open_file(file_path):
+def open_path(file_path):
     file_path = str(file_path)
     bin_name = "open" if (sys_is_linux() or sys_is_darwin()) else "start"
     file_path = '"' + file_path + '"'
     if sys_is_win():
         if file_path.endswith('.toml"'):
             bin_name = "notepad"
+        elif Path(file_path).isdir():
+            bin_name = 'explorer'
         else:
             os.startfile(file_path)
 
             return None
 
     os.system(f"{bin_name} {file_path}")
```

### Comparing `fnschool-20240519.81611.835/src/fnschool/fnprint.py` & `fnschool-20240520.80901.843/src/fnschool/fnprint.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/language.py` & `fnschool-20240520.80901.843/src/fnschool/language.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240520.80901.843/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,17 +1,17 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  fnschool\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-05-19 16:09+0800\n"
-"PO-Revision-Date: 2024-05-19 16:10+0800\n"
+"POT-Creation-Date: 2024-05-20 07:36+0800\n"
+"PO-Revision-Date: 2024-05-20 07:36+0800\n"
 "Last-Translator: larryw3i <larryw3i@163.com>\n"
-"Language: en_US\n"
-"Language-Team: English - United States <larryw3i@163.com>\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: zh_CN\n"
+"Language-Team: Chinese - China <larryw3i@163.com>\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.15.0\n"
 
 msgid ""
 "\n"
@@ -176,14 +176,19 @@
 
 msgid "Got no purchased foods of time node %s ."
 msgstr "时间节点 %s 没有购入的食材。"
 
 msgid "Hello! helping information is here for you:"
 msgstr "您好！这里是给您的帮助信息："
 
+msgid ""
+"Hey! {0}, all of your files will be saved to {1}, show it now? (Yes: 'Y','y')"
+msgstr ""
+"您好～ {0}，您的所有文件将会被保存到 {1} 文件夹，打开它？（打开：“Y”、“y”）"
+
 msgid "Hi, your name is \"{0}\"? (Yes: 'Y' 'y' '', or enter your name)"
 msgstr "您好！您是 “{0}” 吗？（是：“Y”、“y”、“”，或者输入您的姓名）"
 
 msgid ""
 "If new Xuelan milks is purchased. you have to add the purchasing information "
 "of them into the end of the purchasing spreadsheet (e.g: the spreadsheets "
 "Changsheng provided)."
```

### Comparing `fnschool-20240519.81611.835/src/fnschool/path.py` & `fnschool-20240520.80901.843/src/fnschool/path.py`

 * *Files 25% similar despite different names*

```diff
@@ -36,25 +36,14 @@
     shutil.copy(config0_fpath, config_fpath)
     print_warning(
         _("Configuration file '%s' was copied to '%s'.")
         % (config0_fpath, config_fpath)
     )
 
 
-def make_link(src, link):
-    if isinstance(src, PosixPath):
-        src = src.as_posix()
-    if isinstance(link, PosixPath):
-        link = link.as_posix()
-
-    if not os.path.islink(link):
-        os.symlink(src, link, target_is_directory=os.path.isdir(src))
-    elif not os.readlink(link) == src:
-        os.remove(link)
-        os.symlink(src, link, target_is_directory=os.path.isdir(src))
 
 
 def open_sys_explorer(dest=None):
     sys_platform = platform.platform()
     explorer_bin = (
         "explorer"
         if "Windows" in sys_platform
```

### Comparing `fnschool-20240519.81611.835/src/fnschool/test.py` & `fnschool-20240520.80901.843/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240519.81611.835/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240520.80901.843/src/fnschool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240519.81611.835
+Version: 20240520.80901.843
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240519.81611.835/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240520.80901.843/src/fnschool.egg-info/SOURCES.txt`

 * *Files identical despite different names*


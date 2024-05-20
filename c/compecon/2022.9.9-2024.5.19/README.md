# Comparing `tmp/compecon-2022.9.9.tar.gz` & `tmp/compecon-2024.5.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compecon-2022.9.9.tar", last modified: Sat Sep 10 00:49:41 2022, max compression
+gzip compressed data, was "compecon-2024.5.19.tar", last modified: Mon May 20 01:06:28 2024, max compression
```

## Comparing `compecon-2022.9.9.tar` & `compecon-2024.5.19.tar`

### file list

```diff
@@ -1,121 +1,128 @@
-drwxrwxrwx   0        0        0        0 2022-09-10 00:49:41.792508 compecon-2022.9.9/
--rw-rw-rw-   0        0        0     1076 2018-04-29 02:22:55.000000 compecon-2022.9.9/LICENSE.txt
--rw-rw-rw-   0        0        0     2236 2022-09-10 00:49:41.792508 compecon-2022.9.9/PKG-INFO
--rw-rw-rw-   0        0        0     1719 2021-10-12 03:38:00.000000 compecon-2022.9.9/README.md
-drwxrwxrwx   0        0        0        0 2022-09-10 00:49:41.594230 compecon-2022.9.9/compecon/
--rw-rw-rw-   0        0        0      849 2021-09-27 18:01:48.000000 compecon-2022.9.9/compecon/__init__.py
--rw-rw-rw-   0        0        0    48601 2022-08-08 06:15:35.000000 compecon-2022.9.9/compecon/basis.py
--rw-rw-rw-   0        0        0     9418 2021-05-15 00:30:16.000000 compecon-2022.9.9/compecon/basisChebyshev.py
--rw-rw-rw-   0        0        0     6753 2022-09-08 22:53:00.000000 compecon-2022.9.9/compecon/basisLinear.py
--rw-rw-rw-   0        0        0    10236 2021-05-15 00:30:16.000000 compecon-2022.9.9/compecon/basisSpline.py
--rw-rw-rw-   0        0        0     2467 2015-04-12 19:30:47.000000 compecon-2022.9.9/compecon/ce_util.py
--rw-rw-rw-   0        0        0      908 2015-11-03 20:01:47.000000 compecon-2022.9.9/compecon/chebyc.py
--rw-rw-rw-   0        0        0     8269 2022-09-08 22:52:31.000000 compecon-2022.9.9/compecon/ddpmodel.py
-drwxrwxrwx   0        0        0        0 2022-09-10 00:49:41.779513 compecon-2022.9.9/compecon/demos/
--rw-rw-rw-   0        0        0     1074 2017-05-12 21:53:58.000000 compecon-2022.9.9/compecon/demos/__init__.py
--rw-rw-rw-   0        0        0     2347 2015-10-18 04:43:50.000000 compecon-2022.9.9/compecon/demos/dem01_basis.py
--rw-rw-rw-   0        0        0     2080 2015-10-21 04:20:58.000000 compecon-2022.9.9/compecon/demos/demapp00.py
--rw-rw-rw-   0        0        0     5337 2018-03-28 06:23:14.000000 compecon-2022.9.9/compecon/demos/demapp01.py
--rw-rw-rw-   0        0        0     6112 2018-03-28 00:30:37.000000 compecon-2022.9.9/compecon/demos/demapp02.py
--rw-rw-rw-   0        0        0     2038 2018-03-28 02:33:19.000000 compecon-2022.9.9/compecon/demos/demapp03.py
--rw-rw-rw-   0        0        0     3130 2018-03-27 22:10:41.000000 compecon-2022.9.9/compecon/demos/demapp04.py
--rw-rw-rw-   0        0        0     2092 2015-10-18 07:19:58.000000 compecon-2022.9.9/compecon/demos/demapp05.py
--rw-rw-rw-   0        0        0     2172 2015-11-04 03:25:57.000000 compecon-2022.9.9/compecon/demos/demapp06.py
--rw-rw-rw-   0        0        0     4797 2018-03-28 02:57:02.000000 compecon-2022.9.9/compecon/demos/demapp07.py
--rw-rw-rw-   0        0        0     1223 2018-03-27 22:56:23.000000 compecon-2022.9.9/compecon/demos/demapp08.py
--rw-rw-rw-   0        0        0     1150 2018-03-28 00:42:54.000000 compecon-2022.9.9/compecon/demos/demapp09.py
--rw-rw-rw-   0        0        0     1040 2018-03-28 00:47:25.000000 compecon-2022.9.9/compecon/demos/demapp10.py
--rw-rw-rw-   0        0        0     1420 2015-10-25 00:13:53.000000 compecon-2022.9.9/compecon/demos/demddp01.py
--rw-rw-rw-   0        0        0     1277 2015-10-25 00:13:53.000000 compecon-2022.9.9/compecon/demos/demddp02.py
--rw-rw-rw-   0        0        0     1624 2015-10-25 00:13:53.000000 compecon-2022.9.9/compecon/demos/demddp03.py
--rw-rw-rw-   0        0        0     1740 2015-10-25 00:13:53.000000 compecon-2022.9.9/compecon/demos/demddp04.py
--rw-rw-rw-   0        0        0     2306 2015-10-25 00:13:53.000000 compecon-2022.9.9/compecon/demos/demddp05.py
--rw-rw-rw-   0        0        0     1868 2015-10-25 00:13:53.000000 compecon-2022.9.9/compecon/demos/demddp06.py
--rw-rw-rw-   0        0        0     1929 2015-10-25 00:13:53.000000 compecon-2022.9.9/compecon/demos/demddp07.py
--rw-rw-rw-   0        0        0     1660 2015-10-20 21:09:59.000000 compecon-2022.9.9/compecon/demos/demddp08.py
--rw-rw-rw-   0        0        0     1308 2015-10-25 00:13:53.000000 compecon-2022.9.9/compecon/demos/demddp09.py
--rw-rw-rw-   0        0        0     2514 2015-10-25 00:13:53.000000 compecon-2022.9.9/compecon/demos/demddp10.py
--rw-rw-rw-   0        0        0     1911 2015-10-25 00:13:53.000000 compecon-2022.9.9/compecon/demos/demddp11.py
--rw-rw-rw-   0        0        0     1319 2018-03-27 18:19:28.000000 compecon-2022.9.9/compecon/demos/demdif02.py
--rw-rw-rw-   0        0        0     4219 2018-03-29 17:10:47.000000 compecon-2022.9.9/compecon/demos/demdp01.py
--rw-rw-rw-   0        0        0     2013 2018-03-30 21:31:09.000000 compecon-2022.9.9/compecon/demos/demdp01a.py
--rw-rw-rw-   0        0        0     1967 2018-03-30 22:59:49.000000 compecon-2022.9.9/compecon/demos/demdp01b.py
--rw-rw-rw-   0        0        0     5240 2018-03-30 23:06:51.000000 compecon-2022.9.9/compecon/demos/demdp02.py
--rw-rw-rw-   0        0        0     7394 2018-03-30 23:58:56.000000 compecon-2022.9.9/compecon/demos/demdp03.py
--rw-rw-rw-   0        0        0     6211 2018-03-31 00:05:30.000000 compecon-2022.9.9/compecon/demos/demdp04.py
--rw-rw-rw-   0        0        0     5715 2018-03-31 00:14:39.000000 compecon-2022.9.9/compecon/demos/demdp05.py
--rw-rw-rw-   0        0        0     4627 2016-02-17 19:36:39.000000 compecon-2022.9.9/compecon/demos/demdp06.py
--rw-rw-rw-   0        0        0     4776 2018-03-29 17:33:10.000000 compecon-2022.9.9/compecon/demos/demdp06borrar.py
--rw-rw-rw-   0        0        0     4623 2018-03-30 16:03:33.000000 compecon-2022.9.9/compecon/demos/demdp07.py
--rw-rw-rw-   0        0        0     3342 2018-03-30 16:03:33.000000 compecon-2022.9.9/compecon/demos/demdp08.py
--rw-rw-rw-   0        0        0     2634 2018-03-30 16:03:33.000000 compecon-2022.9.9/compecon/demos/demdp09.py
--rw-rw-rw-   0        0        0     4699 2018-03-30 16:03:33.000000 compecon-2022.9.9/compecon/demos/demdp10.py
--rw-rw-rw-   0        0        0     6499 2016-03-13 19:19:27.000000 compecon-2022.9.9/compecon/demos/demdp11.py
--rw-rw-rw-   0        0        0     4692 2018-03-30 16:03:33.000000 compecon-2022.9.9/compecon/demos/demdp12.py
--rw-rw-rw-   0        0        0     1720 2017-05-28 00:57:51.000000 compecon-2022.9.9/compecon/demos/demintro01.py
--rw-rw-rw-   0        0        0     4849 2017-05-28 02:20:07.000000 compecon-2022.9.9/compecon/demos/demintro02.py
--rw-rw-rw-   0        0        0      859 2015-10-15 01:02:44.000000 compecon-2022.9.9/compecon/demos/demlin01.py
--rw-rw-rw-   0        0        0     1151 2020-02-14 07:06:23.000000 compecon-2022.9.9/compecon/demos/demlin02.py
--rw-rw-rw-   0        0        0      935 2015-10-15 01:06:08.000000 compecon-2022.9.9/compecon/demos/demlin03.py
--rw-rw-rw-   0        0        0     1347 2017-09-18 06:10:55.000000 compecon-2022.9.9/compecon/demos/demmath01.py
--rw-rw-rw-   0        0        0     2274 2015-10-15 01:18:58.000000 compecon-2022.9.9/compecon/demos/demmath02.py
--rw-rw-rw-   0        0        0      867 2015-10-15 01:21:56.000000 compecon-2022.9.9/compecon/demos/demmath06.py
--rw-rw-rw-   0        0        0      518 2015-10-12 03:05:13.000000 compecon-2022.9.9/compecon/demos/demopt01.py
--rw-rw-rw-   0        0        0     2589 2018-03-26 17:33:23.000000 compecon-2022.9.9/compecon/demos/demopt04.py
--rw-rw-rw-   0        0        0     1584 2018-03-26 02:40:06.000000 compecon-2022.9.9/compecon/demos/demopt05.py
--rw-rw-rw-   0        0        0     1216 2018-03-26 19:09:46.000000 compecon-2022.9.9/compecon/demos/demopt06.py
--rw-rw-rw-   0        0        0     1204 2015-10-12 04:53:18.000000 compecon-2022.9.9/compecon/demos/demopt07.py
--rw-rw-rw-   0        0        0     1519 2018-03-26 17:31:01.000000 compecon-2022.9.9/compecon/demos/demopt08.py
--rw-rw-rw-   0        0        0      650 2018-03-27 15:17:55.000000 compecon-2022.9.9/compecon/demos/demqua01.py
--rw-rw-rw-   0        0        0     1368 2018-03-27 17:24:58.000000 compecon-2022.9.9/compecon/demos/demqua01bis.py
--rw-rw-rw-   0        0        0     1872 2018-03-27 02:09:48.000000 compecon-2022.9.9/compecon/demos/demqua03.py
--rw-rw-rw-   0        0        0      733 2018-03-26 20:16:46.000000 compecon-2022.9.9/compecon/demos/demqua04.py
--rw-rw-rw-   0        0        0      922 2018-03-26 21:57:19.000000 compecon-2022.9.9/compecon/demos/demqua06.py
--rw-rw-rw-   0        0        0      972 2018-03-26 23:18:24.000000 compecon-2022.9.9/compecon/demos/demqua07.py
--rw-rw-rw-   0        0        0     1311 2018-03-26 23:18:30.000000 compecon-2022.9.9/compecon/demos/demqua08.py
--rw-rw-rw-   0        0        0      524 2018-03-27 05:39:24.000000 compecon-2022.9.9/compecon/demos/demqua10.py
--rw-rw-rw-   0        0        0     1466 2015-11-04 17:26:57.000000 compecon-2022.9.9/compecon/demos/demslv01.py
--rw-rw-rw-   0        0        0     1390 2015-11-04 17:32:55.000000 compecon-2022.9.9/compecon/demos/demslv02.py
--rw-rw-rw-   0        0        0     1558 2015-11-04 18:41:18.000000 compecon-2022.9.9/compecon/demos/demslv03.py
--rw-rw-rw-   0        0        0     1980 2015-10-15 01:55:23.000000 compecon-2022.9.9/compecon/demos/demslv04.py
--rw-rw-rw-   0        0        0     1977 2017-05-29 00:41:39.000000 compecon-2022.9.9/compecon/demos/demslv05.py
--rw-rw-rw-   0        0        0     2252 2017-05-28 22:42:45.000000 compecon-2022.9.9/compecon/demos/demslv05bis.py
--rw-rw-rw-   0        0        0     3105 2017-05-28 22:05:36.000000 compecon-2022.9.9/compecon/demos/demslv06.py
--rw-rw-rw-   0        0        0     1331 2015-10-15 01:57:28.000000 compecon-2022.9.9/compecon/demos/demslv07.py
--rw-rw-rw-   0        0        0     2202 2015-10-15 01:58:20.000000 compecon-2022.9.9/compecon/demos/demslv08.py
--rw-rw-rw-   0        0        0     2835 2015-10-15 01:59:41.000000 compecon-2022.9.9/compecon/demos/demslv09.py
--rw-rw-rw-   0        0        0     1344 2018-03-25 20:04:07.000000 compecon-2022.9.9/compecon/demos/demslv10.py
--rw-rw-rw-   0        0        0     1633 2017-06-12 03:57:17.000000 compecon-2022.9.9/compecon/demos/demslv12.py
--rw-rw-rw-   0        0        0     1607 2018-03-25 23:33:35.000000 compecon-2022.9.9/compecon/demos/demslv14.py
--rw-rw-rw-   0        0        0     3820 2018-09-19 05:22:30.000000 compecon-2022.9.9/compecon/demos/setup.py
--rw-rw-rw-   0        0        0    10521 2015-10-10 00:04:22.000000 compecon-2022.9.9/compecon/demos/slv.py
--rw-rw-rw-   0        0        0     6615 2015-10-10 00:04:22.000000 compecon-2022.9.9/compecon/deprecated.py
--rw-rw-rw-   0        0        0    44884 2021-10-02 06:47:43.000000 compecon-2022.9.9/compecon/dpmodel.py
--rw-rw-rw-   0        0        0     8098 2015-10-26 00:27:23.000000 compecon-2022.9.9/compecon/interpolator.py
--rw-rw-rw-   0        0        0     8646 2015-10-26 00:27:23.000000 compecon-2022.9.9/compecon/interpolator_old.py
--rw-rw-rw-   0        0        0        0 2015-03-29 07:53:16.000000 compecon-2022.9.9/compecon/interpvec.py
--rw-rw-rw-   0        0        0     5679 2016-02-18 19:17:43.000000 compecon-2022.9.9/compecon/lcpstep.py
--rw-rw-rw-   0        0        0     1857 2019-07-24 19:11:38.000000 compecon-2022.9.9/compecon/linear.py
--rw-rw-rw-   0        0        0    11606 2018-03-31 20:15:48.000000 compecon-2022.9.9/compecon/lqmodel.py
--rw-rw-rw-   0        0        0    19526 2022-09-10 00:03:36.000000 compecon-2022.9.9/compecon/nonlinear.py
--rw-rw-rw-   0        0        0      689 2015-11-03 19:50:08.000000 compecon-2022.9.9/compecon/numbaclass.py
--rw-rw-rw-   0        0        0     5648 2021-10-02 06:47:43.000000 compecon-2022.9.9/compecon/ocmodel.py
--rw-rw-rw-   0        0        0     8770 2021-10-06 00:24:16.000000 compecon-2022.9.9/compecon/ode.py
--rw-rw-rw-   0        0        0    14266 2019-07-13 01:05:08.000000 compecon-2022.9.9/compecon/optimize.py
--rw-rw-rw-   0        0        0    30157 2021-05-15 00:41:05.000000 compecon-2022.9.9/compecon/quad.py
--rw-rw-rw-   0        0        0      150 2015-10-31 01:42:13.000000 compecon-2022.9.9/compecon/quadrature.py
--rw-rw-rw-   0        0        0     3807 2015-03-28 03:23:47.000000 compecon-2022.9.9/compecon/smolyak.py
--rw-rw-rw-   0        0        0    12518 2022-09-08 22:54:41.000000 compecon-2022.9.9/compecon/tools.py
-drwxrwxrwx   0        0        0        0 2022-09-10 00:49:41.624220 compecon-2022.9.9/compecon.egg-info/
--rw-rw-rw-   0        0        0     2236 2022-09-10 00:49:41.000000 compecon-2022.9.9/compecon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2889 2022-09-10 00:49:41.000000 compecon-2022.9.9/compecon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-10 00:49:41.000000 compecon-2022.9.9/compecon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2022-09-10 00:49:41.000000 compecon-2022.9.9/compecon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2022-09-10 00:49:41.000000 compecon-2022.9.9/compecon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-10 00:49:41.793508 compecon-2022.9.9/setup.cfg
--rw-rw-rw-   0        0        0     1022 2022-09-10 00:46:22.000000 compecon-2022.9.9/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-10 00:49:41.790509 compecon-2022.9.9/textbook/
--rw-rw-rw-   0        0        0      724 2015-10-09 09:03:29.000000 compecon-2022.9.9/textbook/chapter01.py
--rw-rw-rw-   0        0        0     7514 2015-10-26 00:27:23.000000 compecon-2022.9.9/textbook/chapter03.py
--rw-rw-rw-   0        0        0     4170 2015-10-22 19:40:12.000000 compecon-2022.9.9/textbook/chapter04.py
--rw-rw-rw-   0        0        0     3757 2015-10-22 19:40:12.000000 compecon-2022.9.9/textbook/chapter06.py
+drwxrwxrwx   0        0        0        0 2024-05-20 01:06:28.628465 compecon-2024.5.19/
+-rw-rw-rw-   0        0        0     1076 2018-04-29 02:22:55.000000 compecon-2024.5.19/LICENSE.txt
+-rw-rw-rw-   0        0        0     2237 2024-05-20 01:06:28.626441 compecon-2024.5.19/PKG-INFO
+-rw-rw-rw-   0        0        0     1719 2021-10-12 03:38:00.000000 compecon-2024.5.19/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 01:06:28.484858 compecon-2024.5.19/compecon/
+-rw-rw-rw-   0        0        0      849 2021-09-27 18:01:48.000000 compecon-2024.5.19/compecon/__init__.py
+-rw-rw-rw-   0        0        0    48595 2024-05-20 00:50:57.000000 compecon-2024.5.19/compecon/basis.py
+-rw-rw-rw-   0        0        0     9418 2021-05-15 00:30:16.000000 compecon-2024.5.19/compecon/basisChebyshev.py
+-rw-rw-rw-   0        0        0     6753 2022-09-08 22:53:00.000000 compecon-2024.5.19/compecon/basisLinear.py
+-rw-rw-rw-   0        0        0    10236 2021-05-15 00:30:16.000000 compecon-2024.5.19/compecon/basisSpline.py
+-rw-rw-rw-   0        0        0     2467 2015-04-12 19:30:47.000000 compecon-2024.5.19/compecon/ce_util.py
+-rw-rw-rw-   0        0        0      908 2015-11-03 20:01:47.000000 compecon-2024.5.19/compecon/chebyc.py
+-rw-rw-rw-   0        0        0     8269 2022-09-08 22:52:31.000000 compecon-2024.5.19/compecon/ddpmodel.py
+drwxrwxrwx   0        0        0        0 2024-05-20 01:06:28.606367 compecon-2024.5.19/compecon/demos/
+-rw-rw-rw-   0        0        0     1074 2017-05-12 21:53:58.000000 compecon-2024.5.19/compecon/demos/__init__.py
+-rw-rw-rw-   0        0        0     2347 2015-10-18 04:43:50.000000 compecon-2024.5.19/compecon/demos/dem01_basis.py
+-rw-rw-rw-   0        0        0     2080 2015-10-21 04:20:58.000000 compecon-2024.5.19/compecon/demos/demapp00.py
+-rw-rw-rw-   0        0        0     5337 2018-03-28 06:23:14.000000 compecon-2024.5.19/compecon/demos/demapp01.py
+-rw-rw-rw-   0        0        0     6112 2018-03-28 00:30:37.000000 compecon-2024.5.19/compecon/demos/demapp02.py
+-rw-rw-rw-   0        0        0     2038 2018-03-28 02:33:19.000000 compecon-2024.5.19/compecon/demos/demapp03.py
+-rw-rw-rw-   0        0        0     3130 2018-03-27 22:10:41.000000 compecon-2024.5.19/compecon/demos/demapp04.py
+-rw-rw-rw-   0        0        0     2092 2015-10-18 07:19:58.000000 compecon-2024.5.19/compecon/demos/demapp05.py
+-rw-rw-rw-   0        0        0     2172 2015-11-04 03:25:57.000000 compecon-2024.5.19/compecon/demos/demapp06.py
+-rw-rw-rw-   0        0        0     4797 2018-03-28 02:57:02.000000 compecon-2024.5.19/compecon/demos/demapp07.py
+-rw-rw-rw-   0        0        0     1223 2018-03-27 22:56:23.000000 compecon-2024.5.19/compecon/demos/demapp08.py
+-rw-rw-rw-   0        0        0     1150 2018-03-28 00:42:54.000000 compecon-2024.5.19/compecon/demos/demapp09.py
+-rw-rw-rw-   0        0        0     1040 2018-03-28 00:47:25.000000 compecon-2024.5.19/compecon/demos/demapp10.py
+-rw-rw-rw-   0        0        0     1420 2015-10-25 00:13:53.000000 compecon-2024.5.19/compecon/demos/demddp01.py
+-rw-rw-rw-   0        0        0     1277 2015-10-25 00:13:53.000000 compecon-2024.5.19/compecon/demos/demddp02.py
+-rw-rw-rw-   0        0        0     1624 2015-10-25 00:13:53.000000 compecon-2024.5.19/compecon/demos/demddp03.py
+-rw-rw-rw-   0        0        0     1740 2015-10-25 00:13:53.000000 compecon-2024.5.19/compecon/demos/demddp04.py
+-rw-rw-rw-   0        0        0     2306 2015-10-25 00:13:53.000000 compecon-2024.5.19/compecon/demos/demddp05.py
+-rw-rw-rw-   0        0        0     1868 2015-10-25 00:13:53.000000 compecon-2024.5.19/compecon/demos/demddp06.py
+-rw-rw-rw-   0        0        0     1929 2015-10-25 00:13:53.000000 compecon-2024.5.19/compecon/demos/demddp07.py
+-rw-rw-rw-   0        0        0     1660 2015-10-20 21:09:59.000000 compecon-2024.5.19/compecon/demos/demddp08.py
+-rw-rw-rw-   0        0        0     1308 2015-10-25 00:13:53.000000 compecon-2024.5.19/compecon/demos/demddp09.py
+-rw-rw-rw-   0        0        0     2514 2015-10-25 00:13:53.000000 compecon-2024.5.19/compecon/demos/demddp10.py
+-rw-rw-rw-   0        0        0     1911 2015-10-25 00:13:53.000000 compecon-2024.5.19/compecon/demos/demddp11.py
+-rw-rw-rw-   0        0        0     1319 2018-03-27 18:19:28.000000 compecon-2024.5.19/compecon/demos/demdif02.py
+-rw-rw-rw-   0        0        0     4219 2018-03-29 17:10:47.000000 compecon-2024.5.19/compecon/demos/demdp01.py
+-rw-rw-rw-   0        0        0     2013 2018-03-30 21:31:09.000000 compecon-2024.5.19/compecon/demos/demdp01a.py
+-rw-rw-rw-   0        0        0     1967 2018-03-30 22:59:49.000000 compecon-2024.5.19/compecon/demos/demdp01b.py
+-rw-rw-rw-   0        0        0     5240 2018-03-30 23:06:51.000000 compecon-2024.5.19/compecon/demos/demdp02.py
+-rw-rw-rw-   0        0        0     7394 2018-03-30 23:58:56.000000 compecon-2024.5.19/compecon/demos/demdp03.py
+-rw-rw-rw-   0        0        0     6211 2018-03-31 00:05:30.000000 compecon-2024.5.19/compecon/demos/demdp04.py
+-rw-rw-rw-   0        0        0     5715 2018-03-31 00:14:39.000000 compecon-2024.5.19/compecon/demos/demdp05.py
+-rw-rw-rw-   0        0        0     4627 2016-02-17 19:36:39.000000 compecon-2024.5.19/compecon/demos/demdp06.py
+-rw-rw-rw-   0        0        0     4776 2018-03-29 17:33:10.000000 compecon-2024.5.19/compecon/demos/demdp06borrar.py
+-rw-rw-rw-   0        0        0     4623 2018-03-30 16:03:33.000000 compecon-2024.5.19/compecon/demos/demdp07.py
+-rw-rw-rw-   0        0        0     3342 2018-03-30 16:03:33.000000 compecon-2024.5.19/compecon/demos/demdp08.py
+-rw-rw-rw-   0        0        0     2634 2018-03-30 16:03:33.000000 compecon-2024.5.19/compecon/demos/demdp09.py
+-rw-rw-rw-   0        0        0     4699 2018-03-30 16:03:33.000000 compecon-2024.5.19/compecon/demos/demdp10.py
+-rw-rw-rw-   0        0        0     6499 2016-03-13 19:19:27.000000 compecon-2024.5.19/compecon/demos/demdp11.py
+-rw-rw-rw-   0        0        0     4692 2018-03-30 16:03:33.000000 compecon-2024.5.19/compecon/demos/demdp12.py
+-rw-rw-rw-   0        0        0     1720 2017-05-28 00:57:51.000000 compecon-2024.5.19/compecon/demos/demintro01.py
+-rw-rw-rw-   0        0        0     4849 2017-05-28 02:20:07.000000 compecon-2024.5.19/compecon/demos/demintro02.py
+-rw-rw-rw-   0        0        0      859 2015-10-15 01:02:44.000000 compecon-2024.5.19/compecon/demos/demlin01.py
+-rw-rw-rw-   0        0        0     1151 2020-02-14 07:06:23.000000 compecon-2024.5.19/compecon/demos/demlin02.py
+-rw-rw-rw-   0        0        0      935 2015-10-15 01:06:08.000000 compecon-2024.5.19/compecon/demos/demlin03.py
+-rw-rw-rw-   0        0        0     1347 2017-09-18 06:10:55.000000 compecon-2024.5.19/compecon/demos/demmath01.py
+-rw-rw-rw-   0        0        0     2274 2015-10-15 01:18:58.000000 compecon-2024.5.19/compecon/demos/demmath02.py
+-rw-rw-rw-   0        0        0      867 2015-10-15 01:21:56.000000 compecon-2024.5.19/compecon/demos/demmath06.py
+-rw-rw-rw-   0        0        0      518 2015-10-12 03:05:13.000000 compecon-2024.5.19/compecon/demos/demopt01.py
+-rw-rw-rw-   0        0        0     2589 2018-03-26 17:33:23.000000 compecon-2024.5.19/compecon/demos/demopt04.py
+-rw-rw-rw-   0        0        0     1584 2018-03-26 02:40:06.000000 compecon-2024.5.19/compecon/demos/demopt05.py
+-rw-rw-rw-   0        0        0     1216 2018-03-26 19:09:46.000000 compecon-2024.5.19/compecon/demos/demopt06.py
+-rw-rw-rw-   0        0        0     1204 2015-10-12 04:53:18.000000 compecon-2024.5.19/compecon/demos/demopt07.py
+-rw-rw-rw-   0        0        0     1519 2018-03-26 17:31:01.000000 compecon-2024.5.19/compecon/demos/demopt08.py
+-rw-rw-rw-   0        0        0      650 2018-03-27 15:17:55.000000 compecon-2024.5.19/compecon/demos/demqua01.py
+-rw-rw-rw-   0        0        0     1368 2018-03-27 17:24:58.000000 compecon-2024.5.19/compecon/demos/demqua01bis.py
+-rw-rw-rw-   0        0        0     1872 2018-03-27 02:09:48.000000 compecon-2024.5.19/compecon/demos/demqua03.py
+-rw-rw-rw-   0        0        0      733 2018-03-26 20:16:46.000000 compecon-2024.5.19/compecon/demos/demqua04.py
+-rw-rw-rw-   0        0        0      922 2018-03-26 21:57:19.000000 compecon-2024.5.19/compecon/demos/demqua06.py
+-rw-rw-rw-   0        0        0      972 2018-03-26 23:18:24.000000 compecon-2024.5.19/compecon/demos/demqua07.py
+-rw-rw-rw-   0        0        0     1311 2018-03-26 23:18:30.000000 compecon-2024.5.19/compecon/demos/demqua08.py
+-rw-rw-rw-   0        0        0      524 2018-03-27 05:39:24.000000 compecon-2024.5.19/compecon/demos/demqua10.py
+-rw-rw-rw-   0        0        0     1466 2015-11-04 17:26:57.000000 compecon-2024.5.19/compecon/demos/demslv01.py
+-rw-rw-rw-   0        0        0     1390 2015-11-04 17:32:55.000000 compecon-2024.5.19/compecon/demos/demslv02.py
+-rw-rw-rw-   0        0        0     1558 2015-11-04 18:41:18.000000 compecon-2024.5.19/compecon/demos/demslv03.py
+-rw-rw-rw-   0        0        0     1980 2015-10-15 01:55:23.000000 compecon-2024.5.19/compecon/demos/demslv04.py
+-rw-rw-rw-   0        0        0     1977 2017-05-29 00:41:39.000000 compecon-2024.5.19/compecon/demos/demslv05.py
+-rw-rw-rw-   0        0        0     2252 2017-05-28 22:42:45.000000 compecon-2024.5.19/compecon/demos/demslv05bis.py
+-rw-rw-rw-   0        0        0     3105 2017-05-28 22:05:36.000000 compecon-2024.5.19/compecon/demos/demslv06.py
+-rw-rw-rw-   0        0        0     1331 2015-10-15 01:57:28.000000 compecon-2024.5.19/compecon/demos/demslv07.py
+-rw-rw-rw-   0        0        0     2202 2015-10-15 01:58:20.000000 compecon-2024.5.19/compecon/demos/demslv08.py
+-rw-rw-rw-   0        0        0     2835 2015-10-15 01:59:41.000000 compecon-2024.5.19/compecon/demos/demslv09.py
+-rw-rw-rw-   0        0        0     1344 2018-03-25 20:04:07.000000 compecon-2024.5.19/compecon/demos/demslv10.py
+-rw-rw-rw-   0        0        0     1633 2017-06-12 03:57:17.000000 compecon-2024.5.19/compecon/demos/demslv12.py
+-rw-rw-rw-   0        0        0     1607 2018-03-25 23:33:35.000000 compecon-2024.5.19/compecon/demos/demslv14.py
+-rw-rw-rw-   0        0        0     3820 2018-09-19 05:22:30.000000 compecon-2024.5.19/compecon/demos/setup.py
+-rw-rw-rw-   0        0        0    10521 2015-10-10 00:04:22.000000 compecon-2024.5.19/compecon/demos/slv.py
+-rw-rw-rw-   0        0        0     6615 2015-10-10 00:04:22.000000 compecon-2024.5.19/compecon/deprecated.py
+-rw-rw-rw-   0        0        0    44854 2024-05-20 00:57:04.000000 compecon-2024.5.19/compecon/dpmodel.py
+-rw-rw-rw-   0        0        0     8098 2015-10-26 00:27:23.000000 compecon-2024.5.19/compecon/interpolator.py
+-rw-rw-rw-   0        0        0     8646 2015-10-26 00:27:23.000000 compecon-2024.5.19/compecon/interpolator_old.py
+-rw-rw-rw-   0        0        0        0 2015-03-29 07:53:16.000000 compecon-2024.5.19/compecon/interpvec.py
+-rw-rw-rw-   0        0        0     5679 2016-02-18 19:17:43.000000 compecon-2024.5.19/compecon/lcpstep.py
+-rw-rw-rw-   0        0        0     1857 2019-07-24 19:11:38.000000 compecon-2024.5.19/compecon/linear.py
+-rw-rw-rw-   0        0        0    11606 2018-03-31 20:15:48.000000 compecon-2024.5.19/compecon/lqmodel.py
+-rw-rw-rw-   0        0        0    19526 2022-09-10 00:03:36.000000 compecon-2024.5.19/compecon/nonlinear.py
+-rw-rw-rw-   0        0        0      689 2015-11-03 19:50:08.000000 compecon-2024.5.19/compecon/numbaclass.py
+-rw-rw-rw-   0        0        0     5648 2021-10-02 06:47:43.000000 compecon-2024.5.19/compecon/ocmodel.py
+-rw-rw-rw-   0        0        0     8770 2021-10-06 00:24:16.000000 compecon-2024.5.19/compecon/ode.py
+-rw-rw-rw-   0        0        0    14266 2019-07-13 01:05:08.000000 compecon-2024.5.19/compecon/optimize.py
+-rw-rw-rw-   0        0        0    30157 2021-05-15 00:41:05.000000 compecon-2024.5.19/compecon/quad.py
+-rw-rw-rw-   0        0        0      150 2015-10-31 01:42:13.000000 compecon-2024.5.19/compecon/quadrature.py
+-rw-rw-rw-   0        0        0     3807 2015-03-28 03:23:47.000000 compecon-2024.5.19/compecon/smolyak.py
+-rw-rw-rw-   0        0        0    12520 2024-05-20 01:01:07.000000 compecon-2024.5.19/compecon/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-20 01:06:28.500871 compecon-2024.5.19/compecon.egg-info/
+-rw-rw-rw-   0        0        0     2237 2024-05-20 01:06:28.000000 compecon-2024.5.19/compecon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3025 2024-05-20 01:06:28.000000 compecon-2024.5.19/compecon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 01:06:28.000000 compecon-2024.5.19/compecon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 01:06:28.000000 compecon-2024.5.19/compecon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-05-20 01:06:28.000000 compecon-2024.5.19/compecon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 01:06:28.628465 compecon-2024.5.19/setup.cfg
+-rw-rw-rw-   0        0        0     1022 2024-05-20 01:04:57.000000 compecon-2024.5.19/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 01:06:28.617462 compecon-2024.5.19/tests/
+-rw-rw-rw-   0        0        0      153 2015-04-09 06:54:12.000000 compecon-2024.5.19/tests/test_Smolyak.py
+-rw-rw-rw-   0        0        0     2865 2015-11-03 20:43:54.000000 compecon-2024.5.19/tests/test_basis.py
+-rw-rw-rw-   0        0        0     1294 2015-03-31 21:40:05.000000 compecon-2024.5.19/tests/test_basis01.py
+-rw-rw-rw-   0        0        0      495 2015-10-17 05:43:44.000000 compecon-2024.5.19/tests/test_basisChebyshev.py
+-rw-rw-rw-   0        0        0      125 2015-11-04 00:12:50.000000 compecon-2024.5.19/tests/test_demddp.py
+-rw-rw-rw-   0        0        0      698 2015-04-15 21:22:55.000000 compecon-2024.5.19/tests/test_lcpstep.py
+drwxrwxrwx   0        0        0        0 2024-05-20 01:06:28.625465 compecon-2024.5.19/textbook/
+-rw-rw-rw-   0        0        0      724 2015-10-09 09:03:29.000000 compecon-2024.5.19/textbook/chapter01.py
+-rw-rw-rw-   0        0        0     7514 2015-10-26 00:27:23.000000 compecon-2024.5.19/textbook/chapter03.py
+-rw-rw-rw-   0        0        0     4170 2015-10-22 19:40:12.000000 compecon-2024.5.19/textbook/chapter04.py
+-rw-rw-rw-   0        0        0     3757 2015-10-22 19:40:12.000000 compecon-2024.5.19/textbook/chapter06.py
```

### Comparing `compecon-2022.9.9/LICENSE.txt` & `compecon-2024.5.19/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/PKG-INFO` & `compecon-2024.5.19/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compecon
-Version: 2022.9.9
+Version: 2024.5.19
 Summary: A Computational Economics Toolbox
 Home-page: http://randall-romero.com/code/compecon
 Author: Randall Romero-Aguilar
 Author-email: randall.romero@outlook.com
 Project-URL: Bug Reports, https://github.com/randall-romero/CompEcon/issues
 Project-URL: Source, https://github.com/randall-romero/CompEcon/
 Keywords: computations economics numerical methods
```

### Comparing `compecon-2022.9.9/README.md` & `compecon-2024.5.19/README.md`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/__init__.py` & `compecon-2024.5.19/compecon/__init__.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/basis.py` & `compecon-2024.5.19/compecon/basis.py`

 * *Files 0% similar despite different names*

```diff
@@ -699,15 +699,15 @@
             try:
                 cPhix = np.array([self.c * phix.T for phix in Phix])
             except:
                 cPhix = np.array([np.dot(self.c, phix.T.toarray()) for phix in Phix])
 
         def clean(A):
             A = np.squeeze(A) if dropdim else A
-            return np.asscalar(A) if (A.size == 1 and dropdim) else A
+            return A.item() if (A.size == 1 and dropdim) else A
 
 
         if order in ['none', 'provided', 'jac']:
             return clean(cPhix)
         elif order in ['fjac']:
             return clean(cPhix[0]), clean(cPhix[1:])
         elif order in ['hess', 'all']:
```

### Comparing `compecon-2022.9.9/compecon/basisChebyshev.py` & `compecon-2024.5.19/compecon/basisChebyshev.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/basisLinear.py` & `compecon-2024.5.19/compecon/basisLinear.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/basisSpline.py` & `compecon-2024.5.19/compecon/basisSpline.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/ce_util.py` & `compecon-2024.5.19/compecon/ce_util.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/chebyc.py` & `compecon-2024.5.19/compecon/chebyc.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/ddpmodel.py` & `compecon-2024.5.19/compecon/ddpmodel.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/__init__.py` & `compecon-2024.5.19/compecon/demos/__init__.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/dem01_basis.py` & `compecon-2024.5.19/compecon/demos/dem01_basis.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demapp00.py` & `compecon-2024.5.19/compecon/demos/demapp00.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demapp01.py` & `compecon-2024.5.19/compecon/demos/demapp01.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demapp02.py` & `compecon-2024.5.19/compecon/demos/demapp02.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demapp03.py` & `compecon-2024.5.19/compecon/demos/demapp03.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demapp04.py` & `compecon-2024.5.19/compecon/demos/demapp04.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demapp05.py` & `compecon-2024.5.19/compecon/demos/demapp05.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demapp06.py` & `compecon-2024.5.19/compecon/demos/demapp06.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demapp07.py` & `compecon-2024.5.19/compecon/demos/demapp07.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demapp08.py` & `compecon-2024.5.19/compecon/demos/demapp08.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demapp09.py` & `compecon-2024.5.19/compecon/demos/demapp09.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demapp10.py` & `compecon-2024.5.19/compecon/demos/demapp10.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demddp01.py` & `compecon-2024.5.19/compecon/demos/demddp01.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demddp02.py` & `compecon-2024.5.19/compecon/demos/demddp02.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demddp03.py` & `compecon-2024.5.19/compecon/demos/demddp03.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demddp04.py` & `compecon-2024.5.19/compecon/demos/demddp04.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demddp05.py` & `compecon-2024.5.19/compecon/demos/demddp05.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demddp06.py` & `compecon-2024.5.19/compecon/demos/demddp06.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demddp07.py` & `compecon-2024.5.19/compecon/demos/demddp07.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demddp08.py` & `compecon-2024.5.19/compecon/demos/demddp08.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demddp09.py` & `compecon-2024.5.19/compecon/demos/demddp09.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demddp10.py` & `compecon-2024.5.19/compecon/demos/demddp10.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demddp11.py` & `compecon-2024.5.19/compecon/demos/demddp11.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demdif02.py` & `compecon-2024.5.19/compecon/demos/demdif02.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demdp01.py` & `compecon-2024.5.19/compecon/demos/demdp01.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demdp01a.py` & `compecon-2024.5.19/compecon/demos/demdp01a.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demdp01b.py` & `compecon-2024.5.19/compecon/demos/demdp01b.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demdp02.py` & `compecon-2024.5.19/compecon/demos/demdp02.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demdp03.py` & `compecon-2024.5.19/compecon/demos/demdp03.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demdp04.py` & `compecon-2024.5.19/compecon/demos/demdp04.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demdp05.py` & `compecon-2024.5.19/compecon/demos/demdp05.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demdp06.py` & `compecon-2024.5.19/compecon/demos/demdp06.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demdp06borrar.py` & `compecon-2024.5.19/compecon/demos/demdp06borrar.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demdp07.py` & `compecon-2024.5.19/compecon/demos/demdp07.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demdp08.py` & `compecon-2024.5.19/compecon/demos/demdp08.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demdp09.py` & `compecon-2024.5.19/compecon/demos/demdp09.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demdp10.py` & `compecon-2024.5.19/compecon/demos/demdp10.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demdp11.py` & `compecon-2024.5.19/compecon/demos/demdp11.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demdp12.py` & `compecon-2024.5.19/compecon/demos/demdp12.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demintro01.py` & `compecon-2024.5.19/compecon/demos/demintro01.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demintro02.py` & `compecon-2024.5.19/compecon/demos/demintro02.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demlin01.py` & `compecon-2024.5.19/compecon/demos/demlin01.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demlin02.py` & `compecon-2024.5.19/compecon/demos/demlin02.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demlin03.py` & `compecon-2024.5.19/compecon/demos/demlin03.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demmath01.py` & `compecon-2024.5.19/compecon/demos/demmath01.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demmath02.py` & `compecon-2024.5.19/compecon/demos/demmath02.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demmath06.py` & `compecon-2024.5.19/compecon/demos/demmath06.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demopt01.py` & `compecon-2024.5.19/compecon/demos/demopt01.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demopt04.py` & `compecon-2024.5.19/compecon/demos/demopt04.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demopt05.py` & `compecon-2024.5.19/compecon/demos/demopt05.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demopt06.py` & `compecon-2024.5.19/compecon/demos/demopt06.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demopt07.py` & `compecon-2024.5.19/compecon/demos/demopt07.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demopt08.py` & `compecon-2024.5.19/compecon/demos/demopt08.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demqua01.py` & `compecon-2024.5.19/compecon/demos/demqua01.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demqua01bis.py` & `compecon-2024.5.19/compecon/demos/demqua01bis.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demqua03.py` & `compecon-2024.5.19/compecon/demos/demqua03.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demqua04.py` & `compecon-2024.5.19/compecon/demos/demqua04.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demqua06.py` & `compecon-2024.5.19/compecon/demos/demqua06.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demqua07.py` & `compecon-2024.5.19/compecon/demos/demqua07.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demqua08.py` & `compecon-2024.5.19/compecon/demos/demqua08.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demqua10.py` & `compecon-2024.5.19/compecon/demos/demqua10.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demslv01.py` & `compecon-2024.5.19/compecon/demos/demslv01.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demslv02.py` & `compecon-2024.5.19/compecon/demos/demslv02.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demslv03.py` & `compecon-2024.5.19/compecon/demos/demslv03.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demslv04.py` & `compecon-2024.5.19/compecon/demos/demslv04.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demslv05.py` & `compecon-2024.5.19/compecon/demos/demslv05.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demslv05bis.py` & `compecon-2024.5.19/compecon/demos/demslv05bis.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demslv06.py` & `compecon-2024.5.19/compecon/demos/demslv06.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demslv07.py` & `compecon-2024.5.19/compecon/demos/demslv07.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demslv08.py` & `compecon-2024.5.19/compecon/demos/demslv08.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demslv09.py` & `compecon-2024.5.19/compecon/demos/demslv09.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demslv10.py` & `compecon-2024.5.19/compecon/demos/demslv10.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demslv12.py` & `compecon-2024.5.19/compecon/demos/demslv12.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/demslv14.py` & `compecon-2024.5.19/compecon/demos/demslv14.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/setup.py` & `compecon-2024.5.19/compecon/demos/setup.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/demos/slv.py` & `compecon-2024.5.19/compecon/demos/slv.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/deprecated.py` & `compecon-2024.5.19/compecon/deprecated.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/dpmodel.py` & `compecon-2024.5.19/compecon/dpmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from compecon.lqmodel import LQmodel
 import numpy as np
 import scipy as sp
 import pandas as pd
 from scipy.sparse import block_diag, kron, issparse, identity
 from scipy.sparse.linalg import spsolve
 from compecon.tools import jacobian, hessian, gridmake, indices
-from inspect import getargspec
+
 #from .lcpstep import lcpstep  # todo: is it worth to add lcpstep?
 import warnings
 
 
 #fixme In docstrings, indicate that discrete model should not include x in definitions
 
 __author__ = 'Randall'
```

### Comparing `compecon-2022.9.9/compecon/interpolator.py` & `compecon-2024.5.19/compecon/interpolator.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/interpolator_old.py` & `compecon-2024.5.19/compecon/interpolator_old.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/lcpstep.py` & `compecon-2024.5.19/compecon/lcpstep.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/linear.py` & `compecon-2024.5.19/compecon/linear.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/lqmodel.py` & `compecon-2024.5.19/compecon/lqmodel.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/nonlinear.py` & `compecon-2024.5.19/compecon/nonlinear.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/numbaclass.py` & `compecon-2024.5.19/compecon/numbaclass.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/ocmodel.py` & `compecon-2024.5.19/compecon/ocmodel.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/ode.py` & `compecon-2024.5.19/compecon/ode.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/optimize.py` & `compecon-2024.5.19/compecon/optimize.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/quad.py` & `compecon-2024.5.19/compecon/quad.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/smolyak.py` & `compecon-2024.5.19/compecon/smolyak.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/compecon/tools.py` & `compecon-2024.5.19/compecon/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     """
     if len(arrays) == 1:
         return arrays[0]
 
     arrays = np.atleast_2d(*arrays)
     n = len(arrays)
     idx = np.indices([a.shape[1] for a in arrays]).reshape([n, -1])
-    return np.vstack(arrays[k][:, idx[k]] for k in range(n))
+    return np.vstack([arrays[k][:, idx[k]] for k in range(n)])
 
 
 def indices(*args):
     return np.array([a.flatten() for a in np.indices(args)])
 
 
 def ckron(*arrays, invert=False):
```

### Comparing `compecon-2022.9.9/compecon.egg-info/PKG-INFO` & `compecon-2024.5.19/compecon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compecon
-Version: 2022.9.9
+Version: 2024.5.19
 Summary: A Computational Economics Toolbox
 Home-page: http://randall-romero.com/code/compecon
 Author: Randall Romero-Aguilar
 Author-email: randall.romero@outlook.com
 Project-URL: Bug Reports, https://github.com/randall-romero/CompEcon/issues
 Project-URL: Source, https://github.com/randall-romero/CompEcon/
 Keywords: computations economics numerical methods
```

### Comparing `compecon-2022.9.9/compecon.egg-info/SOURCES.txt` & `compecon-2024.5.19/compecon.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -104,11 +104,17 @@
 compecon/demos/demslv08.py
 compecon/demos/demslv09.py
 compecon/demos/demslv10.py
 compecon/demos/demslv12.py
 compecon/demos/demslv14.py
 compecon/demos/setup.py
 compecon/demos/slv.py
+tests/test_Smolyak.py
+tests/test_basis.py
+tests/test_basis01.py
+tests/test_basisChebyshev.py
+tests/test_demddp.py
+tests/test_lcpstep.py
 textbook/chapter01.py
 textbook/chapter03.py
 textbook/chapter04.py
 textbook/chapter06.py
```

### Comparing `compecon-2022.9.9/setup.py` & `compecon-2024.5.19/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """ The CompEcon package setup.
 Based on setuptools
 
-Randall Romero-Aguilar, 2015-2022
+Randall Romero-Aguilar, 2015-2024
 """
 
 
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='compecon',
-    version='2022.09.09',
+    version='2024.05.19',
     description='A Computational Economics Toolbox',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='http://randall-romero.com/code/compecon',
     author='Randall Romero-Aguilar',
     author_email='randall.romero@outlook.com',
     keywords='computations economics numerical methods',
```

### Comparing `compecon-2022.9.9/textbook/chapter01.py` & `compecon-2024.5.19/textbook/chapter01.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/textbook/chapter03.py` & `compecon-2024.5.19/textbook/chapter03.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/textbook/chapter04.py` & `compecon-2024.5.19/textbook/chapter04.py`

 * *Files identical despite different names*

### Comparing `compecon-2022.9.9/textbook/chapter06.py` & `compecon-2024.5.19/textbook/chapter06.py`

 * *Files identical despite different names*


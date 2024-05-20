# Comparing `tmp/pyDecision-4.5.4.tar.gz` & `tmp/pyDecision-4.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyDecision-4.5.4.tar", last modified: Sun Apr 28 14:56:17 2024, max compression
+gzip compressed data, was "dist\pyDecision-4.5.5.tar", last modified: Mon May 20 01:14:40 2024, max compression
```

## Comparing `pyDecision-4.5.4.tar` & `pyDecision-4.5.5.tar`

### file list

```diff
@@ -1,101 +1,103 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 14:56:17.000000 pyDecision-4.5.4/
--rw-rw-rw-   0        0        0      656 2023-10-24 20:28:27.000000 pyDecision-4.5.4/LICENSE
--rw-rw-rw-   0        0        0    20622 2024-04-28 14:56:17.000000 pyDecision-4.5.4/PKG-INFO
--rw-rw-rw-   0        0        0    20118 2024-04-28 14:54:36.000000 pyDecision-4.5.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 14:56:16.000000 pyDecision-4.5.4/pyDecision/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-4.5.4/pyDecision/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 14:56:17.000000 pyDecision-4.5.4/pyDecision/algorithm/
--rw-rw-rw-   0        0        0     3266 2024-04-28 14:43:26.000000 pyDecision-4.5.4/pyDecision/algorithm/__init__.py
--rw-rw-rw-   0        0        0     1638 2023-08-15 11:11:40.000000 pyDecision-4.5.4/pyDecision/algorithm/ahp.py
--rw-rw-rw-   0        0        0     2591 2023-07-21 17:32:54.000000 pyDecision-4.5.4/pyDecision/algorithm/aras.py
--rw-rw-rw-   0        0        0     2147 2023-07-21 20:21:53.000000 pyDecision-4.5.4/pyDecision/algorithm/borda.py
--rw-rw-rw-   0        0        0     2553 2023-11-10 15:52:16.000000 pyDecision-4.5.4/pyDecision/algorithm/bwm.py
--rw-rw-rw-   0        0        0     1006 2023-11-12 15:54:44.000000 pyDecision-4.5.4/pyDecision/algorithm/bwm_s.py
--rw-rw-rw-   0        0        0     1221 2024-04-24 14:49:40.000000 pyDecision-4.5.4/pyDecision/algorithm/cilos.py
--rw-rw-rw-   0        0        0     2762 2023-07-22 02:44:56.000000 pyDecision-4.5.4/pyDecision/algorithm/cocoso.py
--rw-rw-rw-   0        0        0     2754 2023-07-21 17:33:49.000000 pyDecision-4.5.4/pyDecision/algorithm/codas.py
--rw-rw-rw-   0        0        0     2870 2023-07-23 17:00:58.000000 pyDecision-4.5.4/pyDecision/algorithm/copeland.py
--rw-rw-rw-   0        0        0     2471 2023-07-21 17:34:03.000000 pyDecision-4.5.4/pyDecision/algorithm/copras.py
--rw-rw-rw-   0        0        0     2347 2023-07-23 16:38:01.000000 pyDecision-4.5.4/pyDecision/algorithm/cradis.py
--rw-rw-rw-   0        0        0     1125 2023-10-24 20:07:49.000000 pyDecision-4.5.4/pyDecision/algorithm/critic.py
--rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-4.5.4/pyDecision/algorithm/dematel.py
--rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-4.5.4/pyDecision/algorithm/e_i.py
--rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-4.5.4/pyDecision/algorithm/e_i_s.py
--rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-4.5.4/pyDecision/algorithm/e_i_v.py
--rw-rw-rw-   0        0        0    16907 2023-07-21 20:38:15.000000 pyDecision-4.5.4/pyDecision/algorithm/e_ii.py
--rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-4.5.4/pyDecision/algorithm/e_iii.py
--rw-rw-rw-   0        0        0    14298 2023-07-21 19:41:40.000000 pyDecision-4.5.4/pyDecision/algorithm/e_iv.py
--rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-4.5.4/pyDecision/algorithm/e_tri_b.py
--rw-rw-rw-   0        0        0     2711 2023-07-21 20:33:16.000000 pyDecision-4.5.4/pyDecision/algorithm/edas.py
--rw-rw-rw-   0        0        0      925 2023-07-19 01:09:53.000000 pyDecision-4.5.4/pyDecision/algorithm/entropy.py
--rw-rw-rw-   0        0        0     2289 2024-04-24 15:29:47.000000 pyDecision-4.5.4/pyDecision/algorithm/fucom.py
--rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-4.5.4/pyDecision/algorithm/fuzzy_ahp.py
--rw-rw-rw-   0        0        0     3321 2023-07-25 15:17:23.000000 pyDecision-4.5.4/pyDecision/algorithm/fuzzy_aras.py
--rw-rw-rw-   0        0        0     4635 2023-11-12 11:24:00.000000 pyDecision-4.5.4/pyDecision/algorithm/fuzzy_bwm.py
--rw-rw-rw-   0        0        0     4545 2023-07-21 17:31:44.000000 pyDecision-4.5.4/pyDecision/algorithm/fuzzy_copras.py
--rw-rw-rw-   0        0        0     2500 2024-04-26 21:40:48.000000 pyDecision-4.5.4/pyDecision/algorithm/fuzzy_critic.py
--rw-rw-rw-   0        0        0     4100 2023-08-01 01:06:41.000000 pyDecision-4.5.4/pyDecision/algorithm/fuzzy_dematel.py
--rw-rw-rw-   0        0        0     5042 2023-07-21 18:03:22.000000 pyDecision-4.5.4/pyDecision/algorithm/fuzzy_edas.py
--rw-rw-rw-   0        0        0     5402 2024-04-27 00:21:30.000000 pyDecision-4.5.4/pyDecision/algorithm/fuzzy_fucom.py
--rw-rw-rw-   0        0        0     1786 2024-04-26 21:41:04.000000 pyDecision-4.5.4/pyDecision/algorithm/fuzzy_merec.py
--rw-rw-rw-   0        0        0     3706 2023-07-21 18:11:21.000000 pyDecision-4.5.4/pyDecision/algorithm/fuzzy_moora.py
--rw-rw-rw-   0        0        0     4098 2023-07-21 18:13:14.000000 pyDecision-4.5.4/pyDecision/algorithm/fuzzy_ocra.py
--rw-rw-rw-   0        0        0     4086 2023-07-21 18:17:14.000000 pyDecision-4.5.4/pyDecision/algorithm/fuzzy_topsis.py
--rw-rw-rw-   0        0        0     5994 2023-07-21 18:18:25.000000 pyDecision-4.5.4/pyDecision/algorithm/fuzzy_vikor.py
--rw-rw-rw-   0        0        0     5399 2023-09-09 01:09:43.000000 pyDecision-4.5.4/pyDecision/algorithm/fuzzy_waspas.py
--rw-rw-rw-   0        0        0     2553 2023-07-22 02:46:58.000000 pyDecision-4.5.4/pyDecision/algorithm/gra.py
--rw-rw-rw-   0        0        0     2300 2023-10-26 23:42:55.000000 pyDecision-4.5.4/pyDecision/algorithm/idocriw.py
--rw-rw-rw-   0        0        0     2585 2023-07-21 18:06:06.000000 pyDecision-4.5.4/pyDecision/algorithm/mabac.py
--rw-rw-rw-   0        0        0     2388 2023-07-28 22:31:36.000000 pyDecision-4.5.4/pyDecision/algorithm/macbeth.py
--rw-rw-rw-   0        0        0     2575 2023-07-23 16:39:11.000000 pyDecision-4.5.4/pyDecision/algorithm/mairca.py
--rw-rw-rw-   0        0        0     2598 2024-04-25 15:20:07.000000 pyDecision-4.5.4/pyDecision/algorithm/mara.py
--rw-rw-rw-   0        0        0     3048 2023-07-21 18:09:18.000000 pyDecision-4.5.4/pyDecision/algorithm/marcos.py
--rw-rw-rw-   0        0        0     3766 2023-07-22 02:46:58.000000 pyDecision-4.5.4/pyDecision/algorithm/maut.py
--rw-rw-rw-   0        0        0     1175 2023-10-26 23:47:00.000000 pyDecision-4.5.4/pyDecision/algorithm/merec.py
--rw-rw-rw-   0        0        0     2541 2023-07-21 18:10:51.000000 pyDecision-4.5.4/pyDecision/algorithm/moora.py
--rw-rw-rw-   0        0        0     2549 2023-07-21 18:12:07.000000 pyDecision-4.5.4/pyDecision/algorithm/moosra.py
--rw-rw-rw-   0        0        0     4968 2023-07-22 01:50:19.000000 pyDecision-4.5.4/pyDecision/algorithm/multimoora.py
--rw-rw-rw-   0        0        0     2477 2023-07-21 23:26:24.000000 pyDecision-4.5.4/pyDecision/algorithm/ocra.py
--rw-rw-rw-   0        0        0     2563 2023-09-09 00:46:31.000000 pyDecision-4.5.4/pyDecision/algorithm/oreste.py
--rw-rw-rw-   0        0        0    13836 2023-10-30 12:17:12.000000 pyDecision-4.5.4/pyDecision/algorithm/p_ec.py
--rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-4.5.4/pyDecision/algorithm/p_i.py
--rw-rw-rw-   0        0        0     5891 2023-07-21 19:40:41.000000 pyDecision-4.5.4/pyDecision/algorithm/p_ii.py
--rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-4.5.4/pyDecision/algorithm/p_iii.py
--rw-rw-rw-   0        0        0     8547 2023-07-21 19:39:42.000000 pyDecision-4.5.4/pyDecision/algorithm/p_iv.py
--rw-rw-rw-   0        0        0     6622 2023-08-02 21:49:15.000000 pyDecision-4.5.4/pyDecision/algorithm/p_v.py
--rw-rw-rw-   0        0        0     9380 2023-07-21 19:37:53.000000 pyDecision-4.5.4/pyDecision/algorithm/p_vi.py
--rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-4.5.4/pyDecision/algorithm/p_xgaia.py
--rw-rw-rw-   0        0        0     2139 2023-07-23 16:40:26.000000 pyDecision-4.5.4/pyDecision/algorithm/piv.py
--rw-rw-rw-   0        0        0     2184 2023-07-21 18:14:04.000000 pyDecision-4.5.4/pyDecision/algorithm/psi.py
--rw-rw-rw-   0        0        0      688 2024-04-25 15:23:46.000000 pyDecision-4.5.4/pyDecision/algorithm/psi_m.py
--rw-rw-rw-   0        0        0     3243 2024-04-28 14:55:21.000000 pyDecision-4.5.4/pyDecision/algorithm/rafsi.py
--rw-rw-rw-   0        0        0     5265 2024-04-25 14:52:15.000000 pyDecision-4.5.4/pyDecision/algorithm/regime.py
--rw-rw-rw-   0        0        0      969 2024-04-26 21:38:23.000000 pyDecision-4.5.4/pyDecision/algorithm/roc.py
--rw-rw-rw-   0        0        0     2434 2023-07-22 02:08:59.000000 pyDecision-4.5.4/pyDecision/algorithm/rov.py
--rw-rw-rw-   0        0        0      970 2024-04-26 21:39:12.000000 pyDecision-4.5.4/pyDecision/algorithm/rrw.py
--rw-rw-rw-   0        0        0      929 2024-04-26 21:38:49.000000 pyDecision-4.5.4/pyDecision/algorithm/rsw.py
--rw-rw-rw-   0        0        0     2130 2023-07-21 18:14:55.000000 pyDecision-4.5.4/pyDecision/algorithm/saw.py
--rw-rw-rw-   0        0        0     1991 2024-04-27 19:45:13.000000 pyDecision-4.5.4/pyDecision/algorithm/seca.py
--rw-rw-rw-   0        0        0     2344 2023-07-21 18:15:17.000000 pyDecision-4.5.4/pyDecision/algorithm/smart.py
--rw-rw-rw-   0        0        0     2185 2023-08-02 00:35:27.000000 pyDecision-4.5.4/pyDecision/algorithm/spotis.py
--rw-rw-rw-   0        0        0     2867 2023-07-21 18:15:39.000000 pyDecision-4.5.4/pyDecision/algorithm/todim.py
--rw-rw-rw-   0        0        0     2600 2023-07-21 18:16:04.000000 pyDecision-4.5.4/pyDecision/algorithm/topsis.py
--rw-rw-rw-   0        0        0     3703 2023-07-22 03:11:26.000000 pyDecision-4.5.4/pyDecision/algorithm/vikor.py
--rw-rw-rw-   0        0        0     4278 2023-09-08 23:55:42.000000 pyDecision-4.5.4/pyDecision/algorithm/waspas.py
--rw-rw-rw-   0        0        0     2643 2023-07-21 18:23:36.000000 pyDecision-4.5.4/pyDecision/algorithm/wings.py
--rw-rw-rw-   0        0        0     3188 2024-04-24 01:11:01.000000 pyDecision-4.5.4/pyDecision/algorithm/wisp.py
-drwxrwxrwx   0        0        0        0 2024-04-28 14:56:17.000000 pyDecision-4.5.4/pyDecision/compare/
--rw-rw-rw-   0        0        0      127 2024-04-27 00:17:39.000000 pyDecision-4.5.4/pyDecision/compare/__init__.py
--rw-rw-rw-   0        0        0    26816 2024-04-28 14:47:45.000000 pyDecision-4.5.4/pyDecision/compare/compare.py
-drwxrwxrwx   0        0        0        0 2024-04-28 14:56:17.000000 pyDecision-4.5.4/pyDecision/util/
--rw-rw-rw-   0        0        0     8733 2023-12-03 18:26:24.000000 pyDecision-4.5.4/pyDecision/util/LLM.py
--rw-rw-rw-   0        0        0      109 2023-08-02 19:44:51.000000 pyDecision-4.5.4/pyDecision/util/__init__.py
--rw-rw-rw-   0        0        0     6266 2023-08-02 19:44:27.000000 pyDecision-4.5.4/pyDecision/util/ga.py
-drwxrwxrwx   0        0        0        0 2024-04-28 14:56:16.000000 pyDecision-4.5.4/pyDecision.egg-info/
--rw-rw-rw-   0        0        0    20622 2024-04-28 14:56:15.000000 pyDecision-4.5.4/pyDecision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2801 2024-04-28 14:56:15.000000 pyDecision-4.5.4/pyDecision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 14:56:15.000000 pyDecision-4.5.4/pyDecision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-28 14:56:15.000000 pyDecision-4.5.4/pyDecision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-28 14:56:15.000000 pyDecision-4.5.4/pyDecision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 14:56:17.000000 pyDecision-4.5.4/setup.cfg
--rw-rw-rw-   0        0        0      744 2024-04-28 14:48:12.000000 pyDecision-4.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 01:14:40.000000 pyDecision-4.5.5/
+-rw-rw-rw-   0        0        0      656 2023-10-24 20:28:27.000000 pyDecision-4.5.5/LICENSE
+-rw-rw-rw-   0        0        0    21036 2024-05-20 01:14:40.000000 pyDecision-4.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0    20530 2024-05-20 01:12:36.000000 pyDecision-4.5.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 01:14:39.000000 pyDecision-4.5.5/pyDecision/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-4.5.5/pyDecision/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 01:14:40.000000 pyDecision-4.5.5/pyDecision/algorithm/
+-rw-rw-rw-   0        0        0     3346 2024-05-20 01:04:37.000000 pyDecision-4.5.5/pyDecision/algorithm/__init__.py
+-rw-rw-rw-   0        0        0     1667 2024-05-18 20:21:19.000000 pyDecision-4.5.5/pyDecision/algorithm/ahp.py
+-rw-rw-rw-   0        0        0     2591 2023-07-21 17:32:54.000000 pyDecision-4.5.5/pyDecision/algorithm/aras.py
+-rw-rw-rw-   0        0        0     2147 2023-07-21 20:21:53.000000 pyDecision-4.5.5/pyDecision/algorithm/borda.py
+-rw-rw-rw-   0        0        0     2553 2023-11-10 15:52:16.000000 pyDecision-4.5.5/pyDecision/algorithm/bwm.py
+-rw-rw-rw-   0        0        0     1006 2023-11-12 15:54:44.000000 pyDecision-4.5.5/pyDecision/algorithm/bwm_s.py
+-rw-rw-rw-   0        0        0     1221 2024-04-24 14:49:40.000000 pyDecision-4.5.5/pyDecision/algorithm/cilos.py
+-rw-rw-rw-   0        0        0     2762 2023-07-22 02:44:56.000000 pyDecision-4.5.5/pyDecision/algorithm/cocoso.py
+-rw-rw-rw-   0        0        0     2754 2023-07-21 17:33:49.000000 pyDecision-4.5.5/pyDecision/algorithm/codas.py
+-rw-rw-rw-   0        0        0     2870 2023-07-23 17:00:58.000000 pyDecision-4.5.5/pyDecision/algorithm/copeland.py
+-rw-rw-rw-   0        0        0     2471 2023-07-21 17:34:03.000000 pyDecision-4.5.5/pyDecision/algorithm/copras.py
+-rw-rw-rw-   0        0        0     2347 2023-07-23 16:38:01.000000 pyDecision-4.5.5/pyDecision/algorithm/cradis.py
+-rw-rw-rw-   0        0        0     1125 2023-10-24 20:07:49.000000 pyDecision-4.5.5/pyDecision/algorithm/critic.py
+-rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-4.5.5/pyDecision/algorithm/dematel.py
+-rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-4.5.5/pyDecision/algorithm/e_i.py
+-rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-4.5.5/pyDecision/algorithm/e_i_s.py
+-rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-4.5.5/pyDecision/algorithm/e_i_v.py
+-rw-rw-rw-   0        0        0    16907 2023-07-21 20:38:15.000000 pyDecision-4.5.5/pyDecision/algorithm/e_ii.py
+-rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-4.5.5/pyDecision/algorithm/e_iii.py
+-rw-rw-rw-   0        0        0    14298 2023-07-21 19:41:40.000000 pyDecision-4.5.5/pyDecision/algorithm/e_iv.py
+-rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-4.5.5/pyDecision/algorithm/e_tri_b.py
+-rw-rw-rw-   0        0        0     2764 2024-05-16 23:15:46.000000 pyDecision-4.5.5/pyDecision/algorithm/edas.py
+-rw-rw-rw-   0        0        0      925 2023-07-19 01:09:53.000000 pyDecision-4.5.5/pyDecision/algorithm/entropy.py
+-rw-rw-rw-   0        0        0     2289 2024-04-24 15:29:47.000000 pyDecision-4.5.5/pyDecision/algorithm/fucom.py
+-rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_ahp.py
+-rw-rw-rw-   0        0        0     2873 2024-05-20 00:52:49.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_ahp_ppf.py
+-rw-rw-rw-   0        0        0     3321 2023-07-25 15:17:23.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_aras.py
+-rw-rw-rw-   0        0        0     4635 2023-11-12 11:24:00.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_bwm.py
+-rw-rw-rw-   0        0        0     4545 2023-07-21 17:31:44.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_copras.py
+-rw-rw-rw-   0        0        0     2500 2024-04-26 21:40:48.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_critic.py
+-rw-rw-rw-   0        0        0     4100 2023-08-01 01:06:41.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_dematel.py
+-rw-rw-rw-   0        0        0     5042 2023-07-21 18:03:22.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_edas.py
+-rw-rw-rw-   0        0        0     5402 2024-04-27 00:21:30.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_fucom.py
+-rw-rw-rw-   0        0        0     1786 2024-04-26 21:41:04.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_merec.py
+-rw-rw-rw-   0        0        0     3706 2023-07-21 18:11:21.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_moora.py
+-rw-rw-rw-   0        0        0     4098 2023-07-21 18:13:14.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_ocra.py
+-rw-rw-rw-   0        0        0     4086 2023-07-21 18:17:14.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_topsis.py
+-rw-rw-rw-   0        0        0     5994 2023-07-21 18:18:25.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_vikor.py
+-rw-rw-rw-   0        0        0     5399 2023-09-09 01:09:43.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_waspas.py
+-rw-rw-rw-   0        0        0     2553 2023-07-22 02:46:58.000000 pyDecision-4.5.5/pyDecision/algorithm/gra.py
+-rw-rw-rw-   0        0        0     2300 2023-10-26 23:42:55.000000 pyDecision-4.5.5/pyDecision/algorithm/idocriw.py
+-rw-rw-rw-   0        0        0     2585 2023-07-21 18:06:06.000000 pyDecision-4.5.5/pyDecision/algorithm/mabac.py
+-rw-rw-rw-   0        0        0     2388 2023-07-28 22:31:36.000000 pyDecision-4.5.5/pyDecision/algorithm/macbeth.py
+-rw-rw-rw-   0        0        0     2575 2023-07-23 16:39:11.000000 pyDecision-4.5.5/pyDecision/algorithm/mairca.py
+-rw-rw-rw-   0        0        0     2598 2024-04-25 15:20:07.000000 pyDecision-4.5.5/pyDecision/algorithm/mara.py
+-rw-rw-rw-   0        0        0     3048 2023-07-21 18:09:18.000000 pyDecision-4.5.5/pyDecision/algorithm/marcos.py
+-rw-rw-rw-   0        0        0     3766 2023-07-22 02:46:58.000000 pyDecision-4.5.5/pyDecision/algorithm/maut.py
+-rw-rw-rw-   0        0        0     1175 2023-10-26 23:47:00.000000 pyDecision-4.5.5/pyDecision/algorithm/merec.py
+-rw-rw-rw-   0        0        0     2541 2023-07-21 18:10:51.000000 pyDecision-4.5.5/pyDecision/algorithm/moora.py
+-rw-rw-rw-   0        0        0     2549 2023-07-21 18:12:07.000000 pyDecision-4.5.5/pyDecision/algorithm/moosra.py
+-rw-rw-rw-   0        0        0     4968 2023-07-22 01:50:19.000000 pyDecision-4.5.5/pyDecision/algorithm/multimoora.py
+-rw-rw-rw-   0        0        0     2477 2023-07-21 23:26:24.000000 pyDecision-4.5.5/pyDecision/algorithm/ocra.py
+-rw-rw-rw-   0        0        0     5101 2024-05-20 01:01:36.000000 pyDecision-4.5.5/pyDecision/algorithm/opa.py
+-rw-rw-rw-   0        0        0     2563 2023-09-09 00:46:31.000000 pyDecision-4.5.5/pyDecision/algorithm/oreste.py
+-rw-rw-rw-   0        0        0    13836 2023-10-30 12:17:12.000000 pyDecision-4.5.5/pyDecision/algorithm/p_ec.py
+-rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-4.5.5/pyDecision/algorithm/p_i.py
+-rw-rw-rw-   0        0        0     5891 2023-07-21 19:40:41.000000 pyDecision-4.5.5/pyDecision/algorithm/p_ii.py
+-rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-4.5.5/pyDecision/algorithm/p_iii.py
+-rw-rw-rw-   0        0        0     8547 2023-07-21 19:39:42.000000 pyDecision-4.5.5/pyDecision/algorithm/p_iv.py
+-rw-rw-rw-   0        0        0     6622 2023-08-02 21:49:15.000000 pyDecision-4.5.5/pyDecision/algorithm/p_v.py
+-rw-rw-rw-   0        0        0     9380 2023-07-21 19:37:53.000000 pyDecision-4.5.5/pyDecision/algorithm/p_vi.py
+-rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-4.5.5/pyDecision/algorithm/p_xgaia.py
+-rw-rw-rw-   0        0        0     2139 2023-07-23 16:40:26.000000 pyDecision-4.5.5/pyDecision/algorithm/piv.py
+-rw-rw-rw-   0        0        0     2184 2023-07-21 18:14:04.000000 pyDecision-4.5.5/pyDecision/algorithm/psi.py
+-rw-rw-rw-   0        0        0      688 2024-04-25 15:23:46.000000 pyDecision-4.5.5/pyDecision/algorithm/psi_m.py
+-rw-rw-rw-   0        0        0     3243 2024-04-28 14:55:21.000000 pyDecision-4.5.5/pyDecision/algorithm/rafsi.py
+-rw-rw-rw-   0        0        0     5265 2024-04-25 14:52:15.000000 pyDecision-4.5.5/pyDecision/algorithm/regime.py
+-rw-rw-rw-   0        0        0      969 2024-04-26 21:38:23.000000 pyDecision-4.5.5/pyDecision/algorithm/roc.py
+-rw-rw-rw-   0        0        0     2434 2023-07-22 02:08:59.000000 pyDecision-4.5.5/pyDecision/algorithm/rov.py
+-rw-rw-rw-   0        0        0      970 2024-04-26 21:39:12.000000 pyDecision-4.5.5/pyDecision/algorithm/rrw.py
+-rw-rw-rw-   0        0        0      929 2024-04-26 21:38:49.000000 pyDecision-4.5.5/pyDecision/algorithm/rsw.py
+-rw-rw-rw-   0        0        0     2130 2023-07-21 18:14:55.000000 pyDecision-4.5.5/pyDecision/algorithm/saw.py
+-rw-rw-rw-   0        0        0     1991 2024-04-27 19:45:13.000000 pyDecision-4.5.5/pyDecision/algorithm/seca.py
+-rw-rw-rw-   0        0        0     2344 2023-07-21 18:15:17.000000 pyDecision-4.5.5/pyDecision/algorithm/smart.py
+-rw-rw-rw-   0        0        0     2185 2023-08-02 00:35:27.000000 pyDecision-4.5.5/pyDecision/algorithm/spotis.py
+-rw-rw-rw-   0        0        0     2867 2023-07-21 18:15:39.000000 pyDecision-4.5.5/pyDecision/algorithm/todim.py
+-rw-rw-rw-   0        0        0     2600 2023-07-21 18:16:04.000000 pyDecision-4.5.5/pyDecision/algorithm/topsis.py
+-rw-rw-rw-   0        0        0     3703 2023-07-22 03:11:26.000000 pyDecision-4.5.5/pyDecision/algorithm/vikor.py
+-rw-rw-rw-   0        0        0     4278 2023-09-08 23:55:42.000000 pyDecision-4.5.5/pyDecision/algorithm/waspas.py
+-rw-rw-rw-   0        0        0     2687 2024-05-01 01:06:43.000000 pyDecision-4.5.5/pyDecision/algorithm/wings.py
+-rw-rw-rw-   0        0        0     3188 2024-04-24 01:11:01.000000 pyDecision-4.5.5/pyDecision/algorithm/wisp.py
+drwxrwxrwx   0        0        0        0 2024-05-20 01:14:40.000000 pyDecision-4.5.5/pyDecision/compare/
+-rw-rw-rw-   0        0        0      127 2024-04-27 00:17:39.000000 pyDecision-4.5.5/pyDecision/compare/__init__.py
+-rw-rw-rw-   0        0        0    26816 2024-04-28 14:47:45.000000 pyDecision-4.5.5/pyDecision/compare/compare.py
+drwxrwxrwx   0        0        0        0 2024-05-20 01:14:40.000000 pyDecision-4.5.5/pyDecision/util/
+-rw-rw-rw-   0        0        0     8733 2023-12-03 18:26:24.000000 pyDecision-4.5.5/pyDecision/util/LLM.py
+-rw-rw-rw-   0        0        0      109 2023-08-02 19:44:51.000000 pyDecision-4.5.5/pyDecision/util/__init__.py
+-rw-rw-rw-   0        0        0     6266 2023-08-02 19:44:27.000000 pyDecision-4.5.5/pyDecision/util/ga.py
+drwxrwxrwx   0        0        0        0 2024-05-20 01:14:39.000000 pyDecision-4.5.5/pyDecision.egg-info/
+-rw-rw-rw-   0        0        0    21036 2024-05-20 01:14:37.000000 pyDecision-4.5.5/pyDecision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2867 2024-05-20 01:14:38.000000 pyDecision-4.5.5/pyDecision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 01:14:37.000000 pyDecision-4.5.5/pyDecision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-20 01:14:37.000000 pyDecision-4.5.5/pyDecision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-20 01:14:37.000000 pyDecision-4.5.5/pyDecision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 01:14:40.000000 pyDecision-4.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      744 2024-05-20 01:05:15.000000 pyDecision-4.5.5/setup.py
```

### Comparing `pyDecision-4.5.4/LICENSE` & `pyDecision-4.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/PKG-INFO` & `pyDecision-4.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 4.5.4
+Version: 4.5.5
 Summary: A MCDA Library Incorporating a Large Language Model to Enhance Decision Analysis
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **Fuzzy CRITIC**; **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **Fuzzy FUCOM**; **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **RAFSI** (Ranking of Alternatives through Functional mapping of criterion sub-intervals into a Single Interval); **REGIME** (REGIonal Multicriteria Elimination); **ROC** (Rank Ordered Centroid); **ROV** (Range Of Value); **RRW** (Rank Reciprocal Weighting); **RSW** (Rank Summed Weight); **SAW** (Simple Additive Weighting); **SECA** (Simultaneous Evaluation of Criteria and Alternatives); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **Fuzzy WASPAS**; **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**. 
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **PPF AHP** (Proportional Picture Fuzzy AHP); **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **Fuzzy CRITIC**; **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **Fuzzy FUCOM**; **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **OPA** (Ordinal Priority Approach); **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **RAFSI** (Ranking of Alternatives through Functional mapping of criterion sub-intervals into a Single Interval); **REGIME** (REGIonal Multicriteria Elimination); **ROC** (Rank Ordered Centroid); **ROV** (Range Of Value); **RRW** (Rank Reciprocal Weighting); **RSW** (Rank Summed Weight); **SAW** (Simple Additive Weighting); **SECA** (Simultaneous Evaluation of Criteria and Alternatives); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **Fuzzy WASPAS**. 
 
 pyDecision offers an array of features, including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
 
 ## Citation
 
 PEREIRA, V.; BASILIO, M.P.; SANTOS, C.H.T (2024). Enhancing Decision Analysis with a Large Language Model: pyDecision a Comprehensive Library of MCDA Methods in Python. arXiv. https://arxiv.org/abs/2404.06370
 
@@ -66,14 +66,15 @@
 
 ```
 
 3. Try it in **Colab**:
 
 - AHP ([ Colab Demo ](https://colab.research.google.com/drive/1qwFQs5xkTZ8K-Ul_wWcCtPjLH0QooU9g?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/0377-2217(90)90057-I))
 - Fuzzy AHP ([ Colab Demo ](https://colab.research.google.com/drive/1RtEMOLGL5wtmheMRZv8emcO5wbjYVBCo?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0165-0114(83)80082-7))
+- PPF AHP ([ Colab Demo ](https://colab.research.google.com/drive/1wI-8z2aysGKhSI3PLxN6vOZ4jsbPmKYl?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2023.122354))
 - ARAS ([ Colab Demo ](https://colab.research.google.com/drive/1rwQgXjvC3E6pRhOs7CkcCV8Vw2bXEPLy?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/tede.2010.10))
 - Fuzzy ARAS ([ Colab Demo ](https://colab.research.google.com/drive/1kZDkEWsw0d0nFhDQQk8azZXRod7RnfZr?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/transport.2010.52))
 - Borda ([ Colab Demo ](https://colab.research.google.com/drive/1t5RVtG7_yXK-nPxM0MVd4U01qfTQYW4k?usp=sharing)) ( [ Paper ](http://gerardgreco.free.fr/IMG/pdf/MA_c_moire-Borda-1781.pdf))
 - BWM ([ Colab Demo ](https://colab.research.google.com/drive/1XkacTmtSBvZmx_5K9cfz8t1Ao5j-D-bZ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.omega.2014.11.009))
 - Simplified BWM ([ Colab Demo ](https://colab.research.google.com/drive/1v3QfSdprM8gwxL4VWmh75mPiPn2YWOZn?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/su13084487))
 - Fuzzy BWM ([ Colab Demo ](https://colab.research.google.com/drive/1hBTXyOLpBoC7oE-hsolPH2O0ekzp4VU0?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.knosys.2017.01.010))
 - CILOS ([ Colab Demo ](https://colab.research.google.com/drive/1RnSqO_VEPyvXAMHdneloYvA0TzPx55kw?usp=sharing)) ( [ Paper ](https://doi.org/10.1142/S0219622016500036))
@@ -111,14 +112,15 @@
 - Fuzzy MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1yJ1eOXoGNp3amhoyBtEFCXr5PqwI9S5T?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/math11061544))
 - MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1FpKl0QAdwGgCVvLYsRHvMWhz7yOp17B5?usp=sharing)) ( [ Paper ](http://matwbn.icm.edu.pl/ksiazki/cc/cc35/cc35213.pdf))
 - Fuzzy MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1ydHzGeA8WBVY5Gyu8K7Oq6kofQ5XbK3P?usp=sharing)) ( [ Paper ](https://pdfs.semanticscholar.org/6d33/ca3f14c9ed44d23742fd4e9cf94cebcaf148.pdf))
 - MOOSRA ([ Colab Demo ](https://colab.research.google.com/drive/1KYyA4f3OsipPA5e63Ja4A0OGmHvNY6dj?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.15623/ijret.2014.0315105))
 - MULTIMOORA ([ Colab Demo ](https://colab.research.google.com/drive/1JAT8qqHPNoFfMV6a-CzF6BgRwtcUF3-e?usp=sharing)) ( [ Paper ](https://journals.vilniustech.lt/index.php/TEDE/article/view/5832/5078))
 - OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1yQ41lOdjhiANtD1SOXoxA7gVim7A4X4P?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.5937/sjm10-6802))
 - Fuzzy OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1SniY4RLsR6jR9SnI3AR9k0wGlBWH6Pm8?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.5755/j01.ee.30.5.20546))
+- OPA ([ Colab Demo ](https://colab.research.google.com/drive/1RjryznPElHZUTuXQ2-ZKwJqMAVfJWKDC?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.asoc.2019.105893))
 - ORESTE ([ Colab Demo ](https://colab.research.google.com/drive/1USVCt6KJHJK9NXaknY8wTA4L0d4r2kWw?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0377-2217(82)90131-X))
 - PIV ([ Colab Demo ](https://colab.research.google.com/drive/1PwJoBqYn1O2s22MqC9euP89Uyv4sedS0?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.cie.2018.03.045))
 - PROMETHEE I    ([ Colab Demo ](https://colab.research.google.com/drive/1WsagC7-Y_5X-Xl90pMz8YwUkKfxf2vol?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE II   ([ Colab Demo ](https://colab.research.google.com/drive/143TUtTBy9y6gW0kMVAfhANBhuw1bKvBB?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE III  ([ Colab Demo ](https://colab.research.google.com/drive/11DBaEBBT8B-B3poXubvZ41HELOHok0Rz?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-030-15009-9_5
 ))
 - PROMETHEE IV   ([ Colab Demo ](https://colab.research.google.com/drive/1X2evE6pIf4F7qiKjt1fSU2PqT-NaA5sJ?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-319-11949-6_14))
@@ -140,17 +142,17 @@
 - SPOTIS ([ Colab Demo ](https://colab.research.google.com/drive/1TyjDn-xwut3w6Rf0zMiugdwytwmGY_NE?usp=sharing)) ( [ Paper ](https://doi.org/10.23919/FUSION45008.2020.9190347))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2007.10.046))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0377-2217(03)00020-1))
 - Fuzzy VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1anfCnU2TSrW-Z5vMkS_qXFrYZ0ciQE53?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2011.04.097))
 - WINGS ([ Colab Demo ](https://colab.research.google.com/drive/1li1_cPxwEM3NOZ4hbI8RROXyOmXeoWew?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2013.02.007))
+- WISP, Simple WISP ([ Colab Demo ](https://colab.research.google.com/drive/1xyJf3aydLdVPqhWpNyVXXD8T4PsrX0du?usp=sharing)) ( [ Paper ](https://doi.org/10.1109/TEM.2021.3075783))
 - WSM, WPM, WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1HbLwXI4HkrmI-lsNzDtBOlCiwxfJltHi?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.acme.2013.07.006))
 - Fuzzy WSM, Fuzzy WPM, Fuzzy WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1PcN_PaXwPHawzCU05UiHE504SkgF6vQ2?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.15837/ijccc.2015.6.2078))
-- WISP, Simple WISP ([ Colab Demo ](https://colab.research.google.com/drive/1xyJf3aydLdVPqhWpNyVXXD8T4PsrX0du?usp=sharing)) ( [ Paper ](https://doi.org/10.1109/TEM.2021.3075783))
 
 4. Compare Methods:
 - Compare Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1RfLNEJjaHjtn3Lb2cfEDqS-iblaC4GQZ?usp=sharing))
 - Compare Fuzzy Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1pRO-E9xnk6DYEj_0DaEHUrUiCeIjmnXx?usp=sharing))
 - Compare Weights & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/169hTJxP2APHrDA1h0fD1YEeu9s29wu0T?usp=sharing))
 - Compare Fuzzy Weights & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1nWDF8lrTmXlc-TE4_X1-MPhraFjytj1Z?usp=sharing))
 
@@ -159,10 +161,10 @@
 - [3MOAHP](https://github.com/Valdecy/Method_3MOAHP) - Inconsistency Reduction Technique for AHP and Fuzzy-AHP Methods
 - [pyMissingAHP](https://github.com/Valdecy/pyMissingAHP) - A Method to Infer AHP Missing Pairwise Comparisons
 - [ELECTRE-Tree](https://github.com/Valdecy/ELECTRE-Tree) - Algorithm to infer the ELECTRE Tri-B method parameters
 - [Ranking-Trees](https://github.com/Valdecy/Ranking-Trees) - Algorithm to infer the ELECTRE II, III, IV, and PROMETHEE I, II, III, IV method parameters
 
 # Acknowledgement 
 
-This section is dedicated to all the people who helped to improve or correct the code. Thank you very much!
+This section is dedicated to everyone who helped improve or correct the code. Thank you very much!
 
 * Sabir Mohammedi Taieb (23.JANUARY.2023) - https://sabir97.github.io/ - UniversitÃ© Abdelhamid Ibn Badis Mostaganem (Algeria)
```

### Comparing `pyDecision-4.5.4/README.md` & `pyDecision-4.5.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **Fuzzy CRITIC**; **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **Fuzzy FUCOM**; **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **RAFSI** (Ranking of Alternatives through Functional mapping of criterion sub-intervals into a Single Interval); **REGIME** (REGIonal Multicriteria Elimination); **ROC** (Rank Ordered Centroid); **ROV** (Range Of Value); **RRW** (Rank Reciprocal Weighting); **RSW** (Rank Summed Weight); **SAW** (Simple Additive Weighting); **SECA** (Simultaneous Evaluation of Criteria and Alternatives); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **Fuzzy WASPAS**; **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**. 
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **PPF AHP** (Proportional Picture Fuzzy AHP); **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **Fuzzy CRITIC**; **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **Fuzzy FUCOM**; **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **OPA** (Ordinal Priority Approach); **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **RAFSI** (Ranking of Alternatives through Functional mapping of criterion sub-intervals into a Single Interval); **REGIME** (REGIonal Multicriteria Elimination); **ROC** (Rank Ordered Centroid); **ROV** (Range Of Value); **RRW** (Rank Reciprocal Weighting); **RSW** (Rank Summed Weight); **SAW** (Simple Additive Weighting); **SECA** (Simultaneous Evaluation of Criteria and Alternatives); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **Fuzzy WASPAS**. 
 
 pyDecision offers an array of features, including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
 
 ## Citation
 
 PEREIRA, V.; BASILIO, M.P.; SANTOS, C.H.T (2024). Enhancing Decision Analysis with a Large Language Model: pyDecision a Comprehensive Library of MCDA Methods in Python. arXiv. https://arxiv.org/abs/2404.06370
 
@@ -55,14 +55,15 @@
 
 ```
 
 3. Try it in **Colab**:
 
 - AHP ([ Colab Demo ](https://colab.research.google.com/drive/1qwFQs5xkTZ8K-Ul_wWcCtPjLH0QooU9g?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/0377-2217(90)90057-I))
 - Fuzzy AHP ([ Colab Demo ](https://colab.research.google.com/drive/1RtEMOLGL5wtmheMRZv8emcO5wbjYVBCo?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0165-0114(83)80082-7))
+- PPF AHP ([ Colab Demo ](https://colab.research.google.com/drive/1wI-8z2aysGKhSI3PLxN6vOZ4jsbPmKYl?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2023.122354))
 - ARAS ([ Colab Demo ](https://colab.research.google.com/drive/1rwQgXjvC3E6pRhOs7CkcCV8Vw2bXEPLy?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/tede.2010.10))
 - Fuzzy ARAS ([ Colab Demo ](https://colab.research.google.com/drive/1kZDkEWsw0d0nFhDQQk8azZXRod7RnfZr?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/transport.2010.52))
 - Borda ([ Colab Demo ](https://colab.research.google.com/drive/1t5RVtG7_yXK-nPxM0MVd4U01qfTQYW4k?usp=sharing)) ( [ Paper ](http://gerardgreco.free.fr/IMG/pdf/MA_c_moire-Borda-1781.pdf))
 - BWM ([ Colab Demo ](https://colab.research.google.com/drive/1XkacTmtSBvZmx_5K9cfz8t1Ao5j-D-bZ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.omega.2014.11.009))
 - Simplified BWM ([ Colab Demo ](https://colab.research.google.com/drive/1v3QfSdprM8gwxL4VWmh75mPiPn2YWOZn?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/su13084487))
 - Fuzzy BWM ([ Colab Demo ](https://colab.research.google.com/drive/1hBTXyOLpBoC7oE-hsolPH2O0ekzp4VU0?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.knosys.2017.01.010))
 - CILOS ([ Colab Demo ](https://colab.research.google.com/drive/1RnSqO_VEPyvXAMHdneloYvA0TzPx55kw?usp=sharing)) ( [ Paper ](https://doi.org/10.1142/S0219622016500036))
@@ -100,14 +101,15 @@
 - Fuzzy MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1yJ1eOXoGNp3amhoyBtEFCXr5PqwI9S5T?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/math11061544))
 - MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1FpKl0QAdwGgCVvLYsRHvMWhz7yOp17B5?usp=sharing)) ( [ Paper ](http://matwbn.icm.edu.pl/ksiazki/cc/cc35/cc35213.pdf))
 - Fuzzy MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1ydHzGeA8WBVY5Gyu8K7Oq6kofQ5XbK3P?usp=sharing)) ( [ Paper ](https://pdfs.semanticscholar.org/6d33/ca3f14c9ed44d23742fd4e9cf94cebcaf148.pdf))
 - MOOSRA ([ Colab Demo ](https://colab.research.google.com/drive/1KYyA4f3OsipPA5e63Ja4A0OGmHvNY6dj?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.15623/ijret.2014.0315105))
 - MULTIMOORA ([ Colab Demo ](https://colab.research.google.com/drive/1JAT8qqHPNoFfMV6a-CzF6BgRwtcUF3-e?usp=sharing)) ( [ Paper ](https://journals.vilniustech.lt/index.php/TEDE/article/view/5832/5078))
 - OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1yQ41lOdjhiANtD1SOXoxA7gVim7A4X4P?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.5937/sjm10-6802))
 - Fuzzy OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1SniY4RLsR6jR9SnI3AR9k0wGlBWH6Pm8?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.5755/j01.ee.30.5.20546))
+- OPA ([ Colab Demo ](https://colab.research.google.com/drive/1RjryznPElHZUTuXQ2-ZKwJqMAVfJWKDC?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.asoc.2019.105893))
 - ORESTE ([ Colab Demo ](https://colab.research.google.com/drive/1USVCt6KJHJK9NXaknY8wTA4L0d4r2kWw?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0377-2217(82)90131-X))
 - PIV ([ Colab Demo ](https://colab.research.google.com/drive/1PwJoBqYn1O2s22MqC9euP89Uyv4sedS0?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.cie.2018.03.045))
 - PROMETHEE I    ([ Colab Demo ](https://colab.research.google.com/drive/1WsagC7-Y_5X-Xl90pMz8YwUkKfxf2vol?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE II   ([ Colab Demo ](https://colab.research.google.com/drive/143TUtTBy9y6gW0kMVAfhANBhuw1bKvBB?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE III  ([ Colab Demo ](https://colab.research.google.com/drive/11DBaEBBT8B-B3poXubvZ41HELOHok0Rz?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-030-15009-9_5
 ))
 - PROMETHEE IV   ([ Colab Demo ](https://colab.research.google.com/drive/1X2evE6pIf4F7qiKjt1fSU2PqT-NaA5sJ?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-319-11949-6_14))
@@ -129,17 +131,17 @@
 - SPOTIS ([ Colab Demo ](https://colab.research.google.com/drive/1TyjDn-xwut3w6Rf0zMiugdwytwmGY_NE?usp=sharing)) ( [ Paper ](https://doi.org/10.23919/FUSION45008.2020.9190347))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2007.10.046))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0377-2217(03)00020-1))
 - Fuzzy VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1anfCnU2TSrW-Z5vMkS_qXFrYZ0ciQE53?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2011.04.097))
 - WINGS ([ Colab Demo ](https://colab.research.google.com/drive/1li1_cPxwEM3NOZ4hbI8RROXyOmXeoWew?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2013.02.007))
+- WISP, Simple WISP ([ Colab Demo ](https://colab.research.google.com/drive/1xyJf3aydLdVPqhWpNyVXXD8T4PsrX0du?usp=sharing)) ( [ Paper ](https://doi.org/10.1109/TEM.2021.3075783))
 - WSM, WPM, WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1HbLwXI4HkrmI-lsNzDtBOlCiwxfJltHi?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.acme.2013.07.006))
 - Fuzzy WSM, Fuzzy WPM, Fuzzy WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1PcN_PaXwPHawzCU05UiHE504SkgF6vQ2?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.15837/ijccc.2015.6.2078))
-- WISP, Simple WISP ([ Colab Demo ](https://colab.research.google.com/drive/1xyJf3aydLdVPqhWpNyVXXD8T4PsrX0du?usp=sharing)) ( [ Paper ](https://doi.org/10.1109/TEM.2021.3075783))
 
 4. Compare Methods:
 - Compare Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1RfLNEJjaHjtn3Lb2cfEDqS-iblaC4GQZ?usp=sharing))
 - Compare Fuzzy Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1pRO-E9xnk6DYEj_0DaEHUrUiCeIjmnXx?usp=sharing))
 - Compare Weights & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/169hTJxP2APHrDA1h0fD1YEeu9s29wu0T?usp=sharing))
 - Compare Fuzzy Weights & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1nWDF8lrTmXlc-TE4_X1-MPhraFjytj1Z?usp=sharing))
 
@@ -148,10 +150,10 @@
 - [3MOAHP](https://github.com/Valdecy/Method_3MOAHP) - Inconsistency Reduction Technique for AHP and Fuzzy-AHP Methods
 - [pyMissingAHP](https://github.com/Valdecy/pyMissingAHP) - A Method to Infer AHP Missing Pairwise Comparisons
 - [ELECTRE-Tree](https://github.com/Valdecy/ELECTRE-Tree) - Algorithm to infer the ELECTRE Tri-B method parameters
 - [Ranking-Trees](https://github.com/Valdecy/Ranking-Trees) - Algorithm to infer the ELECTRE II, III, IV, and PROMETHEE I, II, III, IV method parameters
 
 # Acknowledgement 
 
-This section is dedicated to all the people who helped to improve or correct the code. Thank you very much!
+This section is dedicated to everyone who helped improve or correct the code. Thank you very much!
 
 * Sabir Mohammedi Taieb (23.JANUARY.2023) - https://sabir97.github.io/ - Université Abdelhamid Ibn Badis Mostaganem (Algeria)
```

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/__init__.py` & `pyDecision-4.5.5/pyDecision/algorithm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from .e_iii         import electre_iii
 from .e_iv          import electre_iv
 from .e_tri_b       import electre_tri_b
 from .edas          import edas_method
 from .entropy       import entropy_method
 from .fucom         import fucom_method
 from .fuzzy_ahp     import fuzzy_ahp_method
+from .fuzzy_ahp_ppf import ppf_ahp_method
 from .fuzzy_aras    import fuzzy_aras_method
 from .fuzzy_bwm     import fuzzy_bw_method
 from .fuzzy_copras  import fuzzy_copras_method
 from .fuzzy_critic  import fuzzy_critic_method
 from .fuzzy_dematel import fuzzy_dematel_method
 from .fuzzy_edas    import fuzzy_edas_method
 from .fuzzy_fucom   import fuzzy_fucom_method
@@ -44,14 +45,15 @@
 from .marcos        import marcos_method
 from .maut          import maut_method
 from .merec         import merec_method
 from .moora         import moora_method
 from .moosra        import moosra_method
 from .multimoora    import multimoora_method  
 from .ocra          import ocra_method
+from .opa           import opa_method
 from .oreste        import oreste_method
 from .p_ec          import ec_promethee, solution_p_ranking, plot_rank_freq, find_column_modes
 from .p_i           import promethee_i
 from .p_ii          import promethee_ii
 from .p_iii         import promethee_iii
 from .p_iv          import promethee_iv
 from .p_v           import promethee_v
```

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/ahp.py` & `pyDecision-4.5.5/pyDecision/algorithm/ahp.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Required Libraries
 import numpy as np
 from functools import reduce
 
 ###############################################################################
 
-# Function: AHP
+# Function: AHP (Analytic Hierarchy Process)
 def ahp_method(dataset, wd = 'm'):
     inc_rat  = np.array([0, 0, 0, 0.58, 0.9, 1.12, 1.24, 1.32, 1.41, 1.45, 1.49, 1.51, 1.48, 1.56, 1.57, 1.59])
     X        = np.copy(dataset)
     weights  = np.zeros(X.shape[1])
     if (wd == 'm' or wd == 'mean'):
         weights  = np.mean(X/np.sum(X, axis = 0), axis = 1)
         vector   = np.sum(X*weights, axis = 1)/weights
```

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/aras.py` & `pyDecision-4.5.5/pyDecision/algorithm/aras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/borda.py` & `pyDecision-4.5.5/pyDecision/algorithm/borda.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/bwm.py` & `pyDecision-4.5.5/pyDecision/algorithm/bwm.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/bwm_s.py` & `pyDecision-4.5.5/pyDecision/algorithm/bwm_s.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/cilos.py` & `pyDecision-4.5.5/pyDecision/algorithm/cilos.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/cocoso.py` & `pyDecision-4.5.5/pyDecision/algorithm/cocoso.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/codas.py` & `pyDecision-4.5.5/pyDecision/algorithm/codas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/copeland.py` & `pyDecision-4.5.5/pyDecision/algorithm/copeland.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/copras.py` & `pyDecision-4.5.5/pyDecision/algorithm/copras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/cradis.py` & `pyDecision-4.5.5/pyDecision/algorithm/cradis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/critic.py` & `pyDecision-4.5.5/pyDecision/algorithm/critic.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/dematel.py` & `pyDecision-4.5.5/pyDecision/algorithm/dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/e_i.py` & `pyDecision-4.5.5/pyDecision/algorithm/e_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/e_i_s.py` & `pyDecision-4.5.5/pyDecision/algorithm/e_i_s.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/e_i_v.py` & `pyDecision-4.5.5/pyDecision/algorithm/e_i_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/e_ii.py` & `pyDecision-4.5.5/pyDecision/algorithm/e_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/e_iii.py` & `pyDecision-4.5.5/pyDecision/algorithm/e_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/e_iv.py` & `pyDecision-4.5.5/pyDecision/algorithm/e_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/e_tri_b.py` & `pyDecision-4.5.5/pyDecision/algorithm/e_tri_b.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/edas.py` & `pyDecision-4.5.5/pyDecision/algorithm/edas.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         axes.set_ylim([ymin, ymax])
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
-# Function: EDAS
+# Function: EDAS (Evaluation based on Distance from Average Solution)
 def edas_method(dataset, criterion_type, weights, graph = True, verbose = True):
     col_mean = np.mean(dataset, axis = 0)
     pda      = np.zeros((dataset.shape[0], dataset.shape[1]))
     nda      = np.zeros((dataset.shape[0], dataset.shape[1]))
     for i in range(0, dataset.shape[0]):
         for j in range(0, dataset.shape[1]):
             if (criterion_type[j] == 'max'):
```

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/entropy.py` & `pyDecision-4.5.5/pyDecision/algorithm/entropy.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/fucom.py` & `pyDecision-4.5.5/pyDecision/algorithm/fucom.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/fuzzy_ahp.py` & `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/fuzzy_aras.py` & `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_aras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/fuzzy_bwm.py` & `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_bwm.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/fuzzy_copras.py` & `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_copras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/fuzzy_critic.py` & `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_critic.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/fuzzy_dematel.py` & `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/fuzzy_edas.py` & `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/fuzzy_fucom.py` & `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_fucom.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/fuzzy_merec.py` & `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_merec.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/fuzzy_moora.py` & `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_moora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/fuzzy_ocra.py` & `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_ocra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/fuzzy_topsis.py` & `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/fuzzy_vikor.py` & `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/fuzzy_waspas.py` & `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_waspas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/gra.py` & `pyDecision-4.5.5/pyDecision/algorithm/gra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/idocriw.py` & `pyDecision-4.5.5/pyDecision/algorithm/idocriw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/mabac.py` & `pyDecision-4.5.5/pyDecision/algorithm/mabac.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/macbeth.py` & `pyDecision-4.5.5/pyDecision/algorithm/macbeth.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/mairca.py` & `pyDecision-4.5.5/pyDecision/algorithm/mairca.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/mara.py` & `pyDecision-4.5.5/pyDecision/algorithm/mara.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/marcos.py` & `pyDecision-4.5.5/pyDecision/algorithm/marcos.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/maut.py` & `pyDecision-4.5.5/pyDecision/algorithm/maut.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/merec.py` & `pyDecision-4.5.5/pyDecision/algorithm/merec.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/moora.py` & `pyDecision-4.5.5/pyDecision/algorithm/moora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/moosra.py` & `pyDecision-4.5.5/pyDecision/algorithm/moosra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/multimoora.py` & `pyDecision-4.5.5/pyDecision/algorithm/multimoora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/ocra.py` & `pyDecision-4.5.5/pyDecision/algorithm/ocra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/oreste.py` & `pyDecision-4.5.5/pyDecision/algorithm/oreste.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/p_ec.py` & `pyDecision-4.5.5/pyDecision/algorithm/p_ec.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/p_i.py` & `pyDecision-4.5.5/pyDecision/algorithm/p_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/p_ii.py` & `pyDecision-4.5.5/pyDecision/algorithm/p_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/p_iii.py` & `pyDecision-4.5.5/pyDecision/algorithm/p_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/p_iv.py` & `pyDecision-4.5.5/pyDecision/algorithm/p_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/p_v.py` & `pyDecision-4.5.5/pyDecision/algorithm/p_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/p_vi.py` & `pyDecision-4.5.5/pyDecision/algorithm/p_vi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/p_xgaia.py` & `pyDecision-4.5.5/pyDecision/algorithm/p_xgaia.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/piv.py` & `pyDecision-4.5.5/pyDecision/algorithm/piv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/psi.py` & `pyDecision-4.5.5/pyDecision/algorithm/psi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/psi_m.py` & `pyDecision-4.5.5/pyDecision/algorithm/psi_m.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/rafsi.py` & `pyDecision-4.5.5/pyDecision/algorithm/rafsi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/regime.py` & `pyDecision-4.5.5/pyDecision/algorithm/regime.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/roc.py` & `pyDecision-4.5.5/pyDecision/algorithm/roc.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/rov.py` & `pyDecision-4.5.5/pyDecision/algorithm/rov.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/rrw.py` & `pyDecision-4.5.5/pyDecision/algorithm/rrw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/rsw.py` & `pyDecision-4.5.5/pyDecision/algorithm/rsw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/saw.py` & `pyDecision-4.5.5/pyDecision/algorithm/saw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/seca.py` & `pyDecision-4.5.5/pyDecision/algorithm/seca.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/smart.py` & `pyDecision-4.5.5/pyDecision/algorithm/smart.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/spotis.py` & `pyDecision-4.5.5/pyDecision/algorithm/spotis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/todim.py` & `pyDecision-4.5.5/pyDecision/algorithm/todim.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/topsis.py` & `pyDecision-4.5.5/pyDecision/algorithm/topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/vikor.py` & `pyDecision-4.5.5/pyDecision/algorithm/vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/waspas.py` & `pyDecision-4.5.5/pyDecision/algorithm/waspas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/wings.py` & `pyDecision-4.5.5/pyDecision/algorithm/wings.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 import numpy as np
 import matplotlib.pyplot as plt
 
 ###############################################################################
 
 # Function: WINGS (Weighted Influence Non-linear Gauge System)
 def wings_method(dataset, size_x = 10, size_y = 10): 
-    D = dataset
-    C = D/np.sum(D)
-    I = np.eye(dataset.shape[0])
-    T = np.dot(C, np.linalg.inv( I - C ))
-    c_i = np.sum(T, axis = 0)
-    r_i = np.sum(T, axis = 1)
+    D         = dataset
+    C         = D/np.sum(D)
+    I         = np.eye(dataset.shape[0])
+    T         = np.dot(C, np.linalg.inv( I - C ))
+    c_i       = np.sum(T, axis = 0)
+    r_i       = np.sum(T, axis = 1)
     r_plus_c  = r_i + c_i 
     r_minus_c = r_i - c_i 
     weights   = r_plus_c/np.sum(r_plus_c)
     plt.figure(figsize = [size_x, size_y])
     plt.style.use('ggplot')
     for i in range(0, dataset.shape[0]):
         if (r_minus_c[i] >= 0 and  r_plus_c[i] >= np.mean(r_plus_c)):
```

### Comparing `pyDecision-4.5.4/pyDecision/algorithm/wisp.py` & `pyDecision-4.5.5/pyDecision/algorithm/wisp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/compare/compare.py` & `pyDecision-4.5.5/pyDecision/compare/compare.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/util/LLM.py` & `pyDecision-4.5.5/pyDecision/util/LLM.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision/util/ga.py` & `pyDecision-4.5.5/pyDecision/util/ga.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.4/pyDecision.egg-info/PKG-INFO` & `pyDecision-4.5.5/pyDecision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 4.5.4
+Version: 4.5.5
 Summary: A MCDA Library Incorporating a Large Language Model to Enhance Decision Analysis
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **Fuzzy CRITIC**; **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **Fuzzy FUCOM**; **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **RAFSI** (Ranking of Alternatives through Functional mapping of criterion sub-intervals into a Single Interval); **REGIME** (REGIonal Multicriteria Elimination); **ROC** (Rank Ordered Centroid); **ROV** (Range Of Value); **RRW** (Rank Reciprocal Weighting); **RSW** (Rank Summed Weight); **SAW** (Simple Additive Weighting); **SECA** (Simultaneous Evaluation of Criteria and Alternatives); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **Fuzzy WASPAS**; **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**. 
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **PPF AHP** (Proportional Picture Fuzzy AHP); **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **Fuzzy CRITIC**; **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **Fuzzy FUCOM**; **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **OPA** (Ordinal Priority Approach); **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **RAFSI** (Ranking of Alternatives through Functional mapping of criterion sub-intervals into a Single Interval); **REGIME** (REGIonal Multicriteria Elimination); **ROC** (Rank Ordered Centroid); **ROV** (Range Of Value); **RRW** (Rank Reciprocal Weighting); **RSW** (Rank Summed Weight); **SAW** (Simple Additive Weighting); **SECA** (Simultaneous Evaluation of Criteria and Alternatives); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **Fuzzy WASPAS**. 
 
 pyDecision offers an array of features, including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
 
 ## Citation
 
 PEREIRA, V.; BASILIO, M.P.; SANTOS, C.H.T (2024). Enhancing Decision Analysis with a Large Language Model: pyDecision a Comprehensive Library of MCDA Methods in Python. arXiv. https://arxiv.org/abs/2404.06370
 
@@ -66,14 +66,15 @@
 
 ```
 
 3. Try it in **Colab**:
 
 - AHP ([ Colab Demo ](https://colab.research.google.com/drive/1qwFQs5xkTZ8K-Ul_wWcCtPjLH0QooU9g?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/0377-2217(90)90057-I))
 - Fuzzy AHP ([ Colab Demo ](https://colab.research.google.com/drive/1RtEMOLGL5wtmheMRZv8emcO5wbjYVBCo?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0165-0114(83)80082-7))
+- PPF AHP ([ Colab Demo ](https://colab.research.google.com/drive/1wI-8z2aysGKhSI3PLxN6vOZ4jsbPmKYl?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2023.122354))
 - ARAS ([ Colab Demo ](https://colab.research.google.com/drive/1rwQgXjvC3E6pRhOs7CkcCV8Vw2bXEPLy?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/tede.2010.10))
 - Fuzzy ARAS ([ Colab Demo ](https://colab.research.google.com/drive/1kZDkEWsw0d0nFhDQQk8azZXRod7RnfZr?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/transport.2010.52))
 - Borda ([ Colab Demo ](https://colab.research.google.com/drive/1t5RVtG7_yXK-nPxM0MVd4U01qfTQYW4k?usp=sharing)) ( [ Paper ](http://gerardgreco.free.fr/IMG/pdf/MA_c_moire-Borda-1781.pdf))
 - BWM ([ Colab Demo ](https://colab.research.google.com/drive/1XkacTmtSBvZmx_5K9cfz8t1Ao5j-D-bZ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.omega.2014.11.009))
 - Simplified BWM ([ Colab Demo ](https://colab.research.google.com/drive/1v3QfSdprM8gwxL4VWmh75mPiPn2YWOZn?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/su13084487))
 - Fuzzy BWM ([ Colab Demo ](https://colab.research.google.com/drive/1hBTXyOLpBoC7oE-hsolPH2O0ekzp4VU0?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.knosys.2017.01.010))
 - CILOS ([ Colab Demo ](https://colab.research.google.com/drive/1RnSqO_VEPyvXAMHdneloYvA0TzPx55kw?usp=sharing)) ( [ Paper ](https://doi.org/10.1142/S0219622016500036))
@@ -111,14 +112,15 @@
 - Fuzzy MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1yJ1eOXoGNp3amhoyBtEFCXr5PqwI9S5T?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/math11061544))
 - MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1FpKl0QAdwGgCVvLYsRHvMWhz7yOp17B5?usp=sharing)) ( [ Paper ](http://matwbn.icm.edu.pl/ksiazki/cc/cc35/cc35213.pdf))
 - Fuzzy MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1ydHzGeA8WBVY5Gyu8K7Oq6kofQ5XbK3P?usp=sharing)) ( [ Paper ](https://pdfs.semanticscholar.org/6d33/ca3f14c9ed44d23742fd4e9cf94cebcaf148.pdf))
 - MOOSRA ([ Colab Demo ](https://colab.research.google.com/drive/1KYyA4f3OsipPA5e63Ja4A0OGmHvNY6dj?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.15623/ijret.2014.0315105))
 - MULTIMOORA ([ Colab Demo ](https://colab.research.google.com/drive/1JAT8qqHPNoFfMV6a-CzF6BgRwtcUF3-e?usp=sharing)) ( [ Paper ](https://journals.vilniustech.lt/index.php/TEDE/article/view/5832/5078))
 - OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1yQ41lOdjhiANtD1SOXoxA7gVim7A4X4P?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.5937/sjm10-6802))
 - Fuzzy OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1SniY4RLsR6jR9SnI3AR9k0wGlBWH6Pm8?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.5755/j01.ee.30.5.20546))
+- OPA ([ Colab Demo ](https://colab.research.google.com/drive/1RjryznPElHZUTuXQ2-ZKwJqMAVfJWKDC?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.asoc.2019.105893))
 - ORESTE ([ Colab Demo ](https://colab.research.google.com/drive/1USVCt6KJHJK9NXaknY8wTA4L0d4r2kWw?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0377-2217(82)90131-X))
 - PIV ([ Colab Demo ](https://colab.research.google.com/drive/1PwJoBqYn1O2s22MqC9euP89Uyv4sedS0?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.cie.2018.03.045))
 - PROMETHEE I    ([ Colab Demo ](https://colab.research.google.com/drive/1WsagC7-Y_5X-Xl90pMz8YwUkKfxf2vol?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE II   ([ Colab Demo ](https://colab.research.google.com/drive/143TUtTBy9y6gW0kMVAfhANBhuw1bKvBB?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE III  ([ Colab Demo ](https://colab.research.google.com/drive/11DBaEBBT8B-B3poXubvZ41HELOHok0Rz?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-030-15009-9_5
 ))
 - PROMETHEE IV   ([ Colab Demo ](https://colab.research.google.com/drive/1X2evE6pIf4F7qiKjt1fSU2PqT-NaA5sJ?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-319-11949-6_14))
@@ -140,17 +142,17 @@
 - SPOTIS ([ Colab Demo ](https://colab.research.google.com/drive/1TyjDn-xwut3w6Rf0zMiugdwytwmGY_NE?usp=sharing)) ( [ Paper ](https://doi.org/10.23919/FUSION45008.2020.9190347))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2007.10.046))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0377-2217(03)00020-1))
 - Fuzzy VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1anfCnU2TSrW-Z5vMkS_qXFrYZ0ciQE53?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2011.04.097))
 - WINGS ([ Colab Demo ](https://colab.research.google.com/drive/1li1_cPxwEM3NOZ4hbI8RROXyOmXeoWew?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2013.02.007))
+- WISP, Simple WISP ([ Colab Demo ](https://colab.research.google.com/drive/1xyJf3aydLdVPqhWpNyVXXD8T4PsrX0du?usp=sharing)) ( [ Paper ](https://doi.org/10.1109/TEM.2021.3075783))
 - WSM, WPM, WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1HbLwXI4HkrmI-lsNzDtBOlCiwxfJltHi?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.acme.2013.07.006))
 - Fuzzy WSM, Fuzzy WPM, Fuzzy WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1PcN_PaXwPHawzCU05UiHE504SkgF6vQ2?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.15837/ijccc.2015.6.2078))
-- WISP, Simple WISP ([ Colab Demo ](https://colab.research.google.com/drive/1xyJf3aydLdVPqhWpNyVXXD8T4PsrX0du?usp=sharing)) ( [ Paper ](https://doi.org/10.1109/TEM.2021.3075783))
 
 4. Compare Methods:
 - Compare Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1RfLNEJjaHjtn3Lb2cfEDqS-iblaC4GQZ?usp=sharing))
 - Compare Fuzzy Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1pRO-E9xnk6DYEj_0DaEHUrUiCeIjmnXx?usp=sharing))
 - Compare Weights & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/169hTJxP2APHrDA1h0fD1YEeu9s29wu0T?usp=sharing))
 - Compare Fuzzy Weights & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1nWDF8lrTmXlc-TE4_X1-MPhraFjytj1Z?usp=sharing))
 
@@ -159,10 +161,10 @@
 - [3MOAHP](https://github.com/Valdecy/Method_3MOAHP) - Inconsistency Reduction Technique for AHP and Fuzzy-AHP Methods
 - [pyMissingAHP](https://github.com/Valdecy/pyMissingAHP) - A Method to Infer AHP Missing Pairwise Comparisons
 - [ELECTRE-Tree](https://github.com/Valdecy/ELECTRE-Tree) - Algorithm to infer the ELECTRE Tri-B method parameters
 - [Ranking-Trees](https://github.com/Valdecy/Ranking-Trees) - Algorithm to infer the ELECTRE II, III, IV, and PROMETHEE I, II, III, IV method parameters
 
 # Acknowledgement 
 
-This section is dedicated to all the people who helped to improve or correct the code. Thank you very much!
+This section is dedicated to everyone who helped improve or correct the code. Thank you very much!
 
 * Sabir Mohammedi Taieb (23.JANUARY.2023) - https://sabir97.github.io/ - UniversitÃ© Abdelhamid Ibn Badis Mostaganem (Algeria)
```

### Comparing `pyDecision-4.5.4/pyDecision.egg-info/SOURCES.txt` & `pyDecision-4.5.5/pyDecision.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 pyDecision/algorithm/e_iii.py
 pyDecision/algorithm/e_iv.py
 pyDecision/algorithm/e_tri_b.py
 pyDecision/algorithm/edas.py
 pyDecision/algorithm/entropy.py
 pyDecision/algorithm/fucom.py
 pyDecision/algorithm/fuzzy_ahp.py
+pyDecision/algorithm/fuzzy_ahp_ppf.py
 pyDecision/algorithm/fuzzy_aras.py
 pyDecision/algorithm/fuzzy_bwm.py
 pyDecision/algorithm/fuzzy_copras.py
 pyDecision/algorithm/fuzzy_critic.py
 pyDecision/algorithm/fuzzy_dematel.py
 pyDecision/algorithm/fuzzy_edas.py
 pyDecision/algorithm/fuzzy_fucom.py
@@ -54,14 +55,15 @@
 pyDecision/algorithm/marcos.py
 pyDecision/algorithm/maut.py
 pyDecision/algorithm/merec.py
 pyDecision/algorithm/moora.py
 pyDecision/algorithm/moosra.py
 pyDecision/algorithm/multimoora.py
 pyDecision/algorithm/ocra.py
+pyDecision/algorithm/opa.py
 pyDecision/algorithm/oreste.py
 pyDecision/algorithm/p_ec.py
 pyDecision/algorithm/p_i.py
 pyDecision/algorithm/p_ii.py
 pyDecision/algorithm/p_iii.py
 pyDecision/algorithm/p_iv.py
 pyDecision/algorithm/p_v.py
```

### Comparing `pyDecision-4.5.4/setup.py` & `pyDecision-4.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyDecision',
-    version='4.5.4',
+    version='4.5.5',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyDecisions',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
```


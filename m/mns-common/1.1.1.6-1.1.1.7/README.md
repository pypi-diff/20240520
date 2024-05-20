# Comparing `tmp/mns_common-1.1.1.6.tar.gz` & `tmp/mns_common-1.1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns_common-1.1.1.6.tar", last modified: Mon May 20 06:36:23 2024, max compression
+gzip compressed data, was "mns_common-1.1.1.7.tar", last modified: Mon May 20 14:22:03 2024, max compression
```

## Comparing `mns_common-1.1.1.6.tar` & `mns_common-1.1.1.7.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.807006 mns_common-1.1.1.6/
--rw-rw-rw-   0        0        0       59 2024-05-20 06:36:23.806009 mns_common-1.1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.768554 mns_common-1.1.1.6/mns_common/
--rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.1.1.6/mns_common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.770548 mns_common-1.1.1.6/mns_common/api/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.1.1.6/mns_common/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.773540 mns_common-1.1.1.6/mns_common/api/akshare/
--rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.1.1.6/mns_common/api/akshare/__init__.py
--rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.1.1.6/mns_common/api/akshare/k_line_api.py
--rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.1.1.6/mns_common/api/akshare/stock_bid_ask_api.py
--rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.1.1.6/mns_common/api/akshare/stock_dt_pool.py
--rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.1.1.6/mns_common/api/akshare/stock_zb_pool.py
--rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.1.1.6/mns_common/api/akshare/stock_zt_pool_api.py
--rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.1.1.6/mns_common/api/akshare/yjyg_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.776094 mns_common-1.1.1.6/mns_common/api/em/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.1.1.6/mns_common/api/em/__init__.py
--rw-rw-rw-   0        0        0     8352 2024-05-10 13:01:52.000000 mns_common-1.1.1.6/mns_common/api/em/east_money_stock_api.py
--rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.1.1.6/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
--rw-rw-rw-   0        0        0     4371 2024-05-17 04:06:34.000000 mns_common-1.1.1.6/mns_common/api/em/east_money_stock_hk_api.py
--rw-rw-rw-   0        0        0    14960 2024-05-10 12:40:48.000000 mns_common-1.1.1.6/mns_common/api/em/east_money_stock_v2_api.py
--rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.1.1.6/mns_common/api/em/em_concept_index_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.776094 mns_common-1.1.1.6/mns_common/api/kpl/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.1.6/mns_common/api/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.777087 mns_common-1.1.1.6/mns_common/api/kpl/common/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.1.6/mns_common/api/kpl/common/__init__.py
--rw-rw-rw-   0        0        0     6536 2024-04-24 09:08:22.000000 mns_common-1.1.1.6/mns_common/api/kpl/common/kpl_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.778084 mns_common-1.1.1.6/mns_common/api/kpl/concept/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.1.6/mns_common/api/kpl/concept/__init__.py
--rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.1.1.6/mns_common/api/kpl/concept/kpl_concept_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.779081 mns_common-1.1.1.6/mns_common/api/kpl/constant/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.1.6/mns_common/api/kpl/constant/__init__.py
--rw-rw-rw-   0        0        0      669 2023-12-22 09:50:37.000000 mns_common-1.1.1.6/mns_common/api/kpl/constant/kpl_constant.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.780079 mns_common-1.1.1.6/mns_common/api/kpl/industry/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.1.6/mns_common/api/kpl/industry/__init__.py
--rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.1.1.6/mns_common/api/kpl/industry/kpl_industry_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.781075 mns_common-1.1.1.6/mns_common/api/kpl/selection/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.1.6/mns_common/api/kpl/selection/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-05-06 13:55:26.000000 mns_common-1.1.1.6/mns_common/api/kpl/selection/kpl_selection_plate_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.782073 mns_common-1.1.1.6/mns_common/api/kpl/symbol/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.1.6/mns_common/api/kpl/symbol/__init__.py
--rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.1.1.6/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
--rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.1.1.6/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
--rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.1.1.6/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.783071 mns_common-1.1.1.6/mns_common/api/msg/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.1.6/mns_common/api/msg/__init__.py
--rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.1.1.6/mns_common/api/msg/push_msg_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.785065 mns_common-1.1.1.6/mns_common/api/ths/
--rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.1.1.6/mns_common/api/ths/__init__.py
--rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.1.1.6/mns_common/api/ths/ths_big_deal_api.py
--rw-rw-rw-   0        0        0    40309 2024-05-14 08:22:47.000000 mns_common-1.1.1.6/mns_common/api/ths/ths_stock_api.py
--rw-rw-rw-   0        0        0     6648 2024-05-20 06:35:22.000000 mns_common-1.1.1.6/mns_common/api/ths/ths_stock_zt_pool_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.786062 mns_common-1.1.1.6/mns_common/component/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.1.1.6/mns_common/component/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.787059 mns_common-1.1.1.6/mns_common/component/cache/
--rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.1.1.6/mns_common/component/cache/__init__.py
--rw-rw-rw-   0        0        0      809 2024-04-28 07:38:03.000000 mns_common-1.1.1.6/mns_common/component/cache/cache_service.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.788057 mns_common-1.1.1.6/mns_common/component/classify/
--rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.1.1.6/mns_common/component/classify/__init__.py
--rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.1.1.6/mns_common/component/classify/classify_constant.py
--rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.1.1.6/mns_common/component/classify/symbol_classify_api.py
--rw-rw-rw-   0        0        0     5068 2024-05-15 08:05:35.000000 mns_common-1.1.1.6/mns_common/component/common_service_fun_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.789054 mns_common-1.1.1.6/mns_common/component/company/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.1.6/mns_common/component/company/__init__.py
--rw-rw-rw-   0        0        0     7217 2024-05-17 13:48:14.000000 mns_common-1.1.1.6/mns_common/component/company/company_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.790052 mns_common-1.1.1.6/mns_common/component/concept/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.1.6/mns_common/component/concept/__init__.py
--rw-rw-rw-   0        0        0     3235 2024-05-09 14:23:16.000000 mns_common-1.1.1.6/mns_common/component/concept/kpl_concept_common_service_api.py
--rw-rw-rw-   0        0        0     9637 2024-04-30 09:46:26.000000 mns_common-1.1.1.6/mns_common/component/concept/ths_concept_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.791049 mns_common-1.1.1.6/mns_common/component/data/
--rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.1.1.6/mns_common/component/data/__init__.py
--rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.1.1.6/mns_common/component/data/data_init_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.792046 mns_common-1.1.1.6/mns_common/component/industry/
--rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.1.1.6/mns_common/component/industry/__init__.py
--rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.1.1.6/mns_common/component/industry/ths_industry_index_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.792046 mns_common-1.1.1.6/mns_common/component/k_line/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.1.6/mns_common/component/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.794041 mns_common-1.1.1.6/mns_common/component/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.1.1.6/mns_common/component/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.1.1.6/mns_common/component/k_line/clean/k_line_param.py
--rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.1.1.6/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.794041 mns_common-1.1.1.6/mns_common/component/k_line/common/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.1.1.6/mns_common/component/k_line/common/__init__.py
--rw-rw-rw-   0        0        0     4449 2023-12-29 04:25:17.000000 mns_common-1.1.1.6/mns_common/component/k_line/common/k_line_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.796036 mns_common-1.1.1.6/mns_common/component/k_line/patterns/
--rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.1.1.6/mns_common/component/k_line/patterns/__init__.py
--rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.1.1.6/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
--rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.1.1.6/mns_common/component/k_line/patterns/pattern_Enum.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.797033 mns_common-1.1.1.6/mns_common/component/real_time/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.1.6/mns_common/component/real_time/__init__.py
--rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.1.1.6/mns_common/component/real_time/real_time_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.798031 mns_common-1.1.1.6/mns_common/component/self_choose/
--rw-rw-rw-   0        0        0      163 2024-05-14 15:36:27.000000 mns_common-1.1.1.6/mns_common/component/self_choose/__init__.py
--rw-rw-rw-   0        0        0     2232 2024-05-16 05:56:38.000000 mns_common-1.1.1.6/mns_common/component/self_choose/black_list_service_api.py
--rw-rw-rw-   0        0        0      519 2024-05-18 07:01:06.000000 mns_common-1.1.1.6/mns_common/component/self_choose/self_choose_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.799028 mns_common-1.1.1.6/mns_common/component/trade/
--rw-rw-rw-   0        0        0      163 2024-04-27 12:44:35.000000 mns_common-1.1.1.6/mns_common/component/trade/__init__.py
--rw-rw-rw-   0        0        0     3120 2024-05-08 07:34:38.000000 mns_common-1.1.1.6/mns_common/component/trade/trade_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.800025 mns_common-1.1.1.6/mns_common/component/trade_date/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.1.6/mns_common/component/trade_date/__init__.py
--rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.1.1.6/mns_common/component/trade_date/trade_date_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.800025 mns_common-1.1.1.6/mns_common/component/zt/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.1.6/mns_common/component/zt/__init__.py
--rw-rw-rw-   0        0        0     8650 2024-05-12 14:00:57.000000 mns_common-1.1.1.6/mns_common/component/zt/zt_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.802020 mns_common-1.1.1.6/mns_common/constant/
--rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.1.1.6/mns_common/constant/__init__.py
--rw-rw-rw-   0        0        0     1944 2024-05-19 14:56:15.000000 mns_common-1.1.1.6/mns_common/constant/db_name_constant.py
--rw-rw-rw-   0        0        0     4507 2024-01-25 14:21:07.000000 mns_common-1.1.1.6/mns_common/constant/kpl_selection_no_choose_constant.py
--rw-rw-rw-   0        0        0      347 2024-05-01 15:03:02.000000 mns_common-1.1.1.6/mns_common/constant/self_choose_constant.py
--rw-rw-rw-   0        0        0    12240 2024-03-11 15:08:57.000000 mns_common-1.1.1.6/mns_common/constant/ths_concept_no_choose_constant.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.803017 mns_common-1.1.1.6/mns_common/db/
--rw-rw-rw-   0        0        0    10816 2024-04-24 14:49:25.000000 mns_common-1.1.1.6/mns_common/db/MongodbUtil.py
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.1.1.6/mns_common/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.805012 mns_common-1.1.1.6/mns_common/utils/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.1.1.6/mns_common/utils/__init__.py
--rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.1.1.6/mns_common/utils/async_fun.py
--rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.1.1.6/mns_common/utils/data_frame_util.py
--rw-rw-rw-   0        0        0     7379 2023-12-21 03:38:02.000000 mns_common-1.1.1.6/mns_common/utils/date_handle_util.py
--rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.1.1.6/mns_common/utils/ip_util.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:36:23.806009 mns_common-1.1.1.6/mns_common.egg-info/
--rw-rw-rw-   0        0        0       59 2024-05-20 06:36:23.000000 mns_common-1.1.1.6/mns_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3872 2024-05-20 06:36:23.000000 mns_common-1.1.1.6/mns_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 06:36:23.000000 mns_common-1.1.1.6/mns_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-20 06:36:23.000000 mns_common-1.1.1.6/mns_common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 06:36:23.807006 mns_common-1.1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      466 2024-05-20 06:35:58.000000 mns_common-1.1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.245916 mns_common-1.1.1.7/
+-rw-rw-rw-   0        0        0       59 2024-05-20 14:22:03.245916 mns_common-1.1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.203457 mns_common-1.1.1.7/mns_common/
+-rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.1.1.7/mns_common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.205453 mns_common-1.1.1.7/mns_common/api/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.1.1.7/mns_common/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.209442 mns_common-1.1.1.7/mns_common/api/akshare/
+-rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.1.1.7/mns_common/api/akshare/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.1.1.7/mns_common/api/akshare/k_line_api.py
+-rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.1.1.7/mns_common/api/akshare/stock_bid_ask_api.py
+-rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.1.1.7/mns_common/api/akshare/stock_dt_pool.py
+-rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.1.1.7/mns_common/api/akshare/stock_zb_pool.py
+-rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.1.1.7/mns_common/api/akshare/stock_zt_pool_api.py
+-rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.1.1.7/mns_common/api/akshare/yjyg_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.212435 mns_common-1.1.1.7/mns_common/api/em/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.1.1.7/mns_common/api/em/__init__.py
+-rw-rw-rw-   0        0        0     8352 2024-05-10 13:01:52.000000 mns_common-1.1.1.7/mns_common/api/em/east_money_stock_api.py
+-rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.1.1.7/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
+-rw-rw-rw-   0        0        0     4371 2024-05-17 04:06:34.000000 mns_common-1.1.1.7/mns_common/api/em/east_money_stock_hk_api.py
+-rw-rw-rw-   0        0        0    14960 2024-05-10 12:40:48.000000 mns_common-1.1.1.7/mns_common/api/em/east_money_stock_v2_api.py
+-rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.1.1.7/mns_common/api/em/em_concept_index_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.212435 mns_common-1.1.1.7/mns_common/api/kpl/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.1.7/mns_common/api/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.213432 mns_common-1.1.1.7/mns_common/api/kpl/common/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.1.7/mns_common/api/kpl/common/__init__.py
+-rw-rw-rw-   0        0        0     6536 2024-04-24 09:08:22.000000 mns_common-1.1.1.7/mns_common/api/kpl/common/kpl_common_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.214429 mns_common-1.1.1.7/mns_common/api/kpl/concept/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.1.7/mns_common/api/kpl/concept/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.1.1.7/mns_common/api/kpl/concept/kpl_concept_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.215426 mns_common-1.1.1.7/mns_common/api/kpl/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.1.7/mns_common/api/kpl/constant/__init__.py
+-rw-rw-rw-   0        0        0      669 2023-12-22 09:50:37.000000 mns_common-1.1.1.7/mns_common/api/kpl/constant/kpl_constant.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.216423 mns_common-1.1.1.7/mns_common/api/kpl/industry/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.1.7/mns_common/api/kpl/industry/__init__.py
+-rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.1.1.7/mns_common/api/kpl/industry/kpl_industry_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.217420 mns_common-1.1.1.7/mns_common/api/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.1.7/mns_common/api/kpl/selection/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-05-06 13:55:26.000000 mns_common-1.1.1.7/mns_common/api/kpl/selection/kpl_selection_plate_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.218966 mns_common-1.1.1.7/mns_common/api/kpl/symbol/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.1.7/mns_common/api/kpl/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.1.1.7/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
+-rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.1.1.7/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
+-rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.1.1.7/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.219959 mns_common-1.1.1.7/mns_common/api/msg/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.1.7/mns_common/api/msg/__init__.py
+-rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.1.1.7/mns_common/api/msg/push_msg_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.221950 mns_common-1.1.1.7/mns_common/api/ths/
+-rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.1.1.7/mns_common/api/ths/__init__.py
+-rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.1.1.7/mns_common/api/ths/ths_big_deal_api.py
+-rw-rw-rw-   0        0        0    40309 2024-05-14 08:22:47.000000 mns_common-1.1.1.7/mns_common/api/ths/ths_stock_api.py
+-rw-rw-rw-   0        0        0     6648 2024-05-20 06:35:22.000000 mns_common-1.1.1.7/mns_common/api/ths/ths_stock_zt_pool_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.222947 mns_common-1.1.1.7/mns_common/component/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.1.1.7/mns_common/component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.223943 mns_common-1.1.1.7/mns_common/component/cache/
+-rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.1.1.7/mns_common/component/cache/__init__.py
+-rw-rw-rw-   0        0        0      809 2024-04-28 07:38:03.000000 mns_common-1.1.1.7/mns_common/component/cache/cache_service.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.224941 mns_common-1.1.1.7/mns_common/component/classify/
+-rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.1.1.7/mns_common/component/classify/__init__.py
+-rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.1.1.7/mns_common/component/classify/classify_constant.py
+-rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.1.1.7/mns_common/component/classify/symbol_classify_api.py
+-rw-rw-rw-   0        0        0     5068 2024-05-15 08:05:35.000000 mns_common-1.1.1.7/mns_common/component/common_service_fun_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.225938 mns_common-1.1.1.7/mns_common/component/company/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.1.7/mns_common/component/company/__init__.py
+-rw-rw-rw-   0        0        0     7217 2024-05-17 13:48:14.000000 mns_common-1.1.1.7/mns_common/component/company/company_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.227932 mns_common-1.1.1.7/mns_common/component/concept/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.1.7/mns_common/component/concept/__init__.py
+-rw-rw-rw-   0        0        0     3235 2024-05-09 14:23:16.000000 mns_common-1.1.1.7/mns_common/component/concept/kpl_concept_common_service_api.py
+-rw-rw-rw-   0        0        0     9637 2024-04-30 09:46:26.000000 mns_common-1.1.1.7/mns_common/component/concept/ths_concept_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.228930 mns_common-1.1.1.7/mns_common/component/data/
+-rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.1.1.7/mns_common/component/data/__init__.py
+-rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.1.1.7/mns_common/component/data/data_init_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.229927 mns_common-1.1.1.7/mns_common/component/industry/
+-rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.1.1.7/mns_common/component/industry/__init__.py
+-rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.1.1.7/mns_common/component/industry/ths_industry_index_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.229927 mns_common-1.1.1.7/mns_common/component/k_line/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.1.7/mns_common/component/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.231922 mns_common-1.1.1.7/mns_common/component/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.1.1.7/mns_common/component/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.1.1.7/mns_common/component/k_line/clean/k_line_param.py
+-rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.1.1.7/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.231922 mns_common-1.1.1.7/mns_common/component/k_line/common/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.1.1.7/mns_common/component/k_line/common/__init__.py
+-rw-rw-rw-   0        0        0     4449 2023-12-29 04:25:17.000000 mns_common-1.1.1.7/mns_common/component/k_line/common/k_line_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.233916 mns_common-1.1.1.7/mns_common/component/k_line/patterns/
+-rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.1.1.7/mns_common/component/k_line/patterns/__init__.py
+-rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.1.1.7/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
+-rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.1.1.7/mns_common/component/k_line/patterns/pattern_Enum.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.234914 mns_common-1.1.1.7/mns_common/component/real_time/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.1.7/mns_common/component/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.1.1.7/mns_common/component/real_time/real_time_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.235911 mns_common-1.1.1.7/mns_common/component/self_choose/
+-rw-rw-rw-   0        0        0      163 2024-05-14 15:36:27.000000 mns_common-1.1.1.7/mns_common/component/self_choose/__init__.py
+-rw-rw-rw-   0        0        0     2232 2024-05-16 05:56:38.000000 mns_common-1.1.1.7/mns_common/component/self_choose/black_list_service_api.py
+-rw-rw-rw-   0        0        0      519 2024-05-18 07:01:06.000000 mns_common-1.1.1.7/mns_common/component/self_choose/self_choose_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.236909 mns_common-1.1.1.7/mns_common/component/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-27 12:44:35.000000 mns_common-1.1.1.7/mns_common/component/trade/__init__.py
+-rw-rw-rw-   0        0        0     3120 2024-05-08 07:34:38.000000 mns_common-1.1.1.7/mns_common/component/trade/trade_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.237909 mns_common-1.1.1.7/mns_common/component/trade_date/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.1.7/mns_common/component/trade_date/__init__.py
+-rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.1.1.7/mns_common/component/trade_date/trade_date_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.238907 mns_common-1.1.1.7/mns_common/component/zt/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.1.7/mns_common/component/zt/__init__.py
+-rw-rw-rw-   0        0        0     8650 2024-05-12 14:00:57.000000 mns_common-1.1.1.7/mns_common/component/zt/zt_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.240929 mns_common-1.1.1.7/mns_common/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.1.1.7/mns_common/constant/__init__.py
+-rw-rw-rw-   0        0        0     2016 2024-05-20 14:21:50.000000 mns_common-1.1.1.7/mns_common/constant/db_name_constant.py
+-rw-rw-rw-   0        0        0     4507 2024-01-25 14:21:07.000000 mns_common-1.1.1.7/mns_common/constant/kpl_selection_no_choose_constant.py
+-rw-rw-rw-   0        0        0      347 2024-05-01 15:03:02.000000 mns_common-1.1.1.7/mns_common/constant/self_choose_constant.py
+-rw-rw-rw-   0        0        0    12240 2024-03-11 15:08:57.000000 mns_common-1.1.1.7/mns_common/constant/ths_concept_no_choose_constant.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.241927 mns_common-1.1.1.7/mns_common/db/
+-rw-rw-rw-   0        0        0    10816 2024-04-24 14:49:25.000000 mns_common-1.1.1.7/mns_common/db/MongodbUtil.py
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.1.1.7/mns_common/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.244919 mns_common-1.1.1.7/mns_common/utils/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.1.1.7/mns_common/utils/__init__.py
+-rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.1.1.7/mns_common/utils/async_fun.py
+-rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.1.1.7/mns_common/utils/data_frame_util.py
+-rw-rw-rw-   0        0        0     7379 2023-12-21 03:38:02.000000 mns_common-1.1.1.7/mns_common/utils/date_handle_util.py
+-rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.1.1.7/mns_common/utils/ip_util.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:22:03.244919 mns_common-1.1.1.7/mns_common.egg-info/
+-rw-rw-rw-   0        0        0       59 2024-05-20 14:22:03.000000 mns_common-1.1.1.7/mns_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3872 2024-05-20 14:22:03.000000 mns_common-1.1.1.7/mns_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 14:22:03.000000 mns_common-1.1.1.7/mns_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-20 14:22:03.000000 mns_common-1.1.1.7/mns_common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 14:22:03.245916 mns_common-1.1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      466 2024-05-20 14:21:50.000000 mns_common-1.1.1.7/setup.py
```

### Comparing `mns_common-1.1.1.6/README.md` & `mns_common-1.1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/akshare/k_line_api.py` & `mns_common-1.1.1.7/mns_common/api/akshare/k_line_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/akshare/stock_bid_ask_api.py` & `mns_common-1.1.1.7/mns_common/api/akshare/stock_bid_ask_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/akshare/stock_dt_pool.py` & `mns_common-1.1.1.7/mns_common/api/akshare/stock_dt_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/akshare/stock_zb_pool.py` & `mns_common-1.1.1.7/mns_common/api/akshare/stock_zb_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/akshare/stock_zt_pool_api.py` & `mns_common-1.1.1.7/mns_common/api/akshare/stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/akshare/yjyg_sync_api.py` & `mns_common-1.1.1.7/mns_common/api/akshare/yjyg_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/em/east_money_stock_api.py` & `mns_common-1.1.1.7/mns_common/api/em/east_money_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py` & `mns_common-1.1.1.7/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/em/east_money_stock_hk_api.py` & `mns_common-1.1.1.7/mns_common/api/em/east_money_stock_hk_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/em/east_money_stock_v2_api.py` & `mns_common-1.1.1.7/mns_common/api/em/east_money_stock_v2_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/em/em_concept_index_api.py` & `mns_common-1.1.1.7/mns_common/api/em/em_concept_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/kpl/common/kpl_common_api.py` & `mns_common-1.1.1.7/mns_common/api/kpl/common/kpl_common_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/kpl/concept/kpl_concept_api.py` & `mns_common-1.1.1.7/mns_common/api/kpl/concept/kpl_concept_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/kpl/constant/kpl_constant.py` & `mns_common-1.1.1.7/mns_common/api/kpl/constant/kpl_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/kpl/industry/kpl_industry_api.py` & `mns_common-1.1.1.7/mns_common/api/kpl/industry/kpl_industry_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/kpl/selection/kpl_selection_plate_api.py` & `mns_common-1.1.1.7/mns_common/api/kpl/selection/kpl_selection_plate_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py` & `mns_common-1.1.1.7/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py` & `mns_common-1.1.1.7/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/kpl/symbol/symbol_his_quotes_api.py` & `mns_common-1.1.1.7/mns_common/api/kpl/symbol/symbol_his_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/msg/push_msg_api.py` & `mns_common-1.1.1.7/mns_common/api/msg/push_msg_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/ths/ths_big_deal_api.py` & `mns_common-1.1.1.7/mns_common/api/ths/ths_big_deal_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/ths/ths_stock_api.py` & `mns_common-1.1.1.7/mns_common/api/ths/ths_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/api/ths/ths_stock_zt_pool_api.py` & `mns_common-1.1.1.7/mns_common/api/ths/ths_stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/component/cache/cache_service.py` & `mns_common-1.1.1.7/mns_common/component/cache/cache_service.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/component/classify/classify_constant.py` & `mns_common-1.1.1.7/mns_common/component/classify/classify_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/component/classify/symbol_classify_api.py` & `mns_common-1.1.1.7/mns_common/component/classify/symbol_classify_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/component/common_service_fun_api.py` & `mns_common-1.1.1.7/mns_common/component/common_service_fun_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/component/company/company_common_service_api.py` & `mns_common-1.1.1.7/mns_common/component/company/company_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/component/concept/kpl_concept_common_service_api.py` & `mns_common-1.1.1.7/mns_common/component/concept/kpl_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/component/concept/ths_concept_common_service_api.py` & `mns_common-1.1.1.7/mns_common/component/concept/ths_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/component/data/data_init_api.py` & `mns_common-1.1.1.7/mns_common/component/data/data_init_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/component/industry/ths_industry_index_api.py` & `mns_common-1.1.1.7/mns_common/component/industry/ths_industry_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py` & `mns_common-1.1.1.7/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/component/k_line/common/k_line_common_service_api.py` & `mns_common-1.1.1.7/mns_common/component/k_line/common/k_line_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/component/k_line/patterns/k_line_patterns_service_api.py` & `mns_common-1.1.1.7/mns_common/component/k_line/patterns/k_line_patterns_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/component/real_time/real_time_common_service_api.py` & `mns_common-1.1.1.7/mns_common/component/real_time/real_time_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/component/self_choose/black_list_service_api.py` & `mns_common-1.1.1.7/mns_common/component/self_choose/black_list_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/component/self_choose/self_choose_service_api.py` & `mns_common-1.1.1.7/mns_common/component/self_choose/self_choose_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/component/trade/trade_service_api.py` & `mns_common-1.1.1.7/mns_common/component/trade/trade_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/component/trade_date/trade_date_common_service_api.py` & `mns_common-1.1.1.7/mns_common/component/trade_date/trade_date_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/component/zt/zt_common_service_api.py` & `mns_common-1.1.1.7/mns_common/component/zt/zt_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/constant/db_name_constant.py` & `mns_common-1.1.1.7/mns_common/constant/db_name_constant.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,16 +29,20 @@
 
 # 同花顺概念详情表
 THS_STOCK_CONCEPT_DETAIL = "ths_stock_concept_detail"
 # 今日排除买入股票
 TODAY_EXCLUDE_STOCK = "today_exclude_stocks"
 # 今日买入股票
 BUY_STOCK_NAME = 'trade_stocks'
-#  COMPANY_INFO
+
+#  公司信息表
 COMPANY_INFO = 'company_info'
+#  公司信息历史表
+COMPANY_INFO_HIS = 'company_info_his'
+
 # TODAY_NEW_CONCEPT_LIST
 TODAY_NEW_CONCEPT_LIST = 'today_new_concept_list'
 
 # 开票啦历史数据
 KPL_BEST_CHOOSE_HIS = 'kpl_best_choose_his'
 
 # 开票啦每日数据
```

### Comparing `mns_common-1.1.1.6/mns_common/constant/kpl_selection_no_choose_constant.py` & `mns_common-1.1.1.7/mns_common/constant/kpl_selection_no_choose_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/constant/ths_concept_no_choose_constant.py` & `mns_common-1.1.1.7/mns_common/constant/ths_concept_no_choose_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/db/MongodbUtil.py` & `mns_common-1.1.1.7/mns_common/db/MongodbUtil.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/utils/data_frame_util.py` & `mns_common-1.1.1.7/mns_common/utils/data_frame_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common/utils/date_handle_util.py` & `mns_common-1.1.1.7/mns_common/utils/date_handle_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.1.6/mns_common.egg-info/SOURCES.txt` & `mns_common-1.1.1.7/mns_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

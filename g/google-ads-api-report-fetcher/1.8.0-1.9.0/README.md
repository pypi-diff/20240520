# Comparing `tmp/google-ads-api-report-fetcher-1.8.0.tar.gz` & `tmp/google-ads-api-report-fetcher-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-ads-api-report-fetcher-1.8.0.tar", last modified: Thu Jul 13 06:30:14 2023, max compression
+gzip compressed data, was "google-ads-api-report-fetcher-1.9.0.tar", last modified: Wed Jul 26 11:06:32 2023, max compression
```

## Comparing `google-ads-api-report-fetcher-1.8.0.tar` & `google-ads-api-report-fetcher-1.9.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-13 06:30:14.972661 google-ads-api-report-fetcher-1.8.0/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4202 2023-07-13 06:30:14.972661 google-ads-api-report-fetcher-1.8.0/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3489 2023-03-16 20:20:32.000000 google-ads-api-report-fetcher-1.8.0/README.md
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-13 06:30:14.960665 google-ads-api-report-fetcher-1.8.0/gaarf/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.8.0/gaarf/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     8325 2023-07-13 06:29:25.000000 google-ads-api-report-fetcher-1.8.0/gaarf/api_clients.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      916 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.8.0/gaarf/base_query.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2717 2023-07-07 14:27:09.000000 google-ads-api-report-fetcher-1.8.0/gaarf/bq_executor.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-13 06:30:14.964663 google-ads-api-report-fetcher-1.8.0/gaarf/cli/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.8.0/gaarf/cli/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3959 2023-06-19 15:45:10.000000 google-ads-api-report-fetcher-1.8.0/gaarf/cli/bq.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7649 2023-07-13 06:29:25.000000 google-ads-api-report-fetcher-1.8.0/gaarf/cli/gaarf.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4210 2023-06-07 13:55:49.000000 google-ads-api-report-fetcher-1.8.0/gaarf/cli/postprocessor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2967 2023-07-13 06:29:25.000000 google-ads-api-report-fetcher-1.8.0/gaarf/cli/simulator.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3859 2023-06-19 15:45:10.000000 google-ads-api-report-fetcher-1.8.0/gaarf/cli/sql.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    13434 2023-06-21 17:43:19.000000 google-ads-api-report-fetcher-1.8.0/gaarf/cli/utils.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-13 06:30:14.968662 google-ads-api-report-fetcher-1.8.0/gaarf/io/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.8.0/gaarf/io/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1842 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.8.0/gaarf/io/formatter.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1870 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.8.0/gaarf/io/reader.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    10698 2023-07-13 06:29:25.000000 google-ads-api-report-fetcher-1.8.0/gaarf/io/writer.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    10596 2023-05-29 10:48:19.000000 google-ads-api-report-fetcher-1.8.0/gaarf/parsers.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    11869 2023-07-07 09:02:33.000000 google-ads-api-report-fetcher-1.8.0/gaarf/query_editor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    11681 2023-07-12 20:43:36.000000 google-ads-api-report-fetcher-1.8.0/gaarf/query_executor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2927 2023-07-13 06:29:25.000000 google-ads-api-report-fetcher-1.8.0/gaarf/query_post_processor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     5774 2023-07-03 13:01:14.000000 google-ads-api-report-fetcher-1.8.0/gaarf/report.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4088 2023-06-16 18:39:22.000000 google-ads-api-report-fetcher-1.8.0/gaarf/simulation.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1275 2023-06-07 14:38:11.000000 google-ads-api-report-fetcher-1.8.0/gaarf/sql_executor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2295 2023-07-12 20:43:36.000000 google-ads-api-report-fetcher-1.8.0/gaarf/utils.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      158 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.8.0/gaarf/wip.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-13 06:30:14.968662 google-ads-api-report-fetcher-1.8.0/google_ads_api_report_fetcher.egg-info/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4202 2023-07-13 06:30:14.000000 google-ads-api-report-fetcher-1.8.0/google_ads_api_report_fetcher.egg-info/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1169 2023-07-13 06:30:14.000000 google-ads-api-report-fetcher-1.8.0/google_ads_api_report_fetcher.egg-info/SOURCES.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2023-07-13 06:30:14.000000 google-ads-api-report-fetcher-1.8.0/google_ads_api_report_fetcher.egg-info/dependency_links.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      214 2023-07-13 06:30:14.000000 google-ads-api-report-fetcher-1.8.0/google_ads_api_report_fetcher.egg-info/entry_points.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      192 2023-07-13 06:30:14.000000 google-ads-api-report-fetcher-1.8.0/google_ads_api_report_fetcher.egg-info/requires.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       12 2023-07-13 06:30:14.000000 google-ads-api-report-fetcher-1.8.0/google_ads_api_report_fetcher.egg-info/top_level.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       63 2023-07-13 06:30:14.976659 google-ads-api-report-fetcher-1.8.0/setup.cfg
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1723 2023-07-13 06:29:49.000000 google-ads-api-report-fetcher-1.8.0/setup.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-13 06:30:14.968662 google-ads-api-report-fetcher-1.8.0/tests/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.8.0/tests/__init__.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-13 06:30:14.972661 google-ads-api-report-fetcher-1.8.0/tests/unit/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.8.0/tests/unit/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      748 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.8.0/tests/unit/test_base_query.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      423 2023-06-06 14:22:27.000000 google-ads-api-report-fetcher-1.8.0/tests/unit/test_bq_executor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    11446 2023-06-21 17:43:19.000000 google-ads-api-report-fetcher-1.8.0/tests/unit/test_cli_utils.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7233 2023-07-03 13:01:14.000000 google-ads-api-report-fetcher-1.8.0/tests/unit/test_parsers.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4835 2023-07-03 13:01:14.000000 google-ads-api-report-fetcher-1.8.0/tests/unit/test_query_editor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4771 2023-06-16 12:21:00.000000 google-ads-api-report-fetcher-1.8.0/tests/unit/test_query_post_processor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      891 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.8.0/tests/unit/test_reader.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7620 2023-07-03 13:01:14.000000 google-ads-api-report-fetcher-1.8.0/tests/unit/test_report.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2487 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.8.0/tests/unit/test_simulation.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3778 2023-07-13 06:29:25.000000 google-ads-api-report-fetcher-1.8.0/tests/unit/test_writer.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-26 11:06:32.593991 google-ads-api-report-fetcher-1.9.0/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     8890 2023-07-26 11:06:32.593991 google-ads-api-report-fetcher-1.9.0/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     8155 2023-07-25 06:41:13.000000 google-ads-api-report-fetcher-1.9.0/README.md
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-26 11:06:32.577991 google-ads-api-report-fetcher-1.9.0/gaarf/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.9.0/gaarf/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     8325 2023-07-13 06:29:25.000000 google-ads-api-report-fetcher-1.9.0/gaarf/api_clients.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      916 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.9.0/gaarf/base_query.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2717 2023-07-07 14:27:09.000000 google-ads-api-report-fetcher-1.9.0/gaarf/bq_executor.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-26 11:06:32.581991 google-ads-api-report-fetcher-1.9.0/gaarf/cli/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.9.0/gaarf/cli/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3959 2023-07-14 11:11:00.000000 google-ads-api-report-fetcher-1.9.0/gaarf/cli/bq.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7640 2023-07-25 06:41:13.000000 google-ads-api-report-fetcher-1.9.0/gaarf/cli/gaarf.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4210 2023-06-07 13:55:49.000000 google-ads-api-report-fetcher-1.9.0/gaarf/cli/postprocessor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2967 2023-07-13 06:29:25.000000 google-ads-api-report-fetcher-1.9.0/gaarf/cli/simulator.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3859 2023-06-19 15:45:10.000000 google-ads-api-report-fetcher-1.9.0/gaarf/cli/sql.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    13434 2023-07-14 11:13:55.000000 google-ads-api-report-fetcher-1.9.0/gaarf/cli/utils.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-26 11:06:32.581991 google-ads-api-report-fetcher-1.9.0/gaarf/io/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.9.0/gaarf/io/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1842 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.9.0/gaarf/io/formatter.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1870 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.9.0/gaarf/io/reader.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    10698 2023-07-13 06:29:25.000000 google-ads-api-report-fetcher-1.9.0/gaarf/io/writer.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    10596 2023-05-29 10:48:19.000000 google-ads-api-report-fetcher-1.9.0/gaarf/parsers.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    11869 2023-07-07 09:02:33.000000 google-ads-api-report-fetcher-1.9.0/gaarf/query_editor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    15568 2023-07-25 06:41:13.000000 google-ads-api-report-fetcher-1.9.0/gaarf/query_executor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2927 2023-07-13 06:29:25.000000 google-ads-api-report-fetcher-1.9.0/gaarf/query_post_processor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     5968 2023-07-25 06:41:13.000000 google-ads-api-report-fetcher-1.9.0/gaarf/report.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4084 2023-07-25 06:41:13.000000 google-ads-api-report-fetcher-1.9.0/gaarf/simulation.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1275 2023-06-07 14:38:11.000000 google-ads-api-report-fetcher-1.9.0/gaarf/sql_executor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2463 2023-07-25 06:55:59.000000 google-ads-api-report-fetcher-1.9.0/gaarf/utils.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      158 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.9.0/gaarf/wip.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-26 11:06:32.581991 google-ads-api-report-fetcher-1.9.0/google_ads_api_report_fetcher.egg-info/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     8890 2023-07-26 11:06:32.000000 google-ads-api-report-fetcher-1.9.0/google_ads_api_report_fetcher.egg-info/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1169 2023-07-26 11:06:32.000000 google-ads-api-report-fetcher-1.9.0/google_ads_api_report_fetcher.egg-info/SOURCES.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2023-07-26 11:06:32.000000 google-ads-api-report-fetcher-1.9.0/google_ads_api_report_fetcher.egg-info/dependency_links.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      214 2023-07-26 11:06:32.000000 google-ads-api-report-fetcher-1.9.0/google_ads_api_report_fetcher.egg-info/entry_points.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      192 2023-07-26 11:06:32.000000 google-ads-api-report-fetcher-1.9.0/google_ads_api_report_fetcher.egg-info/requires.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       12 2023-07-26 11:06:32.000000 google-ads-api-report-fetcher-1.9.0/google_ads_api_report_fetcher.egg-info/top_level.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       63 2023-07-26 11:06:32.593991 google-ads-api-report-fetcher-1.9.0/setup.cfg
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1751 2023-07-25 13:49:28.000000 google-ads-api-report-fetcher-1.9.0/setup.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-26 11:06:32.585991 google-ads-api-report-fetcher-1.9.0/tests/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.9.0/tests/__init__.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-07-26 11:06:32.589991 google-ads-api-report-fetcher-1.9.0/tests/unit/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.9.0/tests/unit/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      748 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.9.0/tests/unit/test_base_query.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      423 2023-06-06 14:22:27.000000 google-ads-api-report-fetcher-1.9.0/tests/unit/test_bq_executor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    11446 2023-06-21 17:43:19.000000 google-ads-api-report-fetcher-1.9.0/tests/unit/test_cli_utils.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7233 2023-07-03 13:01:14.000000 google-ads-api-report-fetcher-1.9.0/tests/unit/test_parsers.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4835 2023-07-03 13:01:14.000000 google-ads-api-report-fetcher-1.9.0/tests/unit/test_query_editor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4771 2023-06-16 12:21:00.000000 google-ads-api-report-fetcher-1.9.0/tests/unit/test_query_post_processor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      891 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.9.0/tests/unit/test_reader.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7620 2023-07-24 06:55:49.000000 google-ads-api-report-fetcher-1.9.0/tests/unit/test_report.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2487 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.9.0/tests/unit/test_simulation.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3778 2023-07-13 06:29:25.000000 google-ads-api-report-fetcher-1.9.0/tests/unit/test_writer.py
```

### Comparing `google-ads-api-report-fetcher-1.8.0/gaarf/api_clients.py` & `google-ads-api-report-fetcher-1.9.0/gaarf/api_clients.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/gaarf/base_query.py` & `google-ads-api-report-fetcher-1.9.0/gaarf/base_query.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/gaarf/bq_executor.py` & `google-ads-api-report-fetcher-1.9.0/gaarf/bq_executor.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/gaarf/cli/bq.py` & `google-ads-api-report-fetcher-1.9.0/gaarf/cli/bq.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/gaarf/cli/gaarf.py` & `google-ads-api-report-fetcher-1.9.0/gaarf/cli/gaarf.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 
     if config.params:
         config = initialize_runtime_parameters(config)
     logger.debug("initialized config: %s", config)
 
     ads_client = api_clients.GoogleAdsApiClient(
         config_dict=google_ads_config_dict, version=f"v{config.api_version}")
+    ads_query_executor = query_executor.AdsQueryExecutor(ads_client)
     reader_factory = reader.ReaderFactory()
     reader_client = reader_factory.create_reader(main_args.input)
 
     if config.customer_ids_query:
         customer_ids_query = config.customer_ids_query
     elif config.customer_ids_query_file:
         file_reader = reader_factory.create_reader("file")
@@ -130,22 +131,21 @@
     if main_args.disable_account_expansion:
         logger.info(
             "Skipping account expansion because of disable_account_expansion flag"
         )
         customer_ids = config.account if isinstance(
             config.account, MutableSequence) else [config.account]
     else:
-        customer_ids = utils.get_customer_ids(ads_client, config.account,
+        customer_ids = ads_query_executor.expand_mcc(config.account,
                                               customer_ids_query)
     if customer_ids:
         writer_client = writer.WriterFactory().create_writer(
             config.output, **config.writer_params)
         if config.output == "bq":
             _ = writer_client.create_or_get_dataset()
-        ads_query_executor = query_executor.AdsQueryExecutor(ads_client)
 
         logger.info("Total number of customer_ids is %d, accounts=[%s]",
                     len(customer_ids), ",".join(map(str, customer_ids)))
 
         if main_args.parallel_queries:
             logger.info("Running queries in parallel")
             with futures.ThreadPoolExecutor() as executor:
```

### Comparing `google-ads-api-report-fetcher-1.8.0/gaarf/cli/postprocessor.py` & `google-ads-api-report-fetcher-1.9.0/gaarf/cli/postprocessor.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/gaarf/cli/simulator.py` & `google-ads-api-report-fetcher-1.9.0/gaarf/cli/simulator.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/gaarf/cli/sql.py` & `google-ads-api-report-fetcher-1.9.0/gaarf/cli/sql.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/gaarf/cli/utils.py` & `google-ads-api-report-fetcher-1.9.0/gaarf/cli/utils.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/gaarf/io/formatter.py` & `google-ads-api-report-fetcher-1.9.0/gaarf/io/formatter.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/gaarf/io/reader.py` & `google-ads-api-report-fetcher-1.9.0/gaarf/io/reader.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/gaarf/io/writer.py` & `google-ads-api-report-fetcher-1.9.0/gaarf/io/writer.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/gaarf/parsers.py` & `google-ads-api-report-fetcher-1.9.0/gaarf/parsers.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/gaarf/query_editor.py` & `google-ads-api-report-fetcher-1.9.0/gaarf/query_editor.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/gaarf/query_executor.py` & `google-ads-api-report-fetcher-1.9.0/gaarf/query_executor.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,28 +8,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
+from collections.abc import MutableSequence
 from concurrent import futures
 from enum import Enum, auto
 import itertools
 from google.ads.googleads.errors import GoogleAdsException  # type: ignore
 import logging
 from google.api_core import exceptions
 from tenacity import Retrying, RetryError, retry_if_exception_type, stop_after_attempt, wait_exponential
+import warnings
 
 from . import parsers
 from . import api_clients
 from .query_editor import QuerySpecification, QueryElements
-from .report import GaarfReport
+from .report import GaarfReport, GaarfRow
 from .io import writer, reader  # type: ignore
 
+
 logger = logging.getLogger(__name__)
 
 
 class OptimizeStrategy(Enum):
     NONE = auto()
     BATCH = auto()
     PROTOBUF = auto()
@@ -37,51 +40,89 @@
 
 
 class AdsReportFetcher:
     """Class responsible for getting data from Ads API.
 
     Attributes:
         api_client: a client used for connecting to Ads API.
-        customer_ids: account_id(s) from which data will be fetched.
-          Expects list of non-MCC accounts, which can be expanded from MCC
-          by calling `utils.get_customer_ids(ads_api_client, mcc_id)` function.
     """
 
-    def __init__(self, api_client: api_clients.BaseClient,
-                 customer_ids: Union[Sequence[str], str]) -> None:
-
+    def __init__(self,
+                 api_client: api_clients.BaseClient,
+                 customer_ids: Optional[Any] = None) -> None:
         self.api_client = api_client
-        self.customer_ids = [
-            customer_ids
-        ] if not isinstance(customer_ids, list) else customer_ids
+        if customer_ids:
+            warnings.warn(
+                "`AdsReportFetcher` will deprecate passing `customer_ids` to `__init__` method. "
+                "Consider passing list of customer_ids to `AdsReportFetcher.fetch` method",
+                category=DeprecationWarning,
+                stacklevel=3)
+            self.customer_ids = [
+                customer_ids
+            ] if not isinstance(customer_ids, list) else customer_ids
+
+    def expand_mcc(self,
+                   customer_ids: Union[str, MutableSequence[str]],
+                   customer_ids_query: Optional[str] = None) -> List[str]:
+        return self._get_customer_ids(customer_ids, customer_ids_query)
 
     def fetch(self,
               query_specification: Union[str, QueryElements],
+              customer_ids: Optional[Union[List[str], str]] = None,
+              customer_ids_query: Optional[str] = None,
+              expand_mcc: bool = False,
+              args: Optional[Dict[str, Any]] = None,
               optimize_strategy: str = "NONE") -> GaarfReport:
         """Fetches data from Ads API based on query_specification.
 
         Args:
-            query_specification: query text that will be passed to Ads API
+            query_specification: Query text that will be passed to Ads API
                 alongside column_names, customizers and virtual columns.
+            customer_ids: Account(s) for from which data should be fetched.
+            custom_query: GAQL query used to reduce the number of customer_ids.
+            expand_mcc: Whether to perform expansion of root customer_ids
+                into leaf accounts.
+            args: Arguments that need to be passed to the query
             optimize_strategy: strategy for speeding up query execution
                 ("NONE", "PROTOBUF", "BATCH", "BATCH_PROTOBUF").
 
         Returns:
             GaarfReport with results of query execution.
         """
 
+        if isinstance(self.api_client, api_clients.GoogleAdsApiClient):
+            if not customer_ids:
+                warnings.warn(
+                    "`AdsReportFetcher` will require passing `customer_ids` to `fetch` method.",
+                    category=DeprecationWarning,
+                    stacklevel=3)
+                if hasattr(self, "customer_ids"):
+                    if not self.customer_ids:
+                        raise ValueError(
+                            "Please specify add `customer_ids` to `fetch` method")
+                    customer_ids = self.customer_ids
+            else:
+                if expand_mcc:
+                    customer_ids = self.expand_mcc(customer_ids,
+                                                   customer_ids_query)
+                customer_ids = [
+                    customer_ids
+                ] if not isinstance(customer_ids, list) else customer_ids
+        else:
+            customer_ids = []
         total_results: List[List[Tuple[Any]]] = []
         is_fake_report = False
         if not isinstance(query_specification, QueryElements):
             query_specification = QuerySpecification(
                 text=str(query_specification),
+                args=args,
                 api_version=self.api_client.api_version).generate()
 
         parser = parsers.GoogleAdsRowParser(query_specification)
-        for customer_id in self.customer_ids:
+        for customer_id in customer_ids:
             logger.debug("Running query %s for customer_id %s",
                          query_specification.query_title, customer_id)
             try:
                 results = self._parse_ads_response(
                     query_specification, customer_id, parser,
                     getattr(OptimizeStrategy, optimize_strategy))
                 total_results.extend(results)
@@ -100,15 +141,16 @@
             is_fake_report = True
             if not isinstance(self.api_client, api_clients.BaseClient):
                 logger.warning(
                     "Query %s generated zero results, using placeholders to infer schema",
                     query_specification.query_title)
         return GaarfReport(results=total_results,
                            column_names=query_specification.column_names,
-                           is_fake=is_fake_report)
+                           is_fake=is_fake_report,
+                           query_specification=query_specification)
 
     def _parse_ads_response(
         self,
         query_specification: QueryElements,
         customer_id: str,
         parser: parsers.GoogleAdsRowParser,
         optimize_strategy: OptimizeStrategy = OptimizeStrategy.NONE
@@ -213,25 +255,63 @@
             batch: sequence of GoogleAdsRow that needs to be parsed.
         Returns:
             Parsed rows for a batch.
         """
 
         return [parser.parse_ads_row(row) for row in batch]
 
+    def _get_customer_ids(
+            self,
+            seed_customer_ids: Union[str, MutableSequence[str]],
+            customer_ids_query: Optional[str] = None) -> List[str]:
+        """Gets list of customer_ids from an MCC account.
+
+        Args:
+            customer_ids: MCC account_id(s).
+            custom_query: GAQL query used to reduce the number of customer_ids.
+        Returns:
+            All customer_ids from MCC satisfying the condition.
+        """
+
+        query = """
+        SELECT customer_client.id FROM customer_client
+        WHERE customer_client.manager = FALSE AND customer_client.status = "ENABLED"
+        """
+        query_specification = QuerySpecification(query).generate()
+        if not isinstance(seed_customer_ids, MutableSequence):
+            seed_customer_ids = seed_customer_ids.split(",")
+        child_customer_ids = self.fetch(query_specification, seed_customer_ids).to_list()
+        if customer_ids_query:
+            query_specification = QuerySpecification(
+                customer_ids_query).generate()
+            child_customer_ids = self.fetch(query_specification,
+                                                child_customer_ids)
+            child_customer_ids = [
+                row[0] if isinstance(row, GaarfRow) else row
+                for row in child_customer_ids
+            ]
+
+        child_customer_ids = list(
+            set([
+                customer_id for customer_id in child_customer_ids if customer_id != 0
+            ]))
+
+        return child_customer_ids
+
 
 class AdsQueryExecutor:
     """Class responsible for getting data from Ads API and writing it to
         local/remote storage.
 
     Attributes:
         api_client: a client used for connecting to Ads API.
     """
 
     def __init__(self, api_client: api_clients.BaseClient):
-        self.api_client = api_client
+        self.report_fetcher = AdsReportFetcher(api_client)
 
     def execute(self,
                 query_text: str,
                 query_name: str,
                 customer_ids: Union[List[str], str],
                 writer_client: writer.AbsWriter = writer.StdoutWriter(),
                 args: Optional[Dict[str, Any]] = None,
@@ -246,16 +326,21 @@
             args: Arguments that need to be passed to the query
             optimize_strategy: strategy for speeding up query execution
                 ("NONE", "PROTOBUF", "BATCH", "BATCH_PROTOBUF")
         """
 
         query_specification = QuerySpecification(
             query_text, query_name, args,
-            self.api_client.api_version).generate()
-        report_fetcher = AdsReportFetcher(self.api_client, customer_ids)
-        results = report_fetcher.fetch(query_specification,
-                                       optimize_performance)
+            self.report_fetcher.api_client.api_version).generate()
+        results = self.report_fetcher.fetch(query_specification=query_specification,
+                                       customer_ids=customer_ids,
+                                       optimize_strategy=optimize_performance)
         logger.debug("Start writing data for query %s via %s writer",
                      query_specification.query_title, type(writer_client))
         writer_client.write(results, query_specification.query_title)
         logger.debug("Finish writing data for query %s via %s writer",
                      query_specification.query_title, type(writer_client))
+
+    def expand_mcc(self,
+                   customer_ids: Union[str, MutableSequence[str]],
+                   customer_ids_query: Optional[str] = None) -> List[str]:
+        return self.report_fetcher._get_customer_ids(customer_ids, customer_ids_query)
```

### Comparing `google-ads-api-report-fetcher-1.8.0/gaarf/query_post_processor.py` & `google-ads-api-report-fetcher-1.9.0/gaarf/query_post_processor.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/gaarf/report.py` & `google-ads-api-report-fetcher-1.9.0/gaarf/report.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,30 +8,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Any, Sequence, Union
+from typing import Any, Sequence, Optional, Union
 from collections import abc
 import operator
 import pandas as pd
 
+from .query_editor import QuerySpecification
+
 
 class GaarfReport:
 
     def __init__(self,
                  results: Sequence[Any],
                  column_names: Sequence[str],
-                 is_fake: bool = False):
+                 is_fake: bool = False,
+                 query_specification: Optional[QuerySpecification] = None) -> None:
         self.results = results
         self.column_names = column_names
         self.multi_column_report = len(column_names) > 1
         self.is_fake = is_fake
+        self.query_specification = query_specification
 
     def to_list(self) -> Sequence[Any]:
         return self.results
 
     def to_pandas(self) -> pd.DataFrame:
         return pd.DataFrame(data=self.results, columns=self.column_names)
```

### Comparing `google-ads-api-report-fetcher-1.8.0/gaarf/simulation.py` & `google-ads-api-report-fetcher-1.9.0/gaarf/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 def simulate_data(
     query: str,
     simulator_specification: SimulatorSpecification,
     simulation_helper: Callable = Faker()
 ) -> GaarfReport:
     query_specification = QuerySpecification(query).generate()
     client = BaseClient(simulator_specification.api_version)
-    report_fetcher = AdsReportFetcher(client, [])
+    report_fetcher = AdsReportFetcher(client)
     other_types = client.infer_types(query_specification.fields)
     v = report_fetcher.fetch(query_specification)
     try:
         iter(v.results[0])
         results = v.results[0]
     except TypeError:
         results = [v.results[0]]
```

### Comparing `google-ads-api-report-fetcher-1.8.0/gaarf/sql_executor.py` & `google-ads-api-report-fetcher-1.9.0/gaarf/sql_executor.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/gaarf/utils.py` & `google-ads-api-report-fetcher-1.9.0/gaarf/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,47 +10,49 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.import proto
 
 from typing import Sequence, Union
 from collections.abc import MutableSequence
+import warnings
 
 from .api_clients import GoogleAdsApiClient
 from .query_editor import QuerySpecification
 from .query_executor import AdsReportFetcher
 from .report import GaarfRow
 
 
 def get_customer_ids(ads_client: GoogleAdsApiClient,
                      customer_id: Union[str, MutableSequence[str]],
                      customer_ids_query: str = None) -> Sequence[str]:
     """Gets list of customer_ids from an MCC account.
 
     Args:
         ads_client: GoogleAdsApiClient used for connection.
-        customer_id: MCC account_id.
+        customer_id: MCC account_id(s).
         custom_query: GAQL query used to reduce the number of customer_ids.
     Returns:
-        All customer_ids from MCC safisfying the condition.
+        All customer_ids from MCC satisfying the condition.
     """
 
     query = """
     SELECT customer_client.id FROM customer_client
     WHERE customer_client.manager = FALSE AND customer_client.status = "ENABLED"
     """
+    warnings.warn("`get_customer_ids` will be deprecated, use `AdsReportFetcher.expand_mcc` or `AdsQueryExecutor.expand_mcc` methods instead",
+                 category=DeprecationWarning, stacklevel=3)
     query_specification = QuerySpecification(query).generate()
     if not isinstance(customer_id, MutableSequence):
         customer_id = customer_id.split(",")
-    report_fetcher = AdsReportFetcher(ads_client, customer_id)
-    customer_ids = report_fetcher.fetch(query_specification).to_list()
+    report_fetcher = AdsReportFetcher(ads_client)
+    customer_ids = report_fetcher.fetch(query_specification, customer_id).to_list()
     if customer_ids_query:
-        report_fetcher = AdsReportFetcher(ads_client, customer_ids)
         query_specification = QuerySpecification(customer_ids_query).generate()
-        customer_ids = report_fetcher.fetch(query_specification)
+        customer_ids = report_fetcher.fetch(query_specification, customer_ids)
         customer_ids = [
             row[0] if isinstance(row, GaarfRow) else row
             for row in customer_ids
         ]
 
     customer_ids = list(
         set([customer_id for customer_id in customer_ids if customer_id != 0]))
```

### Comparing `google-ads-api-report-fetcher-1.8.0/google_ads_api_report_fetcher.egg-info/SOURCES.txt` & `google-ads-api-report-fetcher-1.9.0/google_ads_api_report_fetcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/setup.py` & `google-ads-api-report-fetcher-1.9.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     "sqlalchemy": ["sqlalchemy"],
     "simulator": ["Faker"]
 }
 EXTRAS_REQUIRE['full'] = list(set(chain(*EXTRAS_REQUIRE.values())))
 
 setup(
     name="google-ads-api-report-fetcher",
-    version="1.8.0",
+    version="1.9.0",
+    python_requires=">3.9",
     description=
     "Library for fetching reports from Google Ads API and saving them locally / BigQuery.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/google/ads-api-reports-fetcher",
     author="Google Inc. (gTech gPS CSE team)",
     author_email="no-reply@google.com",
```

### Comparing `google-ads-api-report-fetcher-1.8.0/tests/unit/test_base_query.py` & `google-ads-api-report-fetcher-1.9.0/tests/unit/test_base_query.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/tests/unit/test_cli_utils.py` & `google-ads-api-report-fetcher-1.9.0/tests/unit/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/tests/unit/test_parsers.py` & `google-ads-api-report-fetcher-1.9.0/tests/unit/test_parsers.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/tests/unit/test_query_editor.py` & `google-ads-api-report-fetcher-1.9.0/tests/unit/test_query_editor.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/tests/unit/test_query_post_processor.py` & `google-ads-api-report-fetcher-1.9.0/tests/unit/test_query_post_processor.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/tests/unit/test_reader.py` & `google-ads-api-report-fetcher-1.9.0/tests/unit/test_reader.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/tests/unit/test_report.py` & `google-ads-api-report-fetcher-1.9.0/tests/unit/test_report.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/tests/unit/test_simulation.py` & `google-ads-api-report-fetcher-1.9.0/tests/unit/test_simulation.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.8.0/tests/unit/test_writer.py` & `google-ads-api-report-fetcher-1.9.0/tests/unit/test_writer.py`

 * *Files identical despite different names*


# Comparing `tmp/auto-test-common-2.0.8.tar.gz` & `tmp/auto-test-common-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-test-common-2.0.8.tar", last modified: Mon May 13 07:43:13 2024, max compression
+gzip compressed data, was "auto-test-common-2.0.9.tar", last modified: Mon May 20 05:40:49 2024, max compression
```

## Comparing `auto-test-common-2.0.8.tar` & `auto-test-common-2.0.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.688644 auto-test-common-2.0.8/
--rw-r--r--   0 edz        (502) staff       (20)      628 2024-05-13 07:43:13.688822 auto-test-common-2.0.8/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.629199 auto-test-common-2.0.8/auto_test_common.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      628 2024-05-13 07:43:13.000000 auto-test-common-2.0.8/auto_test_common.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1821 2024-05-13 07:43:13.000000 auto-test-common-2.0.8/auto_test_common.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2024-05-13 07:43:13.000000 auto-test-common-2.0.8/auto_test_common.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2024-05-13 07:43:13.000000 auto-test-common-2.0.8/auto_test_common.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      727 2024-05-13 07:43:13.000000 auto-test-common-2.0.8/auto_test_common.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2024-05-13 07:43:13.000000 auto-test-common-2.0.8/auto_test_common.egg-info/top_level.txt
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.629737 auto-test-common-2.0.8/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-2.0.8/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.633904 auto-test-common-2.0.8/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-2.0.8/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     5450 2024-04-24 07:01:06.000000 auto-test-common-2.0.8/common/autotest/assert_function.py
--rw-r--r--   0 edz        (502) staff       (20)    12600 2024-05-11 02:32:19.000000 auto-test-common-2.0.8/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     8348 2024-05-10 01:35:28.000000 auto-test-common-2.0.8/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    14203 2024-04-24 05:16:27.000000 auto-test-common-2.0.8/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.636966 auto-test-common-2.0.8/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-2.0.8/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     8960 2024-05-13 07:43:05.000000 auto-test-common-2.0.8/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-2.0.8/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-2.0.8/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.638411 auto-test-common-2.0.8/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.8/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-2.0.8/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.647514 auto-test-common-2.0.8/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-2.0.8/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    25961 2024-04-24 05:16:27.000000 auto-test-common-2.0.8/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)      426 2024-04-24 00:46:49.000000 auto-test-common-2.0.8/common/data/eval_data_handle.py
--rw-r--r--   0 edz        (502) staff       (20)     7933 2024-04-24 05:16:27.000000 auto-test-common-2.0.8/common/data/faker_handle.py
--rw-r--r--   0 edz        (502) staff       (20)    12614 2024-04-24 05:16:27.000000 auto-test-common-2.0.8/common/data/handle_common.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-2.0.8/common/data/template_data.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.654759 auto-test-common-2.0.8/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.8/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-2.0.8/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-2.0.8/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1999 2024-05-13 07:18:24.000000 auto-test-common-2.0.8/common/db/handle_mongo.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-2.0.8/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-2.0.8/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-2.0.8/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.656755 auto-test-common-2.0.8/common/driver/
--rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-2.0.8/common/driver/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-2.0.8/common/driver/api_page.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-2.0.8/common/driver/ui_page.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.662480 auto-test-common-2.0.8/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     5030 2024-04-24 05:16:27.000000 auto-test-common-2.0.8/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-2.0.8/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    10873 2024-04-24 00:46:49.000000 auto-test-common-2.0.8/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-2.0.8/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-2.0.8/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-24 00:46:49.000000 auto-test-common-2.0.8/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-2.0.8/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.663900 auto-test-common-2.0.8/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.8/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-2.0.8/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.672660 auto-test-common-2.0.8/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-2.0.8/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-2.0.8/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-2.0.8/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-2.0.8/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-2.0.8/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    17680 2024-04-24 00:46:49.000000 auto-test-common-2.0.8/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.687842 auto-test-common-2.0.8/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-2.0.8/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1527 2024-04-24 00:46:49.000000 auto-test-common-2.0.8/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     5156 2024-04-24 00:46:49.000000 auto-test-common-2.0.8/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    10707 2024-05-13 07:41:16.000000 auto-test-common-2.0.8/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7770 2024-04-24 00:46:49.000000 auto-test-common-2.0.8/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     5415 2024-04-24 00:46:49.000000 auto-test-common-2.0.8/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13056 2024-04-24 05:10:23.000000 auto-test-common-2.0.8/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-2.0.8/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-2.0.8/common/plugin/my_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-2.0.8/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    23539 2024-05-13 01:17:46.000000 auto-test-common-2.0.8/common/plugin/pytest_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-2.0.8/common/plugin/template_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2090 2024-04-24 00:46:49.000000 auto-test-common-2.0.8/common/plugin/yaml_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      443 2024-05-13 07:43:13.689916 auto-test-common-2.0.8/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     2101 2024-04-30 05:32:18.000000 auto-test-common-2.0.8/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-20 05:40:49.527129 auto-test-common-2.0.9/
+-rw-r--r--   0 edz        (502) staff       (20)      628 2024-05-20 05:40:49.527325 auto-test-common-2.0.9/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-20 05:40:49.487724 auto-test-common-2.0.9/auto_test_common.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      628 2024-05-20 05:40:49.000000 auto-test-common-2.0.9/auto_test_common.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1821 2024-05-20 05:40:49.000000 auto-test-common-2.0.9/auto_test_common.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2024-05-20 05:40:49.000000 auto-test-common-2.0.9/auto_test_common.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2024-05-20 05:40:49.000000 auto-test-common-2.0.9/auto_test_common.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      727 2024-05-20 05:40:49.000000 auto-test-common-2.0.9/auto_test_common.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2024-05-20 05:40:49.000000 auto-test-common-2.0.9/auto_test_common.egg-info/top_level.txt
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-20 05:40:49.488115 auto-test-common-2.0.9/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-2.0.9/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-20 05:40:49.489946 auto-test-common-2.0.9/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-2.0.9/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     5450 2024-04-24 07:01:06.000000 auto-test-common-2.0.9/common/autotest/assert_function.py
+-rw-r--r--   0 edz        (502) staff       (20)    12600 2024-05-11 02:32:19.000000 auto-test-common-2.0.9/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     8348 2024-05-10 01:35:28.000000 auto-test-common-2.0.9/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    14203 2024-04-24 05:16:27.000000 auto-test-common-2.0.9/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-20 05:40:49.491612 auto-test-common-2.0.9/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-2.0.9/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     8995 2024-05-20 01:42:56.000000 auto-test-common-2.0.9/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3753 2024-05-13 07:55:43.000000 auto-test-common-2.0.9/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-2.0.9/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-20 05:40:49.492154 auto-test-common-2.0.9/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.9/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-2.0.9/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-20 05:40:49.494538 auto-test-common-2.0.9/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-2.0.9/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    26253 2024-05-20 05:28:00.000000 auto-test-common-2.0.9/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)      426 2024-04-24 00:46:49.000000 auto-test-common-2.0.9/common/data/eval_data_handle.py
+-rw-r--r--   0 edz        (502) staff       (20)     7933 2024-04-24 05:16:27.000000 auto-test-common-2.0.9/common/data/faker_handle.py
+-rw-r--r--   0 edz        (502) staff       (20)    12584 2024-05-20 05:38:27.000000 auto-test-common-2.0.9/common/data/handle_common.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-2.0.9/common/data/template_data.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-20 05:40:49.496952 auto-test-common-2.0.9/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.9/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-2.0.9/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-2.0.9/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1999 2024-05-13 07:18:24.000000 auto-test-common-2.0.9/common/db/handle_mongo.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-2.0.9/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-2.0.9/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-2.0.9/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-20 05:40:49.498152 auto-test-common-2.0.9/common/driver/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-2.0.9/common/driver/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-2.0.9/common/driver/api_page.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-2.0.9/common/driver/ui_page.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-20 05:40:49.502535 auto-test-common-2.0.9/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     5030 2024-04-24 05:16:27.000000 auto-test-common-2.0.9/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-2.0.9/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    10873 2024-04-24 00:46:49.000000 auto-test-common-2.0.9/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-2.0.9/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-2.0.9/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-24 00:46:49.000000 auto-test-common-2.0.9/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-2.0.9/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-20 05:40:49.504079 auto-test-common-2.0.9/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.9/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-2.0.9/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-20 05:40:49.510750 auto-test-common-2.0.9/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-2.0.9/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-2.0.9/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-2.0.9/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     8595 2024-05-13 08:02:39.000000 auto-test-common-2.0.9/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7366 2024-05-15 05:46:09.000000 auto-test-common-2.0.9/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    17680 2024-04-24 00:46:49.000000 auto-test-common-2.0.9/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-20 05:40:49.526393 auto-test-common-2.0.9/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-2.0.9/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1527 2024-04-24 00:46:49.000000 auto-test-common-2.0.9/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     5156 2024-04-24 00:46:49.000000 auto-test-common-2.0.9/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    10707 2024-05-13 07:41:16.000000 auto-test-common-2.0.9/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7770 2024-04-24 00:46:49.000000 auto-test-common-2.0.9/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     5415 2024-04-24 00:46:49.000000 auto-test-common-2.0.9/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13056 2024-04-24 05:10:23.000000 auto-test-common-2.0.9/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-2.0.9/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-2.0.9/common/plugin/my_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-2.0.9/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    23933 2024-05-16 00:42:26.000000 auto-test-common-2.0.9/common/plugin/pytest_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-2.0.9/common/plugin/template_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2090 2024-04-24 00:46:49.000000 auto-test-common-2.0.9/common/plugin/yaml_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      443 2024-05-20 05:40:49.528178 auto-test-common-2.0.9/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     2101 2024-04-30 05:32:18.000000 auto-test-common-2.0.9/setup.py
```

### Comparing `auto-test-common-2.0.8/PKG-INFO` & `auto-test-common-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 2.0.8
+Version: 2.0.9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-2.0.8/auto_test_common.egg-info/PKG-INFO` & `auto-test-common-2.0.9/auto_test_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 2.0.8
+Version: 2.0.9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-2.0.8/auto_test_common.egg-info/SOURCES.txt` & `auto-test-common-2.0.9/auto_test_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/auto_test_common.egg-info/requires.txt` & `auto-test-common-2.0.9/auto_test_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/autotest/assert_function.py` & `auto-test-common-2.0.9/common/autotest/assert_function.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/autotest/base_requests.py` & `auto-test-common-2.0.9/common/autotest/base_requests.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/autotest/handle_allure.py` & `auto-test-common-2.0.9/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/autotest/handle_assert.py` & `auto-test-common-2.0.9/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/common/api_driver.py` & `auto-test-common-2.0.9/common/common/api_driver.py`

 * *Files 7% similar despite different names*

```diff
@@ -120,22 +120,21 @@
             logger.warning(f'{_data} 转换Json失败')
         return _temp
 
 
     @classmethod
     def getCommontHeader(self, header):
         if header is None:
-            header = {'User-Agent':'Mozilla/5.0 (Windows NT 10.0; Win64; x64) Chrome/83.0.4103.116 Safari/537.36',
-                      'Connection':'keep-alive',
+            header = {'Connection':'keep-alive',
                       'Accept-Encoding':'gzip, deflate, br',
                       'Accept-Language':'zh-CN,zh;q=0.9',
                       'Accept':'*/*'}
         else:
-            if 'User-Agent' not in header:
-                header['User-Agent'] = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) Chrome/83.0.4103.116 Safari/537.36'
+            # if 'User-Agent' not in header:
+            #     header['User-Agent'] = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) Chrome/83.0.4103.116 Safari/537.36'
             if 'Connection' not in header:
                 header['Connection'] = 'keep-alive'
             if 'Accept-Encoding' not in header:
                 header['Accept-Encoding'] = 'gzip, deflate, br'
             if 'Accept-Language' not in header:
                 header['Accept-Language'] = 'zh-CN,zh;q=0.9'
             if 'Accept' not in header:
@@ -155,14 +154,19 @@
                 return _data
         except Exception as e:
             return _data
         return _data
 
     @classmethod
     def handleFile(self,data):
+        try:
+            if isinstance(data, str):
+                data = json.loads(data)
+        except Exception as e:
+            data = data
         if isinstance(data,dict):
             for key in data:
                 if isinstance(data[key], str):
                     from common.file.handle_system import adjust_path
                     _path = adjust_path(data[key])
                     if os.path.exists(path.join(TEST_FILE_PATH, _path)):
                         all_path = os.sep.join([TEST_FILE_PATH, _path])
```

### Comparing `auto-test-common-2.0.8/common/common/constant.py` & `auto-test-common-2.0.9/common/common/constant.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,16 +98,14 @@
     HEADER_CONTENT_TYPE_TEXT = '$.common.request_headers_text'
     HEADER_CONTENT_TYPE_DATA = '$.common.request_headers_data'
     HEADER_CONTENT_TYPE_FORM = '$.common.request_headers_form'
 
 
     #Jira配置：
     JIRA_URL = 'http://jira.ceair.com:8080'
-    #测试
-    #JIRA_URL = 'http://10.18.19.159:8080'
     JIRA_USERNAME = 'jiraUserName'
     JIRA_PASSWORD = 'jiraPassword'
 
     # Jenkis Deploy配置：
     JENKINS_DEPLOY = 'jenkinsDeloyURL'
     JENKINS_DEPLOY_USER = 'jenkinsDeloyUser'
     JENKINS_DEPLOY_TOKEN= 'jenkinsDeloyPassword'
```

### Comparing `auto-test-common-2.0.8/common/common/test.py` & `auto-test-common-2.0.9/common/common/test.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/config/config.py` & `auto-test-common-2.0.9/common/config/config.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/data/data_process.py` & `auto-test-common-2.0.9/common/data/data_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,34 +162,34 @@
         all_path = os.sep.join([TEST_FILE_PATH, file_obj])
         with open(all_path, "wb") as code:
             code.write(content)
         return all_path
 
 
     @classmethod
-    def handle_data_fromat(cls, _template, data=None, _no_content=0, _dataType:bool=False):
+    def handle_data_fromat(cls, _template, data=None, _no_content=0, _dataType:bool=False,_replace:int=0):
         if isinstance(_template, str):
             if isinstance(data, list):
                 _dict = []
                 for _index in range(len(data)):
                     if isinstance(data[_index], dict):
-                        _dict.append(cls.handle_data_fromat(_template, data[_index]))
+                        _dict.append(cls.handle_data_fromat(_template=_template, data=data[_index],_replace=_replace))
                 return _dict
             else:
-                return req_expr(content= _template, data= data, _no_content = _no_content, _dataType = _dataType)
+                return req_expr(content= _template, data= data, _no_content = _no_content, _dataType = _dataType,_replace=_replace)
         else:
             if isinstance(_template, list):
                 for _index in range(len(_template)):
-                    _template[_index] = cls.handle_data_fromat(_template[_index], data, _no_content, _dataType)
+                    _template[_index] = cls.handle_data_fromat(_template=_template[_index], data=data, _no_content=_no_content, _dataType = _dataType,_replace=_replace)
                 return _template
             else:
                 if isinstance(_template, dict):
                     for key in _template.keys():
                         if key.find('$') != 0:
-                            _template[key] = cls.handle_data_fromat(_template[key], data, _no_content, _dataType)
+                            _template[key] = cls.handle_data_fromat(_template=_template[key],  data=data, _no_content=_no_content, _dataType = _dataType,_replace=_replace)
                 return _template
 
 
 
     @classmethod
     def handle_data(cls, variable: str, jsonformat:bool=True, _replace:int=0) -> dict:
         """请求数据处理
@@ -198,15 +198,16 @@
         """
         if variable == '' or variable is None:
             return
         if isinstance(variable, str) and variable.find(".json",len(variable)-5) != -1:
             _path = path.join(TEST_DATA_PATH, variable, )
             with open(_path, "r") as json_file:
                 variable = json.load(json_file)
-        data = req_expr(content=variable, data=cls.response_dict, _replace=_replace)
+        # data = req_expr(content=variable, data=cls.response_dict, _replace=_replace)
+        data = DataProcess.handle_data_fromat(_template=variable, data=cls.response_dict, _replace=_replace)
         if jsonformat:
             variable = convert_json(data)
         else:
             variable = data
         return variable
 
     @classmethod
```

### Comparing `auto-test-common-2.0.8/common/data/faker_handle.py` & `auto-test-common-2.0.9/common/data/faker_handle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/data/handle_common.py` & `auto-test-common-2.0.9/common/data/handle_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,15 +291,14 @@
             else:
                 _new[key] = _json.get(key)
     return _new
 
 def convert_json_bank(content, data):
     _str = req_expr(content=content, data=data, _no_content=0)
     _str = _str.replace(Constant.DATA_NO_CONTENT + ",", '"' + Constant.DATA_NO_CONTENT + '",')
-    #_json = json.loads(_str)
     from common.data.data_process import DataProcess
     _json = DataProcess.handle_data(_str)
     if _json is None:
         return None
     else:
         return json.dumps(convert_json_dict(_json), ensure_ascii=False)
```

### Comparing `auto-test-common-2.0.8/common/data/template_data.py` & `auto-test-common-2.0.9/common/data/template_data.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/db/handle_db.py` & `auto-test-common-2.0.9/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/db/handle_db_batch.py` & `auto-test-common-2.0.9/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/db/handle_mongo.py` & `auto-test-common-2.0.9/common/db/handle_mongo.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/db/handle_mysqldb.py` & `auto-test-common-2.0.9/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/db/handle_oracle.py` & `auto-test-common-2.0.9/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/db/handle_sqlserver.py` & `auto-test-common-2.0.9/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/driver/ui_page.py` & `auto-test-common-2.0.9/common/driver/ui_page.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/file/ReadFile.py` & `auto-test-common-2.0.9/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/file/handle_excel.py` & `auto-test-common-2.0.9/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/file/handle_file.py` & `auto-test-common-2.0.9/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/file/handle_reques.py` & `auto-test-common-2.0.9/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/file/handle_system.py` & `auto-test-common-2.0.9/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/file/handle_yaml.py` & `auto-test-common-2.0.9/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/mq/handle_rabbit.py` & `auto-test-common-2.0.9/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/plat/ATF_platform.py` & `auto-test-common-2.0.9/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/plat/jenkin_platform.py` & `auto-test-common-2.0.9/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/plat/jira_platform.py` & `auto-test-common-2.0.9/common/plat/jira_platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,13 +172,37 @@
             return content
         except Exception as e:
             logger.info(f'添加测试用例到测试计划异常：{jql}')
             return content
 
     @classmethod
     def saveCaseToTestPlanByJql(self, testPlanIssueKey, jql):
+        logger.info(f'JQL:' + jql + ' KEY:' + testPlanIssueKey)
         content = JiraPlatForm.getDataByJql(jql,["id", "key"])
         keys = jsonpath(content, "$.issues[*].key")
         logger.info(f'添加用例列表：'+str(keys))
         JiraPlatForm.saveCaseToTestPlan(testPlanIssueKey, keys)
         logger.info(f'提交到测试计划：' + str(testPlanIssueKey)+'成功')
 
+
+
+if __name__ == '__main__':
+    content = list()
+    jql ='project = DB22100 AND issuetype = 测试用例 AND description ~ http AND 用例执行方式 = 自动化 AND text ~ "新版" ORDER BY priority DESC, updated DESC'
+    fields = ["id", "key"]
+    try:
+        content = APIDriver.http_request(
+            url=f"{Constant.JIRA_URL}/rest/api/2/search",
+            method='post',
+            parametric_key='json',
+            data={
+                "jql": jql,
+                "startAt": 0,
+                "maxResults": 1000,
+                "fields": fields
+            },
+            _auth=HTTPBasicAuth('oushiqiang','Xiaoshu406@@')
+        )
+        content = json.loads(content.content)
+        print(content)
+    except Exception as e:
+        logger.info(f'查询Jql异常：{jql}')
```

### Comparing `auto-test-common-2.0.8/common/plat/mysql_platform.py` & `auto-test-common-2.0.9/common/plat/mysql_platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,10 +150,12 @@
 
 
 
 
 
 
 
+if __name__ == '__main__':
+    print(MysqlPlatForm.get_test_autotest_run('DO23142-1786','31137'))
```

### Comparing `auto-test-common-2.0.8/common/plat/service_platform.py` & `auto-test-common-2.0.9/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/plugin/allure_plugin.py` & `auto-test-common-2.0.9/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/plugin/assert_plugin.py` & `auto-test-common-2.0.9/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/plugin/atf_plugin.py` & `auto-test-common-2.0.9/common/plugin/atf_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/plugin/data_bus.py` & `auto-test-common-2.0.9/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/plugin/data_plugin.py` & `auto-test-common-2.0.9/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/plugin/file_plugin.py` & `auto-test-common-2.0.9/common/plugin/file_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/plugin/hooks_plugin.py` & `auto-test-common-2.0.9/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/plugin/pytest_playwright.py` & `auto-test-common-2.0.9/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/plugin/pytest_plugin.py` & `auto-test-common-2.0.9/common/plugin/pytest_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,24 +25,35 @@
 
     @classmethod
     def getCaseNameList(self):
         """
         获取用例列表
         """
         case_name_list = []
-        if DataProcess.isNotNull(get_system_key('Result')):
-            case_name_list = ATFPlatForm.getCycleByResult(get_system_key('Result'))
+        count = 5
+        temp = 1
+        while temp <= count:
+            if DataProcess.isNotNull(get_system_key('Result')):
+                case_name_list = ATFPlatForm.getCycleByResult(get_system_key('Result'))
+            else:
+                case_name_list = ATFPlatForm.getCycleByResult()
+            if DataProcess.isNotNull(case_name_list):
+                temp = 10
+            else:
+                temp = temp + 1
+        if DataProcess.isNotNull(case_name_list):
+            PytestPlugin.initRunCyleCase()
+            case_name_list_str = ""
+            for temp in case_name_list:
+                case_name_list_str = case_name_list_str+ temp['casename']+";"
+            logger.info("获取需要执行的测试用例:"+case_name_list_str)
+            return case_name_list
         else:
-            case_name_list = ATFPlatForm.getCycleByResult()
-        PytestPlugin.initRunCyleCase()
-        case_name_list_str =""
-        for temp in case_name_list:
-            case_name_list_str = case_name_list_str+ temp['casename']+";"
-        logger.info("获取需要执行的测试用例:"+case_name_list_str)
-        return case_name_list
+            logger.warning("无测试用例列表可运行")
+            return case_name_list
 
 
 
     @classmethod
     def insertCaseToPlan(self):
         if DataProcess.isNotNull(get_system_key('addCaseJql')) and DataProcess.isNotNull(get_system_key(Constant.ISSUE_KEY)):
             JiraPlatForm.saveCaseToTestPlanByJql(get_system_key('issueKey'),get_system_key('addCaseJql'))
```

### Comparing `auto-test-common-2.0.8/common/plugin/template_plugin.py` & `auto-test-common-2.0.9/common/plugin/template_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/common/plugin/yaml_plugin.py` & `auto-test-common-2.0.9/common/plugin/yaml_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.8/setup.py` & `auto-test-common-2.0.9/setup.py`

 * *Files identical despite different names*


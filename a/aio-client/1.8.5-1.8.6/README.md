# Comparing `tmp/aio-client-1.8.5.tar.gz` & `tmp/aio-client-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio-client-1.8.5.tar", last modified: Thu Dec 28 14:29:50 2023, max compression
+gzip compressed data, was "aio-client-1.8.6.tar", last modified: Mon May 20 03:51:56 2024, max compression
```

## Comparing `aio-client-1.8.5.tar` & `aio-client-1.8.6.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.539246 aio-client-1.8.5/
--rw-r--r--   0 toor      (1000) toor      (1000)     7644 2023-12-28 14:29:42.000000 aio-client-1.8.5/CHANGELOG.md
--rw-r--r--   0 toor      (1000) toor      (1000)       95 2023-10-05 11:21:10.000000 aio-client-1.8.5/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     8278 2023-12-28 14:29:50.539246 aio-client-1.8.5/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      259 2023-10-05 11:21:10.000000 aio-client-1.8.5/README.md
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.417246 aio-client-1.8.5/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       77 2022-09-12 14:11:27.000000 aio-client-1.8.5/requirements/base.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-12-28 14:29:50.539246 aio-client-1.8.5/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2104 2023-10-05 11:21:10.000000 aio-client-1.8.5/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.413246 aio-client-1.8.5/src/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.422246 aio-client-1.8.5/src/aio_client/
--rw-r--r--   0 toor      (1000) toor      (1000)       73 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4254 2023-10-05 11:21:09.000000 aio-client-1.8.5/src/aio_client/admin.py
--rw-r--r--   0 toor      (1000) toor      (1000)      292 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/apps.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.429246 aio-client-1.8.5/src/aio_client/base/
--rw-r--r--   0 toor      (1000) toor      (1000)      157 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/base/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.436246 aio-client-1.8.5/src/aio_client/base/client/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/base/client/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3202 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/base/client/sender.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.438246 aio-client-1.8.5/src/aio_client/base/client/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/base/client/tests/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3377 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/base/client/tests/tests_sender.py
--rw-r--r--   0 toor      (1000) toor      (1000)      420 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/base/const.py
--rw-r--r--   0 toor      (1000) toor      (1000)      925 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/base/exceptions.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6679 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/base/helpers.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.445246 aio-client-1.8.5/src/aio_client/base/models/
--rw-r--r--   0 toor      (1000) toor      (1000)      213 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/base/models/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      884 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/base/models/base.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4020 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/base/models/enum.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3065 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/base/models/log.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2350 2023-09-04 08:10:06.000000 aio-client-1.8.5/src/aio_client/base/models/message.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.452246 aio-client-1.8.5/src/aio_client/base/models/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/base/models/tests/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      175 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/base/models/tests/factory_log.py
--rw-r--r--   0 toor      (1000) toor      (1000)      279 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/base/models/tests/factory_message.py
--rw-r--r--   0 toor      (1000) toor      (1000)      725 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/base/models/tests/utils.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1337 2023-12-28 14:29:42.000000 aio-client-1.8.5/src/aio_client/base/signals.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4590 2023-09-04 08:10:06.000000 aio-client-1.8.5/src/aio_client/base/tasks.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.453246 aio-client-1.8.5/src/aio_client/common/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/common/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.459246 aio-client-1.8.5/src/aio_client/common/configuration/
--rw-r--r--   0 toor      (1000) toor      (1000)     4443 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/common/configuration/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1689 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/common/configuration/configuration.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4295 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/configs.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.468246 aio-client-1.8.5/src/aio_client/consumer/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/consumer/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2870 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/consumer/api.py
--rw-r--r--   0 toor      (1000) toor      (1000)      177 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/consumer/const.py
--rw-r--r--   0 toor      (1000) toor      (1000)      536 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/consumer/exceptions.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3950 2023-09-04 08:10:06.000000 aio-client-1.8.5/src/aio_client/consumer/helpers.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.473246 aio-client-1.8.5/src/aio_client/consumer/models/
--rw-r--r--   0 toor      (1000) toor      (1000)      141 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/consumer/models/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4185 2023-09-04 08:10:06.000000 aio-client-1.8.5/src/aio_client/consumer/models/consumer.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.475246 aio-client-1.8.5/src/aio_client/consumer/models/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/consumer/models/tests/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      234 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/consumer/models/tests/factory_consumer.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5127 2023-09-04 08:10:06.000000 aio-client-1.8.5/src/aio_client/consumer/tasks.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.485246 aio-client-1.8.5/src/aio_client/consumer/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)      275 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/consumer/tests/GetConsumerReceipt.json
--rw-r--r--   0 toor      (1000) toor      (1000)      641 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/consumer/tests/GetConsumerRequest.json
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/consumer/tests/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      794 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/consumer/tests/request_data.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5208 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/consumer/tests/tests_api.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5091 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/consumer/tests/tests_helpers.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.512246 aio-client-1.8.5/src/aio_client/migrations/
--rw-r--r--   0 toor      (1000) toor      (1000)    16299 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/migrations/0001_initial.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6222 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/migrations/0002_auto_20181026_1115.py
--rw-r--r--   0 toor      (1000) toor      (1000)      591 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/migrations/0003_auto_20190201_0530.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6412 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/migrations/0004_auto_20200703_1536.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6239 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/migrations/0005_auto_20200703_1550.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1282 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/migrations/0006_auto_20201109_0917.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6700 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/migrations/0007_auto_20201113_2248.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2604 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/migrations/0008_auto_20201209_1503.py
--rw-r--r--   0 toor      (1000) toor      (1000)      557 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/migrations/0009_auto_20201210_1609.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2079 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/migrations/0010_auto_20210416_1519.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4137 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/migrations/0011_auto_20210416_1747.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1937 2023-09-04 08:10:06.000000 aio-client-1.8.5/src/aio_client/migrations/0012_aio_client.py
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/migrations/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.516246 aio-client-1.8.5/src/aio_client/provider/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/provider/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2968 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/provider/api.py
--rw-r--r--   0 toor      (1000) toor      (1000)      714 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/provider/exceptions.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3345 2023-09-04 08:10:06.000000 aio-client-1.8.5/src/aio_client/provider/helpers.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.523246 aio-client-1.8.5/src/aio_client/provider/models/
--rw-r--r--   0 toor      (1000) toor      (1000)      218 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/provider/models/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5412 2023-09-04 08:10:06.000000 aio-client-1.8.5/src/aio_client/provider/models/provider.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.531246 aio-client-1.8.5/src/aio_client/provider/models/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/provider/models/tests/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      514 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/provider/models/tests/factory_provider.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5180 2023-09-04 08:10:06.000000 aio-client-1.8.5/src/aio_client/provider/tasks.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.538246 aio-client-1.8.5/src/aio_client/provider/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)      212 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/provider/tests/GetProviderReceipt.json
--rw-r--r--   0 toor      (1000) toor      (1000)     1390 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/provider/tests/GetProviderRequest.json
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/provider/tests/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      684 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/provider/tests/request_data.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6110 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/provider/tests/tests_api.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4477 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/provider/tests/tests_helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1312 2022-09-12 14:11:27.000000 aio-client-1.8.5/src/aio_client/utils.py
--rw-r--r--   0 toor      (1000) toor      (1000)      448 2023-12-28 14:29:50.000000 aio-client-1.8.5/src/aio_client/version.conf
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-12-28 14:29:50.425246 aio-client-1.8.5/src/aio_client.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     8278 2023-12-28 14:29:50.000000 aio-client-1.8.5/src/aio_client.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     3292 2023-12-28 14:29:50.000000 aio-client-1.8.5/src/aio_client.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       43 2023-12-28 14:29:50.000000 aio-client-1.8.5/src/aio_client.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2022-09-12 14:11:40.000000 aio-client-1.8.5/src/aio_client.egg-info/not-zip-safe
--rw-r--r--   0 toor      (1000) toor      (1000)       77 2023-12-28 14:29:50.000000 aio-client-1.8.5/src/aio_client.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       11 2023-12-28 14:29:50.000000 aio-client-1.8.5/src/aio_client.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.669095 aio-client-1.8.6/
+-rw-r--r--   0 toor      (1000) toor      (1000)     7830 2024-05-20 03:51:51.000000 aio-client-1.8.6/CHANGELOG.md
+-rw-r--r--   0 toor      (1000) toor      (1000)       95 2023-10-05 11:21:10.000000 aio-client-1.8.6/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     8464 2024-05-20 03:51:56.668095 aio-client-1.8.6/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      259 2023-10-05 11:21:10.000000 aio-client-1.8.6/README.md
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.575096 aio-client-1.8.6/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)       77 2022-09-12 14:11:27.000000 aio-client-1.8.6/requirements/base.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2024-05-20 03:51:56.669095 aio-client-1.8.6/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2104 2023-10-05 11:21:10.000000 aio-client-1.8.6/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.571095 aio-client-1.8.6/src/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.585096 aio-client-1.8.6/src/aio_client/
+-rw-r--r--   0 toor      (1000) toor      (1000)       73 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4254 2023-10-05 11:21:09.000000 aio-client-1.8.6/src/aio_client/admin.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      292 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/apps.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.593095 aio-client-1.8.6/src/aio_client/base/
+-rw-r--r--   0 toor      (1000) toor      (1000)      157 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/base/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.595095 aio-client-1.8.6/src/aio_client/base/client/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/base/client/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3202 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/base/client/sender.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.598096 aio-client-1.8.6/src/aio_client/base/client/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/base/client/tests/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3377 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/base/client/tests/tests_sender.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      420 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/base/const.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      925 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/base/exceptions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6679 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/base/helpers.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.604095 aio-client-1.8.6/src/aio_client/base/models/
+-rw-r--r--   0 toor      (1000) toor      (1000)      213 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/base/models/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      884 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/base/models/base.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4020 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/base/models/enum.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3065 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/base/models/log.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2350 2023-09-04 08:10:06.000000 aio-client-1.8.6/src/aio_client/base/models/message.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.609095 aio-client-1.8.6/src/aio_client/base/models/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/base/models/tests/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      175 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/base/models/tests/factory_log.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      279 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/base/models/tests/factory_message.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      725 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/base/models/tests/utils.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1337 2023-12-28 14:29:42.000000 aio-client-1.8.6/src/aio_client/base/signals.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4590 2023-09-04 08:10:06.000000 aio-client-1.8.6/src/aio_client/base/tasks.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.610095 aio-client-1.8.6/src/aio_client/common/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/common/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.612095 aio-client-1.8.6/src/aio_client/common/configuration/
+-rw-r--r--   0 toor      (1000) toor      (1000)     4443 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/common/configuration/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1689 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/common/configuration/configuration.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4295 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/configs.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.617095 aio-client-1.8.6/src/aio_client/consumer/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/consumer/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2870 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/consumer/api.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      177 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/consumer/const.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      536 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/consumer/exceptions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3950 2023-09-04 08:10:06.000000 aio-client-1.8.6/src/aio_client/consumer/helpers.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.619095 aio-client-1.8.6/src/aio_client/consumer/models/
+-rw-r--r--   0 toor      (1000) toor      (1000)      141 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/consumer/models/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4185 2023-09-04 08:10:06.000000 aio-client-1.8.6/src/aio_client/consumer/models/consumer.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.621096 aio-client-1.8.6/src/aio_client/consumer/models/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/consumer/models/tests/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      234 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/consumer/models/tests/factory_consumer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5127 2023-09-04 08:10:06.000000 aio-client-1.8.6/src/aio_client/consumer/tasks.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.632095 aio-client-1.8.6/src/aio_client/consumer/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)      275 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/consumer/tests/GetConsumerReceipt.json
+-rw-r--r--   0 toor      (1000) toor      (1000)      641 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/consumer/tests/GetConsumerRequest.json
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/consumer/tests/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      794 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/consumer/tests/request_data.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5208 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/consumer/tests/tests_api.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5091 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/consumer/tests/tests_helpers.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.654096 aio-client-1.8.6/src/aio_client/migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)    16299 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6222 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/migrations/0002_auto_20181026_1115.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      591 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/migrations/0003_auto_20190201_0530.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6412 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/migrations/0004_auto_20200703_1536.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6239 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/migrations/0005_auto_20200703_1550.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1282 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/migrations/0006_auto_20201109_0917.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6700 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/migrations/0007_auto_20201113_2248.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2604 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/migrations/0008_auto_20201209_1503.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      557 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/migrations/0009_auto_20201210_1609.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2079 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/migrations/0010_auto_20210416_1519.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4137 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/migrations/0011_auto_20210416_1747.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1937 2023-09-04 08:10:06.000000 aio-client-1.8.6/src/aio_client/migrations/0012_aio_client.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/migrations/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.657096 aio-client-1.8.6/src/aio_client/provider/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/provider/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2968 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/provider/api.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      714 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/provider/exceptions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3290 2024-05-20 03:51:51.000000 aio-client-1.8.6/src/aio_client/provider/helpers.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.659095 aio-client-1.8.6/src/aio_client/provider/models/
+-rw-r--r--   0 toor      (1000) toor      (1000)      218 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/provider/models/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5412 2023-09-04 08:10:06.000000 aio-client-1.8.6/src/aio_client/provider/models/provider.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.661095 aio-client-1.8.6/src/aio_client/provider/models/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/provider/models/tests/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      514 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/provider/models/tests/factory_provider.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5180 2023-09-04 08:10:06.000000 aio-client-1.8.6/src/aio_client/provider/tasks.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.667096 aio-client-1.8.6/src/aio_client/provider/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)      212 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/provider/tests/GetProviderReceipt.json
+-rw-r--r--   0 toor      (1000) toor      (1000)     1390 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/provider/tests/GetProviderRequest.json
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/provider/tests/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      684 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/provider/tests/request_data.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6110 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/provider/tests/tests_api.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4477 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/provider/tests/tests_helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1312 2022-09-12 14:11:27.000000 aio-client-1.8.6/src/aio_client/utils.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      450 2024-05-20 03:51:56.000000 aio-client-1.8.6/src/aio_client/version.conf
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-20 03:51:56.667096 aio-client-1.8.6/src/aio_client.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     8464 2024-05-20 03:51:56.000000 aio-client-1.8.6/src/aio_client.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     3292 2024-05-20 03:51:56.000000 aio-client-1.8.6/src/aio_client.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       43 2024-05-20 03:51:56.000000 aio-client-1.8.6/src/aio_client.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2022-09-12 14:11:40.000000 aio-client-1.8.6/src/aio_client.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)       77 2024-05-20 03:51:56.000000 aio-client-1.8.6/src/aio_client.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       11 2024-05-20 03:51:56.000000 aio-client-1.8.6/src/aio_client.egg-info/top_level.txt
```

### Comparing `aio-client-1.8.5/CHANGELOG.md` & `aio-client-1.8.6/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 История изменений
 -----------------
+1.8.6 (2024-04-09)
+++++++++++++++++++
+- (EDUSCHL-21702) Удален вывод в sentry ошибки сохранения GetProviderReceipt
+  и GetProviderRequest
+
+-----------------
 1.8.5 (2023-12-28)
 ++++++++++++++++++
 - (EDUCLLG-8117) Изменен пример aio-сервера в примере конфига и 
   добавлена отправка сигнала через robust_sender, если включен режим отладки
 
 1.8.4 (2023-10-05)
 ++++++++++++++++++
```

### Comparing `aio-client-1.8.5/PKG-INFO` & `aio-client-1.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-client
-Version: 1.8.5
+Version: 1.8.6
 Summary: AIO-клиент
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 Keywords: django СМЭВ3
 Description-Content-Type: text/markdown
 Requires-Dist: six
 Requires-Dist: requests<2.26,>=2.4.2
@@ -14,14 +14,20 @@
 Requires-Dist: m3-builder<2,>=1.2
 
 # AIO-client
 
 Пакет ``aio-client`` предназначен для простой и быстрой интеграции
 пользовательского Django-проекта с подсистемой взаимодействия со СМЭВ 3(AIO).История изменений
 -----------------
+1.8.6 (2024-04-09)
+++++++++++++++++++
+- (EDUSCHL-21702) Удален вывод в sentry ошибки сохранения GetProviderReceipt
+  и GetProviderRequest
+
+-----------------
 1.8.5 (2023-12-28)
 ++++++++++++++++++
 - (EDUCLLG-8117) Изменен пример aio-сервера в примере конфига и 
   добавлена отправка сигнала через robust_sender, если включен режим отладки
 
 1.8.4 (2023-10-05)
 ++++++++++++++++++
```

### Comparing `aio-client-1.8.5/setup.py` & `aio-client-1.8.6/setup.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/admin.py` & `aio-client-1.8.6/src/aio_client/admin.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/base/client/sender.py` & `aio-client-1.8.6/src/aio_client/base/client/sender.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/base/client/tests/tests_sender.py` & `aio-client-1.8.6/src/aio_client/base/client/tests/tests_sender.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/base/exceptions.py` & `aio-client-1.8.6/src/aio_client/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/base/helpers.py` & `aio-client-1.8.6/src/aio_client/base/helpers.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/base/models/base.py` & `aio-client-1.8.6/src/aio_client/base/models/base.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/base/models/enum.py` & `aio-client-1.8.6/src/aio_client/base/models/enum.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/base/models/log.py` & `aio-client-1.8.6/src/aio_client/base/models/log.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/base/models/message.py` & `aio-client-1.8.6/src/aio_client/base/models/message.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/base/models/tests/utils.py` & `aio-client-1.8.6/src/aio_client/base/models/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/base/signals.py` & `aio-client-1.8.6/src/aio_client/base/signals.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/base/tasks.py` & `aio-client-1.8.6/src/aio_client/base/tasks.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/common/configuration/__init__.py` & `aio-client-1.8.6/src/aio_client/common/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/common/configuration/configuration.py` & `aio-client-1.8.6/src/aio_client/common/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/configs.py` & `aio-client-1.8.6/src/aio_client/configs.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/consumer/api.py` & `aio-client-1.8.6/src/aio_client/consumer/api.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/consumer/exceptions.py` & `aio-client-1.8.6/src/aio_client/consumer/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/consumer/helpers.py` & `aio-client-1.8.6/src/aio_client/consumer/helpers.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/consumer/models/consumer.py` & `aio-client-1.8.6/src/aio_client/consumer/models/consumer.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/consumer/tasks.py` & `aio-client-1.8.6/src/aio_client/consumer/tasks.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/consumer/tests/GetConsumerRequest.json` & `aio-client-1.8.6/src/aio_client/consumer/tests/GetConsumerRequest.json`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/consumer/tests/request_data.py` & `aio-client-1.8.6/src/aio_client/consumer/tests/request_data.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/consumer/tests/tests_api.py` & `aio-client-1.8.6/src/aio_client/consumer/tests/tests_api.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/consumer/tests/tests_helpers.py` & `aio-client-1.8.6/src/aio_client/consumer/tests/tests_helpers.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/migrations/0001_initial.py` & `aio-client-1.8.6/src/aio_client/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/migrations/0002_auto_20181026_1115.py` & `aio-client-1.8.6/src/aio_client/migrations/0002_auto_20181026_1115.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/migrations/0003_auto_20190201_0530.py` & `aio-client-1.8.6/src/aio_client/migrations/0003_auto_20190201_0530.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/migrations/0004_auto_20200703_1536.py` & `aio-client-1.8.6/src/aio_client/migrations/0004_auto_20200703_1536.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/migrations/0005_auto_20200703_1550.py` & `aio-client-1.8.6/src/aio_client/migrations/0005_auto_20200703_1550.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/migrations/0006_auto_20201109_0917.py` & `aio-client-1.8.6/src/aio_client/migrations/0006_auto_20201109_0917.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/migrations/0007_auto_20201113_2248.py` & `aio-client-1.8.6/src/aio_client/migrations/0007_auto_20201113_2248.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/migrations/0008_auto_20201209_1503.py` & `aio-client-1.8.6/src/aio_client/migrations/0008_auto_20201209_1503.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/migrations/0009_auto_20201210_1609.py` & `aio-client-1.8.6/src/aio_client/migrations/0009_auto_20201210_1609.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/migrations/0010_auto_20210416_1519.py` & `aio-client-1.8.6/src/aio_client/migrations/0010_auto_20210416_1519.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/migrations/0011_auto_20210416_1747.py` & `aio-client-1.8.6/src/aio_client/migrations/0011_auto_20210416_1747.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/migrations/0012_aio_client.py` & `aio-client-1.8.6/src/aio_client/migrations/0012_aio_client.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/provider/api.py` & `aio-client-1.8.6/src/aio_client/provider/api.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/provider/exceptions.py` & `aio-client-1.8.6/src/aio_client/provider/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/provider/helpers.py` & `aio-client-1.8.6/src/aio_client/provider/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,18 @@
 
     response = send_request(request_log)
     for message in response.json():
         message['request_id'] = request_log
 
         try:
             GetProviderRequest.objects.create(**message)
-        except IntegrityError:
+        except IntegrityError as err:
             error_message = (
                 f'Не удалось создать сообщение GetProviderRequest'
-                f'({message["message_id"]}:{message["origin_message_id"]})')
-            capture_message(error_message)
+                f'({message["message_id"]}:{message["origin_message_id"]})  - {err}')
             if values:
                 values[title] = error_message
         else:
             is_send_signal = True
 
     return response.json(), is_send_signal
 
@@ -82,18 +81,17 @@
 
     response = send_request(request_log)
     for message in response.json():
         message['request_id'] = request_log
 
         try:
             GetProviderReceipt.objects.create(**message)
-        except IntegrityError:
+        except IntegrityError as err:
             error_message = (
                 f'Не удалось создать сообщение GetProviderReceipt'
-                f'({message["message_id"]}:{message["origin_message_id"]})')
-            capture_message(error_message)
+                f'({message["message_id"]}:{message["origin_message_id"]}) - {err}')
             if values:
                 values[title] = error_message
         else:
             is_send_signal = True
 
     return response.json(), is_send_signal
```

### Comparing `aio-client-1.8.5/src/aio_client/provider/models/provider.py` & `aio-client-1.8.6/src/aio_client/provider/models/provider.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/provider/models/tests/factory_provider.py` & `aio-client-1.8.6/src/aio_client/provider/models/tests/factory_provider.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/provider/tasks.py` & `aio-client-1.8.6/src/aio_client/provider/tasks.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/provider/tests/GetProviderRequest.json` & `aio-client-1.8.6/src/aio_client/provider/tests/GetProviderRequest.json`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/provider/tests/request_data.py` & `aio-client-1.8.6/src/aio_client/provider/tests/request_data.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/provider/tests/tests_api.py` & `aio-client-1.8.6/src/aio_client/provider/tests/tests_api.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/provider/tests/tests_helpers.py` & `aio-client-1.8.6/src/aio_client/provider/tests/tests_helpers.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client/utils.py` & `aio-client-1.8.6/src/aio_client/utils.py`

 * *Files identical despite different names*

### Comparing `aio-client-1.8.5/src/aio_client.egg-info/PKG-INFO` & `aio-client-1.8.6/src/aio_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-client
-Version: 1.8.5
+Version: 1.8.6
 Summary: AIO-клиент
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 Keywords: django СМЭВ3
 Description-Content-Type: text/markdown
 Requires-Dist: six
 Requires-Dist: requests<2.26,>=2.4.2
@@ -14,14 +14,20 @@
 Requires-Dist: m3-builder<2,>=1.2
 
 # AIO-client
 
 Пакет ``aio-client`` предназначен для простой и быстрой интеграции
 пользовательского Django-проекта с подсистемой взаимодействия со СМЭВ 3(AIO).История изменений
 -----------------
+1.8.6 (2024-04-09)
+++++++++++++++++++
+- (EDUSCHL-21702) Удален вывод в sentry ошибки сохранения GetProviderReceipt
+  и GetProviderRequest
+
+-----------------
 1.8.5 (2023-12-28)
 ++++++++++++++++++
 - (EDUCLLG-8117) Изменен пример aio-сервера в примере конфига и 
   добавлена отправка сигнала через robust_sender, если включен режим отладки
 
 1.8.4 (2023-10-05)
 ++++++++++++++++++
```

### Comparing `aio-client-1.8.5/src/aio_client.egg-info/SOURCES.txt` & `aio-client-1.8.6/src/aio_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*


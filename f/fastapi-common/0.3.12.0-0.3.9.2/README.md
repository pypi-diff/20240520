# Comparing `tmp/fastapi-common-0.3.12.0.tar.gz` & `tmp/fastapi-common-0.3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-common-0.3.12.0.tar", last modified: Fri Jan 20 23:06:51 2023, max compression
+gzip compressed data, was "fastapi-common-0.3.9.2.tar", last modified: Tue Sep 27 21:12:34 2022, max compression
```

## Comparing `fastapi-common-0.3.12.0.tar` & `fastapi-common-0.3.9.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2023-01-20 23:06:51.247594 fastapi-common-0.3.12.0/
--rw-r--r--   0 alfredo    (501) staff       (20)    35149 2022-05-07 23:57:17.000000 fastapi-common-0.3.12.0/LICENSE
--rw-r--r--   0 alfredo    (501) staff       (20)      353 2023-01-20 23:06:51.247468 fastapi-common-0.3.12.0/PKG-INFO
--rw-r--r--   0 alfredo    (501) staff       (20)     8622 2022-05-24 04:11:10.000000 fastapi-common-0.3.12.0/README.md
-drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2023-01-20 23:06:51.236598 fastapi-common-0.3.12.0/common/
--rw-r--r--   0 alfredo    (501) staff       (20)       56 2022-02-21 23:23:57.000000 fastapi-common-0.3.12.0/common/__init__.py
-drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2023-01-20 23:06:51.236731 fastapi-common-0.3.12.0/common/fastapi/
--rw-r--r--   0 alfredo    (501) staff       (20)       25 2023-01-20 23:06:46.000000 fastapi-common-0.3.12.0/common/fastapi/__init__.py
-drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2023-01-20 23:06:51.236968 fastapi-common-0.3.12.0/common/fastapi/aws/
--rw-r--r--   0 alfredo    (501) staff       (20)        0 2022-05-08 00:15:04.000000 fastapi-common-0.3.12.0/common/fastapi/aws/__init__.py
--rw-r--r--   0 alfredo    (501) staff       (20)     1253 2022-07-21 09:24:21.000000 fastapi-common-0.3.12.0/common/fastapi/aws/manager.py
-drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2023-01-20 23:06:51.237225 fastapi-common-0.3.12.0/common/fastapi/core/
--rw-r--r--   0 alfredo    (501) staff       (20)        0 2022-03-07 23:52:58.000000 fastapi-common-0.3.12.0/common/fastapi/core/__init__.py
-drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2023-01-20 23:06:51.237593 fastapi-common-0.3.12.0/common/fastapi/core/app/
--rw-r--r--   0 alfredo    (501) staff       (20)       42 2022-03-08 01:01:29.000000 fastapi-common-0.3.12.0/common/fastapi/core/app/__init__.py
--rw-r--r--   0 alfredo    (501) staff       (20)      654 2022-03-15 23:31:25.000000 fastapi-common-0.3.12.0/common/fastapi/core/app/app.py
-drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2023-01-20 23:06:51.238689 fastapi-common-0.3.12.0/common/fastapi/core/commands/
--rw-r--r--   0 alfredo    (501) staff       (20)      201 2022-03-08 03:23:19.000000 fastapi-common-0.3.12.0/common/fastapi/core/commands/__init__.py
--rw-r--r--   0 alfredo    (501) staff       (20)      394 2022-03-08 03:18:24.000000 fastapi-common-0.3.12.0/common/fastapi/core/commands/command.py
--rw-r--r--   0 alfredo    (501) staff       (20)     1577 2022-05-08 01:15:19.000000 fastapi-common-0.3.12.0/common/fastapi/core/commands/load_data.py
--rw-r--r--   0 alfredo    (501) staff       (20)      605 2022-03-13 05:21:09.000000 fastapi-common-0.3.12.0/common/fastapi/core/commands/make_migrations.py
--rw-r--r--   0 alfredo    (501) staff       (20)      418 2022-03-11 08:11:55.000000 fastapi-common-0.3.12.0/common/fastapi/core/commands/pytest_cmd.py
--rw-r--r--   0 alfredo    (501) staff       (20)      399 2022-07-04 18:01:48.000000 fastapi-common-0.3.12.0/common/fastapi/core/commands/runserver.py
-drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2023-01-20 23:06:51.239265 fastapi-common-0.3.12.0/common/fastapi/core/parameters/
--rw-r--r--   0 alfredo    (501) staff       (20)      142 2022-03-11 06:23:47.000000 fastapi-common-0.3.12.0/common/fastapi/core/parameters/__init__.py
-drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2023-01-20 23:06:51.240393 fastapi-common-0.3.12.0/common/fastapi/core/parameters/managers/
--rw-r--r--   0 alfredo    (501) staff       (20)      243 2022-03-08 02:32:49.000000 fastapi-common-0.3.12.0/common/fastapi/core/parameters/managers/__init__.py
--rw-r--r--   0 alfredo    (501) staff       (20)     4132 2022-10-26 19:04:54.000000 fastapi-common-0.3.12.0/common/fastapi/core/parameters/managers/base_manager.py
--rw-r--r--   0 alfredo    (501) staff       (20)     1980 2022-03-11 07:10:59.000000 fastapi-common-0.3.12.0/common/fastapi/core/parameters/managers/command_manager.py
--rw-r--r--   0 alfredo    (501) staff       (20)      225 2022-03-08 02:32:49.000000 fastapi-common-0.3.12.0/common/fastapi/core/parameters/managers/flag_manager.py
--rw-r--r--   0 alfredo    (501) staff       (20)     1562 2022-10-29 04:35:39.000000 fastapi-common-0.3.12.0/common/fastapi/core/parameters/managers/manager_param.py
--rw-r--r--   0 alfredo    (501) staff       (20)      817 2022-10-26 19:06:19.000000 fastapi-common-0.3.12.0/common/fastapi/core/parameters/managers/variable_manager.py
--rw-r--r--   0 alfredo    (501) staff       (20)      267 2022-03-08 02:08:06.000000 fastapi-common-0.3.12.0/common/fastapi/core/parameters/param_cfg.py
--rw-r--r--   0 alfredo    (501) staff       (20)      724 2022-03-08 03:08:24.000000 fastapi-common-0.3.12.0/common/fastapi/core/parameters/parameter_manager.py
-drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2023-01-20 23:06:51.241842 fastapi-common-0.3.12.0/common/fastapi/db/
--rw-r--r--   0 alfredo    (501) staff       (20)      112 2022-05-08 00:41:36.000000 fastapi-common-0.3.12.0/common/fastapi/db/__init__.py
--rw-r--r--   0 alfredo    (501) staff       (20)     1736 2022-05-08 02:27:02.000000 fastapi-common-0.3.12.0/common/fastapi/db/connection.py
-drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2023-01-20 23:06:51.242982 fastapi-common-0.3.12.0/common/fastapi/db/dals/
--rw-r--r--   0 alfredo    (501) staff       (20)       41 2022-05-08 00:41:18.000000 fastapi-common-0.3.12.0/common/fastapi/db/dals/__init__.py
--rw-r--r--   0 alfredo    (501) staff       (20)     2904 2023-01-20 23:02:24.000000 fastapi-common-0.3.12.0/common/fastapi/db/dals/async_crud_dal.py
--rw-r--r--   0 alfredo    (501) staff       (20)      923 2023-01-20 22:57:01.000000 fastapi-common-0.3.12.0/common/fastapi/db/dals/base_dal.py
--rw-r--r--   0 alfredo    (501) staff       (20)     3592 2023-01-20 22:59:08.000000 fastapi-common-0.3.12.0/common/fastapi/db/dals/crud_dal.py
--rw-r--r--   0 alfredo    (501) staff       (20)      408 2022-05-24 04:43:22.000000 fastapi-common-0.3.12.0/common/fastapi/db/dals/dal_access.py
--rw-r--r--   0 alfredo    (501) staff       (20)      398 2022-03-13 04:42:42.000000 fastapi-common-0.3.12.0/common/fastapi/db/db_access.py
--rw-r--r--   0 alfredo    (501) staff       (20)      577 2022-05-16 19:37:44.000000 fastapi-common-0.3.12.0/common/fastapi/db/decorators.py
--rw-r--r--   0 alfredo    (501) staff       (20)     1924 2022-08-09 03:40:41.000000 fastapi-common-0.3.12.0/common/fastapi/db/test_db.py
--rw-r--r--   0 alfredo    (501) staff       (20)     3000 2022-08-07 22:52:01.000000 fastapi-common-0.3.12.0/common/fastapi/db/utils.py
-drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2023-01-20 23:06:51.243521 fastapi-common-0.3.12.0/common/fastapi/requests/
--rw-r--r--   0 alfredo    (501) staff       (20)      110 2022-02-21 23:24:00.000000 fastapi-common-0.3.12.0/common/fastapi/requests/__init__.py
--rw-r--r--   0 alfredo    (501) staff       (20)     3484 2022-03-11 08:36:34.000000 fastapi-common-0.3.12.0/common/fastapi/requests/base_manager.py
--rw-r--r--   0 alfredo    (501) staff       (20)      113 2022-03-09 04:31:33.000000 fastapi-common-0.3.12.0/common/fastapi/requests/response_type.py
-drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2023-01-20 23:06:51.244838 fastapi-common-0.3.12.0/common/fastapi/routing/
--rw-r--r--   0 alfredo    (501) staff       (20)      232 2022-03-17 23:41:31.000000 fastapi-common-0.3.12.0/common/fastapi/routing/__init__.py
--rw-r--r--   0 alfredo    (501) staff       (20)     2111 2022-12-04 23:36:43.000000 fastapi-common-0.3.12.0/common/fastapi/routing/base_crud_router.py
--rw-r--r--   0 alfredo    (501) staff       (20)     2976 2022-08-09 03:19:18.000000 fastapi-common-0.3.12.0/common/fastapi/routing/base_router.py
--rw-r--r--   0 alfredo    (501) staff       (20)      969 2022-03-22 19:36:25.000000 fastapi-common-0.3.12.0/common/fastapi/routing/enum.py
--rw-r--r--   0 alfredo    (501) staff       (20)      541 2022-02-21 23:04:40.000000 fastapi-common-0.3.12.0/common/fastapi/routing/generic_crud_router.py
--rw-r--r--   0 alfredo    (501) staff       (20)      324 2022-02-21 23:04:46.000000 fastapi-common-0.3.12.0/common/fastapi/routing/generic_router.py
--rw-r--r--   0 alfredo    (501) staff       (20)     1600 2022-02-17 22:39:07.000000 fastapi-common-0.3.12.0/common/fastapi/routing/utils.py
-drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2023-01-20 23:06:51.245582 fastapi-common-0.3.12.0/common/fastapi/schemas/
--rw-r--r--   0 alfredo    (501) staff       (20)      233 2022-08-09 07:43:31.000000 fastapi-common-0.3.12.0/common/fastapi/schemas/__init__.py
--rw-r--r--   0 alfredo    (501) staff       (20)      827 2022-04-05 00:51:47.000000 fastapi-common-0.3.12.0/common/fastapi/schemas/base_schema.py
--rw-r--r--   0 alfredo    (501) staff       (20)      677 2022-08-09 07:43:21.000000 fastapi-common-0.3.12.0/common/fastapi/schemas/http.py
--rw-r--r--   0 alfredo    (501) staff       (20)      480 2022-03-25 21:04:02.000000 fastapi-common-0.3.12.0/common/fastapi/schemas/request.py
-drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2023-01-20 23:06:51.246102 fastapi-common-0.3.12.0/common/fastapi/testing/
--rw-r--r--   0 alfredo    (501) staff       (20)       78 2022-03-11 07:06:46.000000 fastapi-common-0.3.12.0/common/fastapi/testing/__init__.py
--rw-r--r--   0 alfredo    (501) staff       (20)     2266 2022-05-08 02:03:43.000000 fastapi-common-0.3.12.0/common/fastapi/testing/decorators.py
--rw-r--r--   0 alfredo    (501) staff       (20)      778 2022-03-11 08:11:42.000000 fastapi-common-0.3.12.0/common/fastapi/testing/test_case.py
-drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2023-01-20 23:06:51.246551 fastapi-common-0.3.12.0/common/fastapi/utils/
--rw-r--r--   0 alfredo    (501) staff       (20)      132 2022-03-08 03:22:53.000000 fastapi-common-0.3.12.0/common/fastapi/utils/__init__.py
--rw-r--r--   0 alfredo    (501) staff       (20)      978 2022-03-09 20:32:03.000000 fastapi-common-0.3.12.0/common/fastapi/utils/functions.py
--rw-r--r--   0 alfredo    (501) staff       (20)      467 2022-03-08 02:05:35.000000 fastapi-common-0.3.12.0/common/fastapi/utils/singleton.py
-drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2023-01-20 23:06:51.247279 fastapi-common-0.3.12.0/fastapi_common.egg-info/
--rw-r--r--   0 alfredo    (501) staff       (20)      353 2023-01-20 23:06:51.000000 fastapi-common-0.3.12.0/fastapi_common.egg-info/PKG-INFO
--rw-r--r--   0 alfredo    (501) staff       (20)     2297 2023-01-20 23:06:51.000000 fastapi-common-0.3.12.0/fastapi_common.egg-info/SOURCES.txt
--rw-r--r--   0 alfredo    (501) staff       (20)        1 2023-01-20 23:06:51.000000 fastapi-common-0.3.12.0/fastapi_common.egg-info/dependency_links.txt
--rw-r--r--   0 alfredo    (501) staff       (20)        7 2023-01-20 23:06:51.000000 fastapi-common-0.3.12.0/fastapi_common.egg-info/namespace_packages.txt
--rw-r--r--   0 alfredo    (501) staff       (20)       58 2023-01-20 23:06:51.000000 fastapi-common-0.3.12.0/fastapi_common.egg-info/requires.txt
--rw-r--r--   0 alfredo    (501) staff       (20)        7 2023-01-20 23:06:51.000000 fastapi-common-0.3.12.0/fastapi_common.egg-info/top_level.txt
--rw-r--r--   0 alfredo    (501) staff       (20)       38 2023-01-20 23:06:51.247631 fastapi-common-0.3.12.0/setup.cfg
--rw-r--r--   0 alfredo    (501) staff       (20)      729 2022-09-27 21:13:37.000000 fastapi-common-0.3.12.0/setup.py
+drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2022-09-27 21:12:34.696722 fastapi-common-0.3.9.2/
+-rw-r--r--   0 alfredo    (501) staff       (20)    35149 2022-05-07 23:57:17.000000 fastapi-common-0.3.9.2/LICENSE
+-rw-r--r--   0 alfredo    (501) staff       (20)      380 2022-09-27 21:12:34.696575 fastapi-common-0.3.9.2/PKG-INFO
+-rw-r--r--   0 alfredo    (501) staff       (20)     8622 2022-05-24 04:11:10.000000 fastapi-common-0.3.9.2/README.md
+drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2022-09-27 21:12:34.686142 fastapi-common-0.3.9.2/common/
+-rw-r--r--   0 alfredo    (501) staff       (20)       56 2022-02-21 23:23:57.000000 fastapi-common-0.3.9.2/common/__init__.py
+drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2022-09-27 21:12:34.686261 fastapi-common-0.3.9.2/common/fastapi/
+-rw-r--r--   0 alfredo    (501) staff       (20)       24 2022-08-09 10:06:54.000000 fastapi-common-0.3.9.2/common/fastapi/__init__.py
+drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2022-09-27 21:12:34.686614 fastapi-common-0.3.9.2/common/fastapi/aws/
+-rw-r--r--   0 alfredo    (501) staff       (20)        0 2022-05-08 00:15:04.000000 fastapi-common-0.3.9.2/common/fastapi/aws/__init__.py
+-rw-r--r--   0 alfredo    (501) staff       (20)     1253 2022-07-21 09:24:21.000000 fastapi-common-0.3.9.2/common/fastapi/aws/manager.py
+drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2022-09-27 21:12:34.686936 fastapi-common-0.3.9.2/common/fastapi/core/
+-rw-r--r--   0 alfredo    (501) staff       (20)        0 2022-03-07 23:52:58.000000 fastapi-common-0.3.9.2/common/fastapi/core/__init__.py
+drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2022-09-27 21:12:34.687233 fastapi-common-0.3.9.2/common/fastapi/core/app/
+-rw-r--r--   0 alfredo    (501) staff       (20)       42 2022-03-08 01:01:29.000000 fastapi-common-0.3.9.2/common/fastapi/core/app/__init__.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      654 2022-03-15 23:31:25.000000 fastapi-common-0.3.9.2/common/fastapi/core/app/app.py
+drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2022-09-27 21:12:34.688356 fastapi-common-0.3.9.2/common/fastapi/core/commands/
+-rw-r--r--   0 alfredo    (501) staff       (20)      201 2022-03-08 03:23:19.000000 fastapi-common-0.3.9.2/common/fastapi/core/commands/__init__.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      394 2022-03-08 03:18:24.000000 fastapi-common-0.3.9.2/common/fastapi/core/commands/command.py
+-rw-r--r--   0 alfredo    (501) staff       (20)     1577 2022-05-08 01:15:19.000000 fastapi-common-0.3.9.2/common/fastapi/core/commands/load_data.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      605 2022-03-13 05:21:09.000000 fastapi-common-0.3.9.2/common/fastapi/core/commands/make_migrations.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      418 2022-03-11 08:11:55.000000 fastapi-common-0.3.9.2/common/fastapi/core/commands/pytest_cmd.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      399 2022-07-04 18:01:48.000000 fastapi-common-0.3.9.2/common/fastapi/core/commands/runserver.py
+drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2022-09-27 21:12:34.689040 fastapi-common-0.3.9.2/common/fastapi/core/parameters/
+-rw-r--r--   0 alfredo    (501) staff       (20)      142 2022-03-11 06:23:47.000000 fastapi-common-0.3.9.2/common/fastapi/core/parameters/__init__.py
+drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2022-09-27 21:12:34.690071 fastapi-common-0.3.9.2/common/fastapi/core/parameters/managers/
+-rw-r--r--   0 alfredo    (501) staff       (20)      243 2022-03-08 02:32:49.000000 fastapi-common-0.3.9.2/common/fastapi/core/parameters/managers/__init__.py
+-rw-r--r--   0 alfredo    (501) staff       (20)     3857 2022-08-09 10:03:25.000000 fastapi-common-0.3.9.2/common/fastapi/core/parameters/managers/base_manager.py
+-rw-r--r--   0 alfredo    (501) staff       (20)     1980 2022-03-11 07:10:59.000000 fastapi-common-0.3.9.2/common/fastapi/core/parameters/managers/command_manager.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      225 2022-03-08 02:32:49.000000 fastapi-common-0.3.9.2/common/fastapi/core/parameters/managers/flag_manager.py
+-rw-r--r--   0 alfredo    (501) staff       (20)     1572 2022-08-09 09:50:20.000000 fastapi-common-0.3.9.2/common/fastapi/core/parameters/managers/manager_param.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      899 2022-07-21 09:20:36.000000 fastapi-common-0.3.9.2/common/fastapi/core/parameters/managers/variable_manager.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      267 2022-03-08 02:08:06.000000 fastapi-common-0.3.9.2/common/fastapi/core/parameters/param_cfg.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      724 2022-03-08 03:08:24.000000 fastapi-common-0.3.9.2/common/fastapi/core/parameters/parameter_manager.py
+drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2022-09-27 21:12:34.691415 fastapi-common-0.3.9.2/common/fastapi/db/
+-rw-r--r--   0 alfredo    (501) staff       (20)      112 2022-05-08 00:41:36.000000 fastapi-common-0.3.9.2/common/fastapi/db/__init__.py
+-rw-r--r--   0 alfredo    (501) staff       (20)     1736 2022-05-08 02:27:02.000000 fastapi-common-0.3.9.2/common/fastapi/db/connection.py
+drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2022-09-27 21:12:34.692622 fastapi-common-0.3.9.2/common/fastapi/db/dals/
+-rw-r--r--   0 alfredo    (501) staff       (20)       41 2022-05-08 00:41:18.000000 fastapi-common-0.3.9.2/common/fastapi/db/dals/__init__.py
+-rw-r--r--   0 alfredo    (501) staff       (20)     2708 2022-07-29 11:03:33.000000 fastapi-common-0.3.9.2/common/fastapi/db/dals/async_crud_dal.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      754 2022-08-06 04:27:05.000000 fastapi-common-0.3.9.2/common/fastapi/db/dals/base_dal.py
+-rw-r--r--   0 alfredo    (501) staff       (20)     2507 2022-07-29 11:33:44.000000 fastapi-common-0.3.9.2/common/fastapi/db/dals/crud_dal.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      408 2022-05-24 04:43:22.000000 fastapi-common-0.3.9.2/common/fastapi/db/dals/dal_access.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      398 2022-03-13 04:42:42.000000 fastapi-common-0.3.9.2/common/fastapi/db/db_access.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      577 2022-05-16 19:37:44.000000 fastapi-common-0.3.9.2/common/fastapi/db/decorators.py
+-rw-r--r--   0 alfredo    (501) staff       (20)     1924 2022-08-09 03:40:41.000000 fastapi-common-0.3.9.2/common/fastapi/db/test_db.py
+-rw-r--r--   0 alfredo    (501) staff       (20)     3000 2022-08-07 22:52:01.000000 fastapi-common-0.3.9.2/common/fastapi/db/utils.py
+drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2022-09-27 21:12:34.693096 fastapi-common-0.3.9.2/common/fastapi/requests/
+-rw-r--r--   0 alfredo    (501) staff       (20)      110 2022-02-21 23:24:00.000000 fastapi-common-0.3.9.2/common/fastapi/requests/__init__.py
+-rw-r--r--   0 alfredo    (501) staff       (20)     3484 2022-03-11 08:36:34.000000 fastapi-common-0.3.9.2/common/fastapi/requests/base_manager.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      113 2022-03-09 04:31:33.000000 fastapi-common-0.3.9.2/common/fastapi/requests/response_type.py
+drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2022-09-27 21:12:34.694158 fastapi-common-0.3.9.2/common/fastapi/routing/
+-rw-r--r--   0 alfredo    (501) staff       (20)      232 2022-03-17 23:41:31.000000 fastapi-common-0.3.9.2/common/fastapi/routing/__init__.py
+-rw-r--r--   0 alfredo    (501) staff       (20)     2125 2022-08-09 07:43:58.000000 fastapi-common-0.3.9.2/common/fastapi/routing/base_crud_router.py
+-rw-r--r--   0 alfredo    (501) staff       (20)     2976 2022-08-09 03:19:18.000000 fastapi-common-0.3.9.2/common/fastapi/routing/base_router.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      969 2022-03-22 19:36:25.000000 fastapi-common-0.3.9.2/common/fastapi/routing/enum.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      541 2022-02-21 23:04:40.000000 fastapi-common-0.3.9.2/common/fastapi/routing/generic_crud_router.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      324 2022-02-21 23:04:46.000000 fastapi-common-0.3.9.2/common/fastapi/routing/generic_router.py
+-rw-r--r--   0 alfredo    (501) staff       (20)     1600 2022-02-17 22:39:07.000000 fastapi-common-0.3.9.2/common/fastapi/routing/utils.py
+drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2022-09-27 21:12:34.694879 fastapi-common-0.3.9.2/common/fastapi/schemas/
+-rw-r--r--   0 alfredo    (501) staff       (20)      233 2022-08-09 07:43:31.000000 fastapi-common-0.3.9.2/common/fastapi/schemas/__init__.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      827 2022-04-05 00:51:47.000000 fastapi-common-0.3.9.2/common/fastapi/schemas/base_schema.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      677 2022-08-09 07:43:21.000000 fastapi-common-0.3.9.2/common/fastapi/schemas/http.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      480 2022-03-25 21:04:02.000000 fastapi-common-0.3.9.2/common/fastapi/schemas/request.py
+drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2022-09-27 21:12:34.695333 fastapi-common-0.3.9.2/common/fastapi/testing/
+-rw-r--r--   0 alfredo    (501) staff       (20)       78 2022-03-11 07:06:46.000000 fastapi-common-0.3.9.2/common/fastapi/testing/__init__.py
+-rw-r--r--   0 alfredo    (501) staff       (20)     2266 2022-05-08 02:03:43.000000 fastapi-common-0.3.9.2/common/fastapi/testing/decorators.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      778 2022-03-11 08:11:42.000000 fastapi-common-0.3.9.2/common/fastapi/testing/test_case.py
+drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2022-09-27 21:12:34.695727 fastapi-common-0.3.9.2/common/fastapi/utils/
+-rw-r--r--   0 alfredo    (501) staff       (20)      132 2022-03-08 03:22:53.000000 fastapi-common-0.3.9.2/common/fastapi/utils/__init__.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      978 2022-03-09 20:32:03.000000 fastapi-common-0.3.9.2/common/fastapi/utils/functions.py
+-rw-r--r--   0 alfredo    (501) staff       (20)      467 2022-03-08 02:05:35.000000 fastapi-common-0.3.9.2/common/fastapi/utils/singleton.py
+drwxr-xr-x   0 alfredo    (501) staff       (20)        0 2022-09-27 21:12:34.696389 fastapi-common-0.3.9.2/fastapi_common.egg-info/
+-rw-r--r--   0 alfredo    (501) staff       (20)      380 2022-09-27 21:12:34.000000 fastapi-common-0.3.9.2/fastapi_common.egg-info/PKG-INFO
+-rw-r--r--   0 alfredo    (501) staff       (20)     2297 2022-09-27 21:12:34.000000 fastapi-common-0.3.9.2/fastapi_common.egg-info/SOURCES.txt
+-rw-r--r--   0 alfredo    (501) staff       (20)        1 2022-09-27 21:12:34.000000 fastapi-common-0.3.9.2/fastapi_common.egg-info/dependency_links.txt
+-rw-r--r--   0 alfredo    (501) staff       (20)        7 2022-09-27 21:12:34.000000 fastapi-common-0.3.9.2/fastapi_common.egg-info/namespace_packages.txt
+-rw-r--r--   0 alfredo    (501) staff       (20)       58 2022-09-27 21:12:34.000000 fastapi-common-0.3.9.2/fastapi_common.egg-info/requires.txt
+-rw-r--r--   0 alfredo    (501) staff       (20)        7 2022-09-27 21:12:34.000000 fastapi-common-0.3.9.2/fastapi_common.egg-info/top_level.txt
+-rw-r--r--   0 alfredo    (501) staff       (20)       38 2022-09-27 21:12:34.696763 fastapi-common-0.3.9.2/setup.cfg
+-rw-r--r--   0 alfredo    (501) staff       (20)      729 2022-09-27 21:12:26.000000 fastapi-common-0.3.9.2/setup.py
```

### Comparing `fastapi-common-0.3.12.0/LICENSE` & `fastapi-common-0.3.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/README.md` & `fastapi-common-0.3.9.2/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/common/fastapi/aws/manager.py` & `fastapi-common-0.3.9.2/common/fastapi/aws/manager.py`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/common/fastapi/core/app/app.py` & `fastapi-common-0.3.9.2/common/fastapi/core/app/app.py`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/common/fastapi/core/commands/load_data.py` & `fastapi-common-0.3.9.2/common/fastapi/core/commands/load_data.py`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/common/fastapi/core/commands/make_migrations.py` & `fastapi-common-0.3.9.2/common/fastapi/core/commands/make_migrations.py`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/common/fastapi/core/parameters/managers/base_manager.py` & `fastapi-common-0.3.9.2/common/fastapi/core/parameters/managers/base_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,23 +45,20 @@
                 return '='.join(value.split('=')[1:])
             elif field_type == SysArgv:
                 try:
                     return sys.argv[self._last_index]
                 except IndexError:
                     pass
         if field_type in [Environ, Mixed]:
-            res = os.environ.get(field_name, None)
-            if res is not None:
-                return res
+            return os.environ.get(field_name, None)
         if field_type == Mixed:
             try:
                 return sys.argv[self._last_index]
             except IndexError:
                 pass
-
         if field.default is Ellipsis:
             raise ValueError(f'value {field_name} must be setted')
         return field.default
 
     def _get_list_value(self, field_name) -> Optional[List]:
         field: ManagerParameter = self.get_field(field_name)
         field_type = type(field)
@@ -91,21 +88,15 @@
         fields = list(vars(target_obj).items())
         if hasattr(target_obj, '__annotations__'):
             fields += list(target_obj.__annotations__.items())
         return filter(lambda field: predicate(field, self), fields)
 
     def _set_parameters_by_predicate(self, target, predicate):
         fields = self._get_parameters_by_predicate(predicate)
-        errors: List[ValueError] = []
         for field, field_type in fields:
-            try:
-                value = self._get_field_by_type(field, field_type)
-                setattr(target, field, value)
-            except ValueError as e:  # type: ValueError
-                errors.append(e.args[0])
-        if errors:
-            raise ValueError(errors)
+            value = self._get_field_by_type(field, field_type)
+            setattr(target, field, value)
 
     def _set_parameters(self):
         self._set_parameters_by_predicate(target=self, predicate=is_bool_param)
         self._set_parameters_by_predicate(target=self, predicate=is_str_param)
         self._set_parameters_by_predicate(target=self, predicate=is_list_param)
```

### Comparing `fastapi-common-0.3.12.0/common/fastapi/core/parameters/managers/command_manager.py` & `fastapi-common-0.3.9.2/common/fastapi/core/parameters/managers/command_manager.py`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/common/fastapi/core/parameters/managers/manager_param.py` & `fastapi-common-0.3.9.2/common/fastapi/core/parameters/managers/manager_param.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class ManagerParameter(Generic[T]):
     """
     A generic manager param which receives a type and has a default value
     """
     default: T
 
-    def __init__(self, default: T):
+    def __init__(self, default: T) -> object:
         """
 
         :rtype: object
         """
         self.default = default
```

### Comparing `fastapi-common-0.3.12.0/common/fastapi/core/parameters/managers/variable_manager.py` & `fastapi-common-0.3.9.2/common/fastapi/core/parameters/managers/variable_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     DB_PASS: str = Environ(...)
     DB_HOST: str = Environ(...)
     DB_PORT: str = Environ(...)
     DB_NAME: str = Environ(...)
     SECRET_KEY: str = Environ(None)
     STATIC_FOLDER: str = Environ(None)
     STATIC_URL: str = Environ(None)
+    ACCESS_KEY_ID: str = Environ(None)
+    SECRET_ACCESS_KEY: str = Environ(None)
 
     def backup(self):
         self._backup_data.append(vars(self).copy())
 
     def restore(self, index=-1):
         if not self._backup_data:
             raise AssertionError('There is no backup to restore')
```

### Comparing `fastapi-common-0.3.12.0/common/fastapi/core/parameters/parameter_manager.py` & `fastapi-common-0.3.9.2/common/fastapi/core/parameters/parameter_manager.py`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/common/fastapi/db/connection.py` & `fastapi-common-0.3.9.2/common/fastapi/db/connection.py`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/common/fastapi/db/dals/async_crud_dal.py` & `fastapi-common-0.3.9.2/common/fastapi/db/dals/async_crud_dal.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,65 +21,58 @@
     async def create(self, data) -> T:
         item = self.model(**data)
         self._db.add(item)
 
         if self._auto_commit:
             await self.commit()
             await self._db.refresh(item)
-        else:
-            await self.flush()
         return item
 
     async def list(self, **query) -> List[T]:
         query_performed = query_perform(self.model, **query)
         stmt = select(self.model).filter(*query_performed)
         result = await self._db.execute(stmt)
         return result.scalars()
 
-    # TODO: might fail because no async function
     def get_object_or_404(self, **query) -> T:
         item = self.get_object(**query)
         if not item:
             raise HTTPException(404, f'{self.model.__name__} object not found')
         return item
 
     async def get_object(self, **query):
         query_performed = query_perform(self.model, **query)
 
         stmt = select(self.model).filter(*query_performed)
         result = await self._db.execute(stmt)
         return result.scalars().first()
 
-    async def detail(self, **query) -> T:
-        return await self.get_object_or_404(**query)
+    def detail(self, **query) -> T:
+        return self.get_object_or_404(**query)
 
     async def delete_all(self):
         query = delete(self.model)
         await self._db.execute(query)
         await self._db.commit()
 
     async def delete(self, **query):
         item = self.detail(**query)
         self._db.delete(item)
         if self._auto_commit:
             await self.commit()
-        else:
-            await self.flush()
 
     async def update(self, data, **query) -> T:
         item = self.get_object_or_404(**query)
         if 'id' in data:
             raise ValueError("updated data cannot include object's id")
         update_data = {getattr(self.model, key): value for key, value in data.items()}
         item.update(update_data)
 
         if self._auto_commit:
             await self.commit()
-        else:
-            await self.flush()
         return item.first()
 
     @classmethod
     async def bulk_create(cls, data, bulk_count):
         from . import get_dal
         dal: cls = await get_dal(cls, auto_commit=False)
         for count, item in enumerate(data):
```

### Comparing `fastapi-common-0.3.12.0/common/fastapi/db/dals/base_dal.py` & `fastapi-common-0.3.9.2/common/fastapi/db/dals/base_dal.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 from typing import Type
 
+
 class Dal:
     _auto_commit: bool = True
 
     def __init__(self, db, auto_commit=True, *args, **kwargs):
         self._db = db
         self._auto_commit = auto_commit
 
     # noinspection PyPep8Naming
-    def get_dal(self, DalType: Type['Dal'], *args, **kwargs):
-        dal = DalType(db=self._db, auto_commit=False, *args, **kwargs)
+    def get_dal(self, DalType: Type['Dal']):
+        dal = DalType(self._db, False)
         return dal
 
     def commit(self):
         self._db.commit()
 
-    def flush(self):
-        self._db.flush()
-
 
 class AsyncDal:
     _auto_commit: bool = True
 
     def __init__(self, db, auto_commit=True, *args, **kwargs):
         self._db = db
         self._auto_commit = auto_commit
 
     # noinspection PyPep8Naming
     def get_dal(self, DalType: Type['AsyncDal']):
-        dal = DalType(db=self._db, auto_commit=False)
+        dal = DalType(self._db, False)
         return dal
 
     async def commit(self):
         await self._db.commit()
-
-    async def flush(self):
-        await self._db.flush()
```

### Comparing `fastapi-common-0.3.12.0/common/fastapi/db/decorators.py` & `fastapi-common-0.3.9.2/common/fastapi/db/decorators.py`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/common/fastapi/db/test_db.py` & `fastapi-common-0.3.9.2/common/fastapi/db/test_db.py`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/common/fastapi/db/utils.py` & `fastapi-common-0.3.9.2/common/fastapi/db/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/common/fastapi/requests/base_manager.py` & `fastapi-common-0.3.9.2/common/fastapi/requests/base_manager.py`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/common/fastapi/routing/base_crud_router.py` & `fastapi-common-0.3.9.2/common/fastapi/routing/base_crud_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,20 +36,20 @@
         async def remove(id: int, dal: CRUDDal = Depends(get_dal_dependency(CRUDDal, model=self.model))):
             dal.delete(id=id)
             return HTTP_200_REMOVED
 
         @put('/detail/{id}', response_model=HTTPResponseModel)
         async def update_detail(id: int, request: request_schema,
                                 dal: CRUDDal = Depends(get_dal_dependency(CRUDDal, model=self.model))):
-            data = request.data
+            data = request.data.dict()
             dal.update(data, id=id)
             return HTTP_200_UPDATED
 
         @post('/create', response_model=HTTPResponseModel)
         async def create(request: request_schema,
                          dal: CRUDDal = Depends(get_dal_dependency(CRUDDal, model=self.model))):
-            data = request.data
+            data = request.data.dict()
             dal.create(data)
             return HTTP_201_CREATED
 
         return ('create', create), ('list', list), ('update_detail', update_detail), ('remove', remove), (
             'detail', detail)
```

### Comparing `fastapi-common-0.3.12.0/common/fastapi/routing/base_router.py` & `fastapi-common-0.3.9.2/common/fastapi/routing/base_router.py`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/common/fastapi/routing/enum.py` & `fastapi-common-0.3.9.2/common/fastapi/routing/enum.py`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/common/fastapi/routing/generic_crud_router.py` & `fastapi-common-0.3.9.2/common/fastapi/routing/generic_crud_router.py`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/common/fastapi/routing/utils.py` & `fastapi-common-0.3.9.2/common/fastapi/routing/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/common/fastapi/schemas/base_schema.py` & `fastapi-common-0.3.9.2/common/fastapi/schemas/base_schema.py`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/common/fastapi/schemas/http.py` & `fastapi-common-0.3.9.2/common/fastapi/schemas/http.py`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/common/fastapi/testing/decorators.py` & `fastapi-common-0.3.9.2/common/fastapi/testing/decorators.py`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/common/fastapi/testing/test_case.py` & `fastapi-common-0.3.9.2/common/fastapi/testing/test_case.py`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/common/fastapi/utils/functions.py` & `fastapi-common-0.3.9.2/common/fastapi/utils/functions.py`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/fastapi_common.egg-info/SOURCES.txt` & `fastapi-common-0.3.9.2/fastapi_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi-common-0.3.12.0/setup.py` & `fastapi-common-0.3.9.2/setup.py`

 * *Files identical despite different names*


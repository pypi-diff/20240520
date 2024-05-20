# Comparing `tmp/aws-xray-sdk-2.8.0.tar.gz` & `tmp/aws-xray-sdk-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aws-xray-sdk-2.8.0.tar", last modified: Thu Apr 29 00:03:01 2021, max compression
+gzip compressed data, was "dist/aws-xray-sdk-2.9.0.tar", last modified: Mon Dec  6 20:54:38 2021, max compression
```

## Comparing `aws-xray-sdk-2.8.0.tar` & `aws-xray-sdk-2.9.0.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)    11357 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/LICENSE
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     1776 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/setup.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)       67 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/setup.cfg
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk.egg-info/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     4053 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)        1 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)    23070 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk.egg-info/PKG-INFO
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)       13 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk.egg-info/top_level.txt
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)       64 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk.egg-info/requires.txt
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)      123 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/MANIFEST.in
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     3417 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/sdk_config.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/httplib/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     7817 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/httplib/patch.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)      126 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/httplib/__init__.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/django/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     2268 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/django/apps.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     3685 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/django/middleware.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     2689 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/django/db.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)       63 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/django/__init__.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     1026 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/django/templates.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     2279 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/django/conf.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/flask/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     4013 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/flask/middleware.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/flask/__init__.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/aiohttp/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     3009 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/aiohttp/middleware.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/aiohttp/__init__.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     2627 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/aiohttp/client.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/sqlalchemy/
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/sqlalchemy/util/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     4317 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/sqlalchemy/util/decorators.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/sqlalchemy/util/__init__.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)      750 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/sqlalchemy/query.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/sqlalchemy/__init__.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/mysql/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)      986 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/mysql/patch.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)       47 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/mysql/__init__.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/botocore/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     1217 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/botocore/patch.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)       46 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/botocore/__init__.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/bottle/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     3944 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/bottle/middleware.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/bottle/__init__.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/pymysql/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     1161 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/pymysql/patch.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)       67 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/pymysql/__init__.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/pg8000/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)      914 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/pg8000/patch.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)       67 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/pg8000/__init__.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     4608 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/boto_utils.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     4456 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/util.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/sqlalchemy_core/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     3810 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/sqlalchemy_core/patch.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)       65 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/sqlalchemy_core/__init__.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/psycopg2/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     1582 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/psycopg2/patch.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)       47 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/psycopg2/__init__.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/pynamodb/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     2676 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/pynamodb/patch.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)       46 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/pynamodb/__init__.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/pymongo/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     2334 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/pymongo/patch.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)      108 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/pymongo/__init__.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/__init__.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/flask_sqlalchemy/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     2491 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/flask_sqlalchemy/query.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/flask_sqlalchemy/__init__.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/resources/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)    21929 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/resources/aws_para_whitelist.json
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/requests/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     1490 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/requests/patch.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)       46 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/requests/__init__.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/sqlite3/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)      708 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/sqlite3/patch.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)       47 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/sqlite3/__init__.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/aiobotocore/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     1028 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/aiobotocore/patch.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)       46 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/aiobotocore/__init__.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     1886 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/ext/dbapi2.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/utils/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)      696 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/utils/atomic_counter.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     1970 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/utils/stacktrace.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     1198 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/utils/conversion.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/utils/__init__.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)      834 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/utils/compat.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     1892 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/utils/search_pattern.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     4657 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/lambda_launcher.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/plugins/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)      432 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/plugins/ecs_plugin.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     2194 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/plugins/ec2_plugin.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)      469 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/plugins/elasticbeanstalk_plugin.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/plugins/__init__.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)      757 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/plugins/utils.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)      382 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/http.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     5216 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/subsegment.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     3820 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/facade_segment.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     3512 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/trace_header.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     1218 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/default_dynamic_naming.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)      774 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/traceid.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     2412 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/throwable.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)    10269 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/entity.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/__init__.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     3219 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/dummy_entities.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)      708 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/noop_traceid.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     5292 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/segment.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     6304 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/connector.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     2556 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/rule_cache.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/local/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)      104 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/local/sampling_rule.json
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/local/__init__.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     3699 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/local/sampling_rule.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     1028 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/local/reservoir.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     3532 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/local/sampler.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     1888 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/rule_poller.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/__init__.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     4346 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/sampling_rule.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     2285 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/target_poller.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     2735 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/reservoir.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     4634 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/sampler.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)    21345 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/recorder.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/emitters/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/emitters/__init__.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     2317 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/emitters/udp_emitter.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     7674 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/patcher.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/streaming/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     1983 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/streaming/default_streaming.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/streaming/__init__.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     4927 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/context.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)      351 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/__init__.py
-drwxr-xr-x   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/exceptions/
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)      445 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/exceptions/exceptions.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)        0 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/exceptions/__init__.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     2524 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/daemon_config.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     3832 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/async_recorder.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)     3392 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/core/async_context.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)       18 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/version.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)       67 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/aws_xray_sdk/__init__.py
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)    23070 2021-04-29 00:03:01.000000 aws-xray-sdk-2.8.0/PKG-INFO
--rw-r--r--   0 bolpeng  (11919509) amazon     (100)    17867 2021-04-29 00:01:38.000000 aws-xray-sdk-2.8.0/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/
+-rw-r--r--   0 root         (0) staff       (20)    23070 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)    11357 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/LICENSE
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/
+-rw-r--r--   0 root         (0) staff       (20)     3832 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/async_recorder.py
+-rw-r--r--   0 root         (0) staff       (20)     2524 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/daemon_config.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/plugins/
+-rw-r--r--   0 root         (0) staff       (20)      432 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/plugins/ecs_plugin.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/plugins/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      757 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/plugins/utils.py
+-rw-r--r--   0 root         (0) staff       (20)      469 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/plugins/elasticbeanstalk_plugin.py
+-rw-r--r--   0 root         (0) staff       (20)     2194 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/plugins/ec2_plugin.py
+-rw-r--r--   0 root         (0) staff       (20)    21369 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/recorder.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/
+-rw-r--r--   0 root         (0) staff       (20)     2285 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/target_poller.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1888 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/rule_poller.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/local/
+-rw-r--r--   0 root         (0) staff       (20)      104 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/local/sampling_rule.json
+-rw-r--r--   0 root         (0) staff       (20)        0 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/local/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3699 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/local/sampling_rule.py
+-rw-r--r--   0 root         (0) staff       (20)     1028 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/local/reservoir.py
+-rw-r--r--   0 root         (0) staff       (20)     3479 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/local/sampler.py
+-rw-r--r--   0 root         (0) staff       (20)     6304 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/connector.py
+-rw-r--r--   0 root         (0) staff       (20)     4346 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/sampling_rule.py
+-rw-r--r--   0 root         (0) staff       (20)     2735 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/reservoir.py
+-rw-r--r--   0 root         (0) staff       (20)     4634 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/sampler.py
+-rw-r--r--   0 root         (0) staff       (20)     2556 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/rule_cache.py
+-rw-r--r--   0 root         (0) staff       (20)      351 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/utils/
+-rw-r--r--   0 root         (0) staff       (20)     1970 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/utils/stacktrace.py
+-rw-r--r--   0 root         (0) staff       (20)      696 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/utils/atomic_counter.py
+-rw-r--r--   0 root         (0) staff       (20)      834 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/utils/compat.py
+-rw-r--r--   0 root         (0) staff       (20)     1187 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/utils/conversion.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/utils/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1892 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/utils/search_pattern.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/
+-rw-r--r--   0 root         (0) staff       (20)     2412 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/throwable.py
+-rw-r--r--   0 root         (0) staff       (20)     1218 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/default_dynamic_naming.py
+-rw-r--r--   0 root         (0) staff       (20)     5216 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/subsegment.py
+-rw-r--r--   0 root         (0) staff       (20)     3512 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/trace_header.py
+-rw-r--r--   0 root         (0) staff       (20)     3820 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/facade_segment.py
+-rw-r--r--   0 root         (0) staff       (20)     3219 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/dummy_entities.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      382 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/http.py
+-rw-r--r--   0 root         (0) staff       (20)    10269 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/entity.py
+-rw-r--r--   0 root         (0) staff       (20)     5292 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/segment.py
+-rw-r--r--   0 root         (0) staff       (20)      774 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/traceid.py
+-rw-r--r--   0 root         (0) staff       (20)      708 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/noop_traceid.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/exceptions/
+-rw-r--r--   0 root         (0) staff       (20)        0 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/exceptions/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      445 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/exceptions/exceptions.py
+-rw-r--r--   0 root         (0) staff       (20)     3392 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/async_context.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/streaming/
+-rw-r--r--   0 root         (0) staff       (20)     1983 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/streaming/default_streaming.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/streaming/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     4884 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/context.py
+-rw-r--r--   0 root         (0) staff       (20)     7674 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/patcher.py
+-rw-r--r--   0 root         (0) staff       (20)     4657 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/lambda_launcher.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/emitters/
+-rw-r--r--   0 root         (0) staff       (20)     2317 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/emitters/udp_emitter.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/core/emitters/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)       18 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/version.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/flask/
+-rw-r--r--   0 root         (0) staff       (20)        0 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/flask/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     4013 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/flask/middleware.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/aiohttp/
+-rw-r--r--   0 root         (0) staff       (20)     2627 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/aiohttp/client.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/aiohttp/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3009 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/aiohttp/middleware.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/pymysql/
+-rw-r--r--   0 root         (0) staff       (20)     1161 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/pymysql/patch.py
+-rw-r--r--   0 root         (0) staff       (20)       67 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/pymysql/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/flask_sqlalchemy/
+-rw-r--r--   0 root         (0) staff       (20)     2491 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/flask_sqlalchemy/query.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/flask_sqlalchemy/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/aiobotocore/
+-rw-r--r--   0 root         (0) staff       (20)     1028 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/aiobotocore/patch.py
+-rw-r--r--   0 root         (0) staff       (20)       46 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/aiobotocore/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     4456 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/util.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/resources/
+-rw-r--r--   0 root         (0) staff       (20)    21929 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/resources/aws_para_whitelist.json
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/pynamodb/
+-rw-r--r--   0 root         (0) staff       (20)     2676 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/pynamodb/patch.py
+-rw-r--r--   0 root         (0) staff       (20)       46 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/pynamodb/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/sqlalchemy/
+-rw-r--r--   0 root         (0) staff       (20)      750 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/sqlalchemy/query.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/sqlalchemy/util/
+-rw-r--r--   0 root         (0) staff       (20)        0 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/sqlalchemy/util/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     4317 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/sqlalchemy/util/decorators.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/sqlalchemy/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/httplib/
+-rw-r--r--   0 root         (0) staff       (20)     7817 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/httplib/patch.py
+-rw-r--r--   0 root         (0) staff       (20)      126 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/httplib/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/pymongo/
+-rw-r--r--   0 root         (0) staff       (20)     2334 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/pymongo/patch.py
+-rw-r--r--   0 root         (0) staff       (20)      108 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/pymongo/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/botocore/
+-rw-r--r--   0 root         (0) staff       (20)     1217 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/botocore/patch.py
+-rw-r--r--   0 root         (0) staff       (20)       46 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/botocore/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/requests/
+-rw-r--r--   0 root         (0) staff       (20)     1490 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/requests/patch.py
+-rw-r--r--   0 root         (0) staff       (20)       46 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/requests/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/sqlalchemy_core/
+-rw-r--r--   0 root         (0) staff       (20)     3810 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/sqlalchemy_core/patch.py
+-rw-r--r--   0 root         (0) staff       (20)       65 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/sqlalchemy_core/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/sqlite3/
+-rw-r--r--   0 root         (0) staff       (20)      708 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/sqlite3/patch.py
+-rw-r--r--   0 root         (0) staff       (20)       47 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/sqlite3/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/mysql/
+-rw-r--r--   0 root         (0) staff       (20)      986 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/mysql/patch.py
+-rw-r--r--   0 root         (0) staff       (20)       47 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/mysql/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1886 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/dbapi2.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/psycopg2/
+-rw-r--r--   0 root         (0) staff       (20)     1582 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/psycopg2/patch.py
+-rw-r--r--   0 root         (0) staff       (20)       47 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/psycopg2/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     4535 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/boto_utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/django/
+-rw-r--r--   0 root         (0) staff       (20)     2689 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/django/db.py
+-rw-r--r--   0 root         (0) staff       (20)     2279 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/django/conf.py
+-rw-r--r--   0 root         (0) staff       (20)       63 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/django/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     2268 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/django/apps.py
+-rw-r--r--   0 root         (0) staff       (20)     1026 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/django/templates.py
+-rw-r--r--   0 root         (0) staff       (20)     3685 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/django/middleware.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/bottle/
+-rw-r--r--   0 root         (0) staff       (20)        0 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/bottle/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3944 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/bottle/middleware.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/pg8000/
+-rw-r--r--   0 root         (0) staff       (20)      914 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/pg8000/patch.py
+-rw-r--r--   0 root         (0) staff       (20)       67 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/ext/pg8000/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)       67 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3417 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/aws_xray_sdk/sdk_config.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/aws_xray_sdk.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)    23070 2021-12-06 20:54:37.000000 aws-xray-sdk-2.9.0/aws_xray_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     4053 2021-12-06 20:54:37.000000 aws-xray-sdk-2.9.0/aws_xray_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)       64 2021-12-06 20:54:37.000000 aws-xray-sdk-2.9.0/aws_xray_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       13 2021-12-06 20:54:37.000000 aws-xray-sdk-2.9.0/aws_xray_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2021-12-06 20:54:37.000000 aws-xray-sdk-2.9.0/aws_xray_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)      123 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)    17867 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/README.md
+-rw-r--r--   0 root         (0) staff       (20)     1776 2021-12-06 20:53:53.000000 aws-xray-sdk-2.9.0/setup.py
+-rw-r--r--   0 root         (0) staff       (20)       67 2021-12-06 20:54:38.000000 aws-xray-sdk-2.9.0/setup.cfg
```

### Comparing `aws-xray-sdk-2.8.0/LICENSE` & `aws-xray-sdk-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/setup.py` & `aws-xray-sdk-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk.egg-info/SOURCES.txt` & `aws-xray-sdk-2.9.0/aws_xray_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk.egg-info/PKG-INFO` & `aws-xray-sdk-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-xray-sdk
-Version: 2.8.0
+Version: 2.9.0
 Summary: The AWS X-Ray SDK for Python (the SDK) enables Python developers to record and emit information from within their applications to the AWS X-Ray service.
 Home-page: https://github.com/aws/aws-xray-sdk-python
 Author: Amazon Web Services
 License: Apache License 2.0
 Description: [![Build Status](https://travis-ci.org/aws/aws-xray-sdk-python.svg?branch=master)](https://travis-ci.org/aws/aws-xray-sdk-python)
         [![codecov](https://codecov.io/gh/aws/aws-xray-sdk-python/branch/master/graph/badge.svg)](https://codecov.io/gh/aws/aws-xray-sdk-python)
```

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/sdk_config.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/sdk_config.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/httplib/patch.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/httplib/patch.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/django/apps.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/django/apps.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/django/middleware.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/django/middleware.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/django/db.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/django/db.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/django/templates.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/django/templates.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/django/conf.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/django/conf.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/flask/middleware.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/flask/middleware.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/aiohttp/middleware.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/aiohttp/middleware.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/aiohttp/client.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/aiohttp/client.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/sqlalchemy/util/decorators.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/sqlalchemy/util/decorators.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/sqlalchemy/query.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/sqlalchemy/query.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/mysql/patch.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/mysql/patch.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/botocore/patch.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/botocore/patch.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/bottle/middleware.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/bottle/middleware.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/pymysql/patch.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/pymysql/patch.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/pg8000/patch.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/pg8000/patch.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/boto_utils.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/boto_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from __future__ import absolute_import
 # Need absolute import as botocore is also in the current folder for py27
 import json
+import pkgutil
 
-from pkg_resources import resource_filename
 from botocore.exceptions import ClientError
 
 from aws_xray_sdk.core import xray_recorder
 from aws_xray_sdk.core.models import http
 from aws_xray_sdk.core.exceptions.exceptions import SegmentNotFoundException
 
 from aws_xray_sdk.ext.util import inject_trace_header, to_snake_case
 
 
-with open(resource_filename(__name__, 'resources/aws_para_whitelist.json'), 'r') as data_file:
-    whitelist = json.load(data_file)
+whitelist = json.loads(pkgutil.get_data(__name__, 'resources/aws_para_whitelist.json'))
 
 
 def inject_header(wrapped, instance, args, kwargs):
     # skip tracing for SDK built-in centralized sampling pollers
     url = args[0].url
     if 'GetCentralizedSamplingRules' in url or 'SamplingTargets' in url:
         return wrapped(*args, **kwargs)
```

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/util.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/util.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/sqlalchemy_core/patch.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/sqlalchemy_core/patch.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/psycopg2/patch.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/psycopg2/patch.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/pynamodb/patch.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/pynamodb/patch.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/pymongo/patch.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/pymongo/patch.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/flask_sqlalchemy/query.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/flask_sqlalchemy/query.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/resources/aws_para_whitelist.json` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/resources/aws_para_whitelist.json`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/requests/patch.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/requests/patch.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/sqlite3/patch.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/sqlite3/patch.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/aiobotocore/patch.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/aiobotocore/patch.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/ext/dbapi2.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/ext/dbapi2.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/utils/atomic_counter.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/utils/atomic_counter.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/utils/stacktrace.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/utils/stacktrace.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/utils/conversion.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/utils/conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,9 +27,9 @@
             for key, value in vars(obj).items():
                 if not callable(value) and not key.startswith('_'):
                     metadata[key] = metadata_to_dict(value)
             return metadata
         else:
             return obj
     except Exception:
-        log.exception("Failed to convert {} to dict".format(str(obj)))
+        log.exception("Failed to convert metadata to dict")
         return {}
```

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/utils/compat.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/utils/compat.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/utils/search_pattern.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/utils/search_pattern.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/lambda_launcher.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/lambda_launcher.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/plugins/ec2_plugin.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/plugins/ec2_plugin.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/plugins/utils.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/subsegment.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/subsegment.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/facade_segment.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/facade_segment.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/trace_header.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/trace_header.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/default_dynamic_naming.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/default_dynamic_naming.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/traceid.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/traceid.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/throwable.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/throwable.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/entity.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/entity.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/dummy_entities.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/dummy_entities.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/noop_traceid.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/noop_traceid.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/models/segment.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/models/segment.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/connector.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/connector.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/rule_cache.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/rule_cache.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/local/sampling_rule.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/local/sampling_rule.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/local/reservoir.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/local/reservoir.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/local/sampler.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/local/sampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import json
+import pkgutil
 from random import Random
 
-from pkg_resources import resource_filename
 from .sampling_rule import SamplingRule
 from ...exceptions.exceptions import InvalidSamplingManifestError
 
-
-with open(resource_filename(__name__, 'sampling_rule.json')) as f:
-    local_sampling_rule = json.load(f)
+local_sampling_rule = json.loads(pkgutil.get_data(__name__, 'sampling_rule.json'))
 
 SUPPORTED_RULE_VERSION = (1, 2)
 
 
 class LocalSampler(object):
     """
     The local sampler that holds either custom sampling rules
```

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/rule_poller.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/rule_poller.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/sampling_rule.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/sampling_rule.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/target_poller.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/target_poller.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/reservoir.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/reservoir.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/sampling/sampler.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/sampling/sampler.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/recorder.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/recorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 from aws_xray_sdk import global_sdk_config
 from aws_xray_sdk.version import VERSION
 from .models.segment import Segment, SegmentContextManager
 from .models.subsegment import Subsegment, SubsegmentContextManager
 from .models.default_dynamic_naming import DefaultDynamicNaming
 from .models.dummy_entities import DummySegment, DummySubsegment
 from .emitters.udp_emitter import UDPEmitter
-from .sampling.sampler import DefaultSampler
-from .sampling.local.sampler import LocalSampler
 from .streaming.default_streaming import DefaultStreaming
 from .context import Context
 from .daemon_config import DaemonConfig
 from .plugins.utils import get_plugin_modules
 from .lambda_launcher import check_in_lambda
 from .exceptions.exceptions import SegmentNameMissingException, SegmentNotFoundException
 from .utils.compat import string_types
@@ -54,18 +52,20 @@
     """
     def __init__(self):
 
         self._streaming = DefaultStreaming()
         context = check_in_lambda()
         if context:
             # Special handling when running on AWS Lambda.
+            from .sampling.local.sampler import LocalSampler
             self._context = context
             self.streaming_threshold = 0
             self._sampler = LocalSampler()
         else:
+            from .sampling.sampler import DefaultSampler
             self._context = Context()
             self._sampler = DefaultSampler()
 
         self._emitter = UDPEmitter()
         self._sampling = True
         self._max_trace_back = 10
         self._plugins = None
```

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/emitters/udp_emitter.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/emitters/udp_emitter.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/patcher.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/patcher.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/streaming/default_streaming.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/streaming/default_streaming.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/context.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,14 @@
         self._local.__dict__.clear()
 
     def handle_context_missing(self):
         """
         Called whenever there is no trace entity to access or mutate.
         """
         if self.context_missing == 'RUNTIME_ERROR':
-            log.error(MISSING_SEGMENT_MSG)
             raise SegmentNotFoundException(MISSING_SEGMENT_MSG)
         else:
             log.error(MISSING_SEGMENT_MSG)
 
     def _is_subsegment(self, entity):
 
         return hasattr(entity, 'type') and entity.type == 'subsegment'
```

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/daemon_config.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/daemon_config.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/async_recorder.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/async_recorder.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/aws_xray_sdk/core/async_context.py` & `aws-xray-sdk-2.9.0/aws_xray_sdk/core/async_context.py`

 * *Files identical despite different names*

### Comparing `aws-xray-sdk-2.8.0/PKG-INFO` & `aws-xray-sdk-2.9.0/aws_xray_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-xray-sdk
-Version: 2.8.0
+Version: 2.9.0
 Summary: The AWS X-Ray SDK for Python (the SDK) enables Python developers to record and emit information from within their applications to the AWS X-Ray service.
 Home-page: https://github.com/aws/aws-xray-sdk-python
 Author: Amazon Web Services
 License: Apache License 2.0
 Description: [![Build Status](https://travis-ci.org/aws/aws-xray-sdk-python.svg?branch=master)](https://travis-ci.org/aws/aws-xray-sdk-python)
         [![codecov](https://codecov.io/gh/aws/aws-xray-sdk-python/branch/master/graph/badge.svg)](https://codecov.io/gh/aws/aws-xray-sdk-python)
```

### Comparing `aws-xray-sdk-2.8.0/README.md` & `aws-xray-sdk-2.9.0/README.md`

 * *Files identical despite different names*


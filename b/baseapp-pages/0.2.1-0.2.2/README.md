# Comparing `tmp/baseapp_pages-0.2.1.tar.gz` & `tmp/baseapp_pages-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseapp_pages-0.2.1.tar", last modified: Tue Apr 16 21:09:48 2024, max compression
+gzip compressed data, was "baseapp_pages-0.2.2.tar", last modified: Sun May 19 23:32:16 2024, max compression
```

## Comparing `baseapp_pages-0.2.1.tar` & `baseapp_pages-0.2.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:09:48.249081 baseapp_pages-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-16 21:09:48.249081 baseapp_pages-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:09:48.245081 baseapp_pages-0.2.1/baseapp_pages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:09:48.245081 baseapp_pages-0.2.1/baseapp_pages/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/graphql/mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/graphql/object_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/graphql/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:09:48.245081 baseapp_pages-0.2.1/baseapp_pages/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    12927 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)    10055 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/migrations/0002_page_pageevent_page_snapshot_insert_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/migrations/0003_remove_page_snapshot_insert_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/migrations/0004_alter_page_comments_count_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:09:48.249081 baseapp_pages-0.2.1/baseapp_pages/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/tests/test_create_mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/tests/test_delete_mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/tests/test_edit_mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/tests/test_get_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/tests/test_list_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/baseapp_pages/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:09:48.245081 baseapp_pages-0.2.1/baseapp_pages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-16 21:09:48.000000 baseapp_pages-0.2.1/baseapp_pages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-16 21:09:48.000000 baseapp_pages-0.2.1/baseapp_pages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 21:09:48.000000 baseapp_pages-0.2.1/baseapp_pages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-16 21:09:48.000000 baseapp_pages-0.2.1/baseapp_pages.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 21:09:48.000000 baseapp_pages-0.2.1/baseapp_pages.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-16 21:09:48.253080 baseapp_pages-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:09:48.249081 baseapp_pages-0.2.1/testproject/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/testproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/testproject/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/testproject/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/testproject/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:09:48.249081 baseapp_pages-0.2.1/testproject/testapp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/testproject/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/testproject/testapp/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/testproject/testapp/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:09:48.249081 baseapp_pages-0.2.1/testproject/testapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/testproject/testapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/testproject/testapp/migrations/0002_auto_20160321_1909.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/testproject/testapp/migrations/0003_auto_20160725_2001.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/testproject/testapp/migrations/0004_auto_20160811_1614.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/testproject/testapp/migrations/0005_user_password_changed_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/testproject/testapp/migrations/0006_alter_user_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/testproject/testapp/migrations/0007_user_groups_user_is_staff_user_user_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/testproject/testapp/migrations/0008_user_phone_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/testproject/testapp/migrations/0009_alter_user_options.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/testproject/testapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/testproject/testapp/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/testproject/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-16 21:09:47.000000 baseapp_pages-0.2.1/testproject/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:32:16.813536 baseapp_pages-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-19 23:32:16.813536 baseapp_pages-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:32:16.805536 baseapp_pages-0.2.2/baseapp_pages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:32:16.805536 baseapp_pages-0.2.2/baseapp_pages/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/graphql/mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/graphql/object_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/graphql/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:32:16.805536 baseapp_pages-0.2.2/baseapp_pages/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    12927 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10055 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/migrations/0002_page_pageevent_page_snapshot_insert_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/migrations/0003_remove_page_snapshot_insert_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/migrations/0004_alter_page_comments_count_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:32:16.809536 baseapp_pages-0.2.2/baseapp_pages/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/tests/test_create_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/tests/test_delete_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/tests/test_edit_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/tests/test_get_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/tests/test_list_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:32:16.805536 baseapp_pages-0.2.2/baseapp_pages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/baseapp_pages.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-19 23:32:16.813536 baseapp_pages-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:32:16.809536 baseapp_pages-0.2.2/testproject/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/testproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/testproject/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/testproject/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/testproject/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:32:16.809536 baseapp_pages-0.2.2/testproject/testapp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/testproject/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/testproject/testapp/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/testproject/testapp/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:32:16.813536 baseapp_pages-0.2.2/testproject/testapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/testproject/testapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/testproject/testapp/migrations/0002_auto_20160321_1909.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/testproject/testapp/migrations/0003_auto_20160725_2001.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/testproject/testapp/migrations/0004_auto_20160811_1614.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/testproject/testapp/migrations/0005_user_password_changed_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/testproject/testapp/migrations/0006_alter_user_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/testproject/testapp/migrations/0007_user_groups_user_is_staff_user_user_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/testproject/testapp/migrations/0008_user_phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/testproject/testapp/migrations/0009_alter_user_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/testproject/testapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/testproject/testapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/testproject/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-19 23:32:16.000000 baseapp_pages-0.2.2/testproject/wsgi.py
```

### Comparing `baseapp_pages-0.2.1/PKG-INFO` & `baseapp_pages-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseapp_pages
-Version: 0.2.1
+Version: 0.2.2
 Summary: BaseApp Pages
 Home-page: https://github.com/silverlogic/baseapp-backend
 Author: The SilverLogic
 Author-email: dev@tsl.io
 License: BSD-3-Clause  # Example license
 Description: # BaseApp Pages
```

### Comparing `baseapp_pages-0.2.1/README.md` & `baseapp_pages-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/baseapp_pages/admin.py` & `baseapp_pages-0.2.2/baseapp_pages/admin.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/baseapp_pages/graphql/mutations.py` & `baseapp_pages-0.2.2/baseapp_pages/graphql/mutations.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/baseapp_pages/graphql/object_types.py` & `baseapp_pages-0.2.2/baseapp_pages/graphql/object_types.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/baseapp_pages/graphql/queries.py` & `baseapp_pages-0.2.2/baseapp_pages/graphql/queries.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/baseapp_pages/migrations/0001_initial.py` & `baseapp_pages-0.2.2/baseapp_pages/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/baseapp_pages/migrations/0002_page_pageevent_page_snapshot_insert_and_more.py` & `baseapp_pages-0.2.2/baseapp_pages/migrations/0002_page_pageevent_page_snapshot_insert_and_more.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/baseapp_pages/migrations/0003_remove_page_snapshot_insert_and_more.py` & `baseapp_pages-0.2.2/baseapp_pages/migrations/0003_remove_page_snapshot_insert_and_more.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/baseapp_pages/migrations/0004_alter_page_comments_count_and_more.py` & `baseapp_pages-0.2.2/baseapp_pages/migrations/0004_alter_page_comments_count_and_more.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/baseapp_pages/models.py` & `baseapp_pages-0.2.2/baseapp_pages/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,19 @@
             )
         ]
 
     def __str__(self):
         return self.path
 
 
-@pghistory.track(pghistory.Snapshot())
+@pghistory.track(
+    pghistory.InsertEvent(),
+    pghistory.UpdateEvent(),
+    pghistory.DeleteEvent(),
+)
 class Metadata(TimeStampedModel, RelayModel):
     target_content_type = models.ForeignKey(
         ContentType,
         blank=True,
         null=True,
         on_delete=models.CASCADE,
     )
@@ -129,11 +133,15 @@
             # Return the function unchanged, not decorated.
             return func
         return dec(func)
 
     return decorator
 
 
-@pghistory.track(pghistory.Snapshot())
+@pghistory.track(
+    pghistory.InsertEvent(),
+    pghistory.UpdateEvent(),
+    pghistory.DeleteEvent(),
+)
 class Page(AbstractPage):
     class Meta:
         swappable = swapper.swappable_setting("baseapp_pages", "Page")
```

### Comparing `baseapp_pages-0.2.1/baseapp_pages/permissions.py` & `baseapp_pages-0.2.2/baseapp_pages/permissions.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/baseapp_pages/tests/test_create_mutation.py` & `baseapp_pages-0.2.2/baseapp_pages/tests/test_create_mutation.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/baseapp_pages/tests/test_delete_mutation.py` & `baseapp_pages-0.2.2/baseapp_pages/tests/test_delete_mutation.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/baseapp_pages/tests/test_edit_mutation.py` & `baseapp_pages-0.2.2/baseapp_pages/tests/test_edit_mutation.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/baseapp_pages/tests/test_get_queries.py` & `baseapp_pages-0.2.2/baseapp_pages/tests/test_get_queries.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/baseapp_pages/tests/test_list_queries.py` & `baseapp_pages-0.2.2/baseapp_pages/tests/test_list_queries.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/baseapp_pages.egg-info/PKG-INFO` & `baseapp_pages-0.2.2/baseapp_pages.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseapp-pages
-Version: 0.2.1
+Version: 0.2.2
 Summary: BaseApp Pages
 Home-page: https://github.com/silverlogic/baseapp-backend
 Author: The SilverLogic
 Author-email: dev@tsl.io
 License: BSD-3-Clause  # Example license
 Description: # BaseApp Pages
```

### Comparing `baseapp_pages-0.2.1/baseapp_pages.egg-info/SOURCES.txt` & `baseapp_pages-0.2.2/baseapp_pages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/setup.cfg` & `baseapp_pages-0.2.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [metadata]
 name = baseapp_pages
-version = 0.2.1
+version = 0.2.2
 description = BaseApp Pages
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/silverlogic/baseapp-backend
 author = The SilverLogic
 author_email = dev@tsl.io
 license = BSD-3-Clause  # Example license
 
 [options]
 include_package_data = true
 packages = find:
 python_requires = >=3.6
 install_requires = 
-	baseapp-core >= 0.2.9
+	baseapp-core >= 0.2.14
 	baseapp-comments >= 0.1.3
 	django-translated-fields >= 0.12
 	django-quill-editor >= 0.1
 
 [options.package_data]
 baseapp_pages = 
 	*.j2
```

### Comparing `baseapp_pages-0.2.1/testproject/graphql.py` & `baseapp_pages-0.2.2/testproject/graphql.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/testproject/settings.py` & `baseapp_pages-0.2.2/testproject/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # Application definition
 INSTALLED_APPS += [
     "graphene_django",
     "baseapp_pages",
     "django_quill",
     "baseapp_reactions",
     "baseapp_comments",
+    "baseapp_reports",
     "baseapp_auth",
     "testproject.testapp",
 ]
 
 ROOT_URLCONF = "testproject.urls"
 
 # Auth
```

### Comparing `baseapp_pages-0.2.1/testproject/testapp/migrations/0001_initial.py` & `baseapp_pages-0.2.2/testproject/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/testproject/testapp/migrations/0002_auto_20160321_1909.py` & `baseapp_pages-0.2.2/testproject/testapp/migrations/0002_auto_20160321_1909.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/testproject/testapp/migrations/0003_auto_20160725_2001.py` & `baseapp_pages-0.2.2/testproject/testapp/migrations/0003_auto_20160725_2001.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/testproject/testapp/migrations/0004_auto_20160811_1614.py` & `baseapp_pages-0.2.2/testproject/testapp/migrations/0004_auto_20160811_1614.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/testproject/testapp/migrations/0005_user_password_changed_date.py` & `baseapp_pages-0.2.2/testproject/testapp/migrations/0005_user_password_changed_date.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/testproject/testapp/migrations/0006_alter_user_id.py` & `baseapp_pages-0.2.2/testproject/testapp/migrations/0006_alter_user_id.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/testproject/testapp/migrations/0007_user_groups_user_is_staff_user_user_permissions.py` & `baseapp_pages-0.2.2/testproject/testapp/migrations/0007_user_groups_user_is_staff_user_user_permissions.py`

 * *Files identical despite different names*

### Comparing `baseapp_pages-0.2.1/testproject/testapp/migrations/0009_alter_user_options.py` & `baseapp_pages-0.2.2/testproject/testapp/migrations/0009_alter_user_options.py`

 * *Files identical despite different names*


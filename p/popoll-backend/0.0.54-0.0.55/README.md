# Comparing `tmp/popoll_backend-0.0.54.tar.gz` & `tmp/popoll_backend-0.0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popoll_backend-0.0.54.tar", last modified: Fri May 17 08:59:16 2024, max compression
+gzip compressed data, was "popoll_backend-0.0.55.tar", last modified: Mon May 20 21:07:56 2024, max compression
```

## Comparing `popoll_backend-0.0.54.tar` & `popoll_backend-0.0.55.tar`

### file list

```diff
@@ -1,81 +1,83 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:59:16.250701 popoll_backend-0.0.54/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-17 08:59:16.249701 popoll_backend-0.0.54/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:59:16.235701 popoll_backend-0.0.54/popoll_backend/
--rw-rw-rw-   0 root         (0) root         (0)     6971 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:59:16.236701 popoll_backend-0.0.54/popoll_backend/model/
--rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:59:16.238701 popoll_backend-0.0.54/popoll_backend/model/db/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/model/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      683 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/model/db/answer.py
--rw-rw-rw-   0 root         (0) root         (0)      798 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/model/db/date.py
--rw-rw-rw-   0 root         (0) root         (0)      394 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/model/db/instrument.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/model/db/option.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/model/db/session.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/model/db/user.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/model/db/user_instruments.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:59:16.240701 popoll_backend-0.0.54/popoll_backend/model/payload/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/model/payload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/model/payload/date_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/model/payload/dates_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/model/payload/history.py
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/model/payload/id_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/model/payload/instrument_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      276 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/model/payload/instruments_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      711 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/model/payload/user.py
--rw-rw-rw-   0 root         (0) root         (0)      957 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/model/payload/user_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/model/payload/users_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/model/payload/users_payload_details.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:59:16.245701 popoll_backend-0.0.54/popoll_backend/query/
--rw-rw-rw-   0 root         (0) root         (0)     2204 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1029 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/create_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/create_date.py
--rw-rw-rw-   0 root         (0) root         (0)      648 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/create_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)     1628 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/create_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      789 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/create_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1349 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/create_user.py
--rw-rw-rw-   0 root         (0) root         (0)      527 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/delete_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/delete_date.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/delete_user.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/get_answer.py
--rw-rw-rw-   0 root         (0) root         (0)     1796 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/get_date.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/get_dates.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/get_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      486 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/get_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/get_search_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/get_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/get_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1591 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/get_users.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/update_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      991 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/update_date.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/update_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     1415 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/popoll_backend/query/update_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:59:16.249701 popoll_backend-0.0.54/popoll_backend.egg-info/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-17 08:59:16.000000 popoll_backend-0.0.54/popoll_backend.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2556 2024-05-17 08:59:16.000000 popoll_backend-0.0.54/popoll_backend.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 08:59:16.000000 popoll_backend-0.0.54/popoll_backend.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-17 08:59:16.000000 popoll_backend-0.0.54/popoll_backend.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-17 08:59:16.000000 popoll_backend-0.0.54/popoll_backend.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-17 08:59:10.000000 popoll_backend-0.0.54/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 08:59:16.250701 popoll_backend-0.0.54/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:59:16.249701 popoll_backend-0.0.54/tests/
--rw-rw-rw-   0 root         (0) root         (0)      536 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/tests/test_01_db_creation.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/tests/test_02_simple_adds.py
--rw-rw-rw-   0 root         (0) root         (0)     1268 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/tests/test_03_no_duplicates.py
--rw-rw-rw-   0 root         (0) root         (0)     1668 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/tests/test_04_update_user_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     1927 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/tests/test_05_update_date_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     1201 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/tests/test_06_update_answer_entry.py
--rw-rw-rw-   0 root         (0) root         (0)      763 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/tests/test_07_delete_user_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/tests/test_08_delete_date_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     2328 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/tests/test_09_delete_user_date_entries.py
--rw-rw-rw-   0 root         (0) root         (0)     1378 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/tests/test_10_get_users.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/tests/test_11_get_users_sort_name.py
--rw-rw-rw-   0 root         (0) root         (0)     1248 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/tests/test_12_get_dates_sort_dateTime.py
--rw-rw-rw-   0 root         (0) root         (0)     2887 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/tests/test_13_history.py
--rw-rw-rw-   0 root         (0) root         (0)     2167 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/tests/test_14_get_answers_user.py
--rw-rw-rw-   0 root         (0) root         (0)     2403 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/tests/test_15_multi_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)     5145 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/tests/test_16_get_date.py
--rw-rw-rw-   0 root         (0) root         (0)      478 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/tests/test_17_get_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/tests/test_19_delete_database.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/tests/test_20_add_answer_no_dupe.py
--rw-rw-rw-   0 root         (0) root         (0)      863 2024-05-17 08:58:56.000000 popoll_backend-0.0.54/tests/test_21_get_dates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:07:56.784942 popoll_backend-0.0.55/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-20 21:07:56.783942 popoll_backend-0.0.55/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:07:56.767942 popoll_backend-0.0.55/popoll_backend/
+-rw-rw-rw-   0 root         (0) root         (0)     6748 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:07:56.768942 popoll_backend-0.0.55/popoll_backend/model/
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:07:56.770942 popoll_backend-0.0.55/popoll_backend/model/db/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/model/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      683 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/model/db/answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/model/db/date.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/model/db/instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/model/db/option.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/model/db/session.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/model/db/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/model/db/user_instruments.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:07:56.773942 popoll_backend-0.0.55/popoll_backend/model/payload/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/model/payload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/model/payload/date_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/model/payload/dates_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      730 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/model/payload/history.py
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/model/payload/id_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/model/payload/instrument_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      276 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/model/payload/instruments_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      711 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/model/payload/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      957 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/model/payload/user_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/model/payload/users_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/model/payload/users_payload_details.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:07:56.778942 popoll_backend-0.0.55/popoll_backend/query/
+-rw-rw-rw-   0 root         (0) root         (0)     2214 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1029 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/create_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/create_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/create_instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)     1470 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/create_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      789 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/create_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/create_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      527 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/delete_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/delete_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/delete_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/get_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1796 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/get_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/get_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      589 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/get_instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/get_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      486 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/get_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/get_search_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/get_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/get_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1591 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/get_users.py
+-rw-rw-rw-   0 root         (0) root         (0)      732 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/update_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      991 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/update_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/update_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/popoll_backend/query/update_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:07:56.783942 popoll_backend-0.0.55/popoll_backend.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-20 21:07:56.000000 popoll_backend-0.0.55/popoll_backend.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2627 2024-05-20 21:07:56.000000 popoll_backend-0.0.55/popoll_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 21:07:56.000000 popoll_backend-0.0.55/popoll_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-20 21:07:56.000000 popoll_backend-0.0.55/popoll_backend.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-20 21:07:56.000000 popoll_backend-0.0.55/popoll_backend.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-20 21:07:51.000000 popoll_backend-0.0.55/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 21:07:56.784942 popoll_backend-0.0.55/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:07:56.783942 popoll_backend-0.0.55/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_01_db_creation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_02_simple_adds.py
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_03_no_duplicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1668 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_04_update_user_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1927 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_05_update_date_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_06_update_answer_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)      763 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_07_delete_user_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_08_delete_date_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_09_delete_user_date_entries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1378 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_10_get_users.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_11_get_users_sort_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     1248 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_12_get_dates_sort_dateTime.py
+-rw-rw-rw-   0 root         (0) root         (0)     2887 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_13_history.py
+-rw-rw-rw-   0 root         (0) root         (0)     2167 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_14_get_answers_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     2403 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_15_multi_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)     5145 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_16_get_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      478 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_17_get_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_19_delete_database.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_20_add_answer_no_dupe.py
+-rw-rw-rw-   0 root         (0) root         (0)      863 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_21_get_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      453 2024-05-20 21:07:37.000000 popoll_backend-0.0.55/tests/test_22_add_instrument.py
```

### Comparing `popoll_backend-0.0.54/PKG-INFO` & `popoll_backend-0.0.55/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popoll_backend
-Version: 0.0.54
+Version: 0.0.55
 Summary: A small example package
 Author-email: vivi5421 <pypi@villard.me>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `popoll_backend-0.0.54/popoll_backend/__main__.py` & `popoll_backend-0.0.55/popoll_backend/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,19 +46,20 @@
     return _body[param] if mandatory else _body.get(param, default)
 
 
 
 def history(f):
     @wraps(f)
     def decorated(*args, **kwargs):
+        _poll = kwargs.get('poll')
         res = f(*args, **kwargs)
-        os.makedirs(os.path.join('.history', kwargs["poll"]), exist_ok=True)
+        os.makedirs(os.path.join('.history', _poll), exist_ok=True)
         logger = logging.getLogger('my_logger')
         logger.handlers.clear()
-        handler = logging.handlers.RotatingFileHandler(os.path.join('.history', kwargs["poll"], f'{kwargs["poll"]}.history.log'), maxBytes=1024*1024, backupCount=10)
+        handler = logging.handlers.RotatingFileHandler(os.path.join('.history', _poll, f'{_poll}.history.log'), maxBytes=1024*1024, backupCount=10)
         logger.addHandler(handler)
         logger.warning(json.dumps(History(flask.request, res, kwargs).toJSON()))
         return res
     return decorated
 
 
 class PollEndpoint(Resource):
@@ -68,20 +69,23 @@
     def post(self, poll:str): return CreatePoll(poll, body(flask.request, 'name', mandatory=False, default=poll), body(flask.request, 'instruments', mandatory=False, default=[]), body(flask.request, 'color', mandatory=False, default="#000000")).run()
     
     @history
     def put(self, poll:str): return UpdatePoll(poll, body(flask.request, 'name'), body(flask.request, 'color')).run()
     
     
     
+    
+    
 
 class InstrumentsEndpoint(Resource):
     def get(self, poll: str) -> Dict[str, Any]: return GetInstruments(poll).run()
     
     @history
-    def post(self, poll: str) -> int: return CreateInstrument(poll, body(flask.request, 'name')).run()
+    def post(self, poll: str) -> int: 
+        return CreateInstrument(poll, body(flask.request, 'name'), body(flask.request, 'rank')).run()
 
 
 
 
 
 
 
@@ -153,22 +157,14 @@
     def get(self, poll: str, id: str): return GetSession(poll, id).run()
     
     @history
     def post(self, poll: str, id: str): return CreateSession(poll, id, body(flask.request, 'user_id')).run()
 
 
 
-class GlobalInstrumentsEndpoint(Resource):
-    def get(self): return GetInstruments('__global').run()
-    
-    @history
-    def post(self) -> int: return CreateInstrument('__global', body(flask.request, 'name')).run()
-
-
-api.add_resource(GlobalInstrumentsEndpoint, '/instrument')
 
 api.add_resource(PollEndpoint, '/<string:poll>')
 api.add_resource(InstrumentsEndpoint, '/<string:poll>/instrument')
 api.add_resource(UsersEndpoint, '/<string:poll>/user')
 api.add_resource(UserEndpoint, '/<string:poll>/user/<int:id>')
 api.add_resource(DatesEndpoint, '/<string:poll>/date')
 api.add_resource(DateEndpoint, '/<string:poll>/date/<int:id>')
```

### Comparing `popoll_backend-0.0.54/popoll_backend/model/db/answer.py` & `popoll_backend-0.0.55/popoll_backend/model/db/answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/model/db/date.py` & `popoll_backend-0.0.55/popoll_backend/model/db/date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/model/db/session.py` & `popoll_backend-0.0.55/popoll_backend/model/db/session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/model/db/user_instruments.py` & `popoll_backend-0.0.55/popoll_backend/model/db/user_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/model/payload/date_payload.py` & `popoll_backend-0.0.55/popoll_backend/model/payload/date_payload.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/model/payload/history.py` & `popoll_backend-0.0.55/popoll_backend/model/payload/history.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/model/payload/user.py` & `popoll_backend-0.0.55/popoll_backend/model/payload/user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/model/payload/user_payload.py` & `popoll_backend-0.0.55/popoll_backend/model/payload/user_payload.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/query/__init__.py` & `popoll_backend-0.0.55/popoll_backend/query/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,29 +2,28 @@
 import os
 import sqlite3
 
 from typing import Type
 
 from popoll_backend.model import Payload
 
-
 class Query:
     
     fail_if_db_exists: bool = False
     fail_if_db_not_exists: bool = True
     
     def __init__(self, poll: str):
         self.poll = poll
         self.db_file = f'{poll}.db'
         if self.fail_if_db_exists and os.path.exists(self.db_file):
             flask.abort(409, f'The poll [{poll}] already exists.')
         if self.fail_if_db_not_exists and not os.path.exists(self.db_file):
             flask.abort(400, f'The poll [{poll}] does not exist.')
     
-    def run(self, cursor: sqlite3.Cursor=None):
+    def run(self, cursor: sqlite3.Cursor=None) -> Payload:
         if cursor:
             return self._run(cursor)
         else:
             with sqlite3.connect(self.db_file) as connection:
                 cursor: sqlite3.Cursor = connection.cursor()
                 cursor.execute("PRAGMA foreign_keys = ON")
                 cursor.execute("ATTACH DATABASE 'instruments.db' AS instruments;")
```

### Comparing `popoll_backend-0.0.54/popoll_backend/query/create_answer.py` & `popoll_backend-0.0.55/popoll_backend/query/create_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/query/create_date.py` & `popoll_backend-0.0.55/popoll_backend/query/create_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/query/create_instrument.py` & `popoll_backend-0.0.55/popoll_backend/query/create_instrument.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import sqlite3
 
 from popoll_backend.model import Payload
-from popoll_backend.model.payload.id_payload import IdPayload
 from popoll_backend.query import Query
+from popoll_backend.query.get_instrument import GetInstrument
 
 
 class CreateInstrument(Query):
     
-    name: str
     instrument_id: int
+    name: str
+    rank: int
     
-    def __init__(self, poll, name: str):
+    def __init__(self, poll: str, name: str, rank: int):
         super().__init__(poll)
         self.name = name
+        self.rank = rank
         
     def process(self, cursor: sqlite3.Cursor):
-        cursor.execute('INSERT INTO instruments.instruments(name) VALUES (?)', (self.name,))
+        cursor.execute('INSERT INTO instruments.instruments(name, rank) VALUES (?, ?)', (self.name, self.rank))
         self.instrument_id = cursor.lastrowid
         
     def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
-        return IdPayload(self.instrument_id)
+        return GetInstrument(self.poll, self.instrument_id).run(cursor)
```

### Comparing `popoll_backend-0.0.54/popoll_backend/query/create_poll.py` & `popoll_backend-0.0.55/popoll_backend/query/create_poll.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,16 +29,14 @@
         self.name = name
         self.instruments = instruments
         self.color = color
     
     def process(self, cursor: sqlite3.Cursor):
         cursor.execute(Option.create_table())
         cursor.execute('INSERT INTO options(name, color) values(?, ?)', (self.name, self.color))
-        # cursor.execute(Instrument.create_table())
-        # cursor.executemany('INSERT INTO instruments(name) values(?)', [(d,) for d in self.instruments])
         cursor.execute(Date.create_table())
         cursor.execute(User.create_table())
         cursor.execute(Answer.create_table())
         cursor.execute(UserInstruments.create_table())
         cursor.execute(Session.create_table())
     
     def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
```

### Comparing `popoll_backend-0.0.54/popoll_backend/query/create_session.py` & `popoll_backend-0.0.55/popoll_backend/query/create_session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/query/create_user.py` & `popoll_backend-0.0.55/popoll_backend/query/create_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/query/delete_answer.py` & `popoll_backend-0.0.55/popoll_backend/query/delete_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/query/delete_date.py` & `popoll_backend-0.0.55/popoll_backend/query/delete_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/query/delete_user.py` & `popoll_backend-0.0.55/popoll_backend/query/delete_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/query/get_answer.py` & `popoll_backend-0.0.55/popoll_backend/query/get_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/query/get_date.py` & `popoll_backend-0.0.55/popoll_backend/query/get_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/query/get_dates.py` & `popoll_backend-0.0.55/popoll_backend/query/get_dates.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/query/get_instruments.py` & `popoll_backend-0.0.55/popoll_backend/query/get_instruments.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import sqlite3
 from typing import List
 
-from popoll_backend.model import Payload
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.payload.instruments_payload import InstrumentsPayload
 from popoll_backend.query import Query
 
 
 class GetInstruments(Query):
     
     instruments: List[Instrument]
     
     def __init__(self, poll: str):
         super().__init__(poll)
     
     def process(self, cursor: sqlite3.Cursor):
-        self.instruments = [Instrument(row) for row in cursor.execute('SELECT * from instruments.instruments').fetchall()]
+        self.instruments = [Instrument(row) for row in cursor.execute('SELECT * from instruments.instruments ORDER BY rank').fetchall()]
         
-    def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
+    def buildResponse(self, cursor: sqlite3.Cursor) -> InstrumentsPayload:
         return InstrumentsPayload(self.instruments)
```

### Comparing `popoll_backend-0.0.54/popoll_backend/query/get_search_answer.py` & `popoll_backend-0.0.55/popoll_backend/query/get_search_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/query/get_session.py` & `popoll_backend-0.0.55/popoll_backend/query/get_session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/query/get_user.py` & `popoll_backend-0.0.55/popoll_backend/query/get_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/query/get_users.py` & `popoll_backend-0.0.55/popoll_backend/query/get_users.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/query/update_answer.py` & `popoll_backend-0.0.55/popoll_backend/query/update_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/query/update_date.py` & `popoll_backend-0.0.55/popoll_backend/query/update_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/query/update_poll.py` & `popoll_backend-0.0.55/popoll_backend/query/update_poll.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend/query/update_user.py` & `popoll_backend-0.0.55/popoll_backend/query/update_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/popoll_backend.egg-info/PKG-INFO` & `popoll_backend-0.0.55/popoll_backend.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popoll_backend
-Version: 0.0.54
+Version: 0.0.55
 Summary: A small example package
 Author-email: vivi5421 <pypi@villard.me>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `popoll_backend-0.0.54/popoll_backend.egg-info/SOURCES.txt` & `popoll_backend-0.0.55/popoll_backend.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 popoll_backend/query/create_user.py
 popoll_backend/query/delete_answer.py
 popoll_backend/query/delete_date.py
 popoll_backend/query/delete_user.py
 popoll_backend/query/get_answer.py
 popoll_backend/query/get_date.py
 popoll_backend/query/get_dates.py
+popoll_backend/query/get_instrument.py
 popoll_backend/query/get_instruments.py
 popoll_backend/query/get_poll.py
 popoll_backend/query/get_search_answer.py
 popoll_backend/query/get_session.py
 popoll_backend/query/get_user.py
 popoll_backend/query/get_users.py
 popoll_backend/query/update_answer.py
@@ -64,8 +65,9 @@
 tests/test_13_history.py
 tests/test_14_get_answers_user.py
 tests/test_15_multi_instruments.py
 tests/test_16_get_date.py
 tests/test_17_get_instruments.py
 tests/test_19_delete_database.py
 tests/test_20_add_answer_no_dupe.py
-tests/test_21_get_dates.py
+tests/test_21_get_dates.py
+tests/test_22_add_instrument.py
```

### Comparing `popoll_backend-0.0.54/pyproject.toml` & `popoll_backend-0.0.55/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", 'wheel', 'flask', 'flask_cors', 'flask-restful', 'jsonpickle', 'sqlalchemy', 'sqlalchemy-utils', 'psycopg2-binary', 'pyyaml', 'pyopenssl']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "popoll_backend"
-version = "0.0.54"
+version = "0.0.55"
 authors = [
   { name="vivi5421", email="pypi@villard.me" },
 ]
 description = "A small example package"
 readme = "README.md"
 license = { file = "LICENSE" }
 dependencies = [
```

### Comparing `popoll_backend-0.0.54/tests/test_01_db_creation.py` & `popoll_backend-0.0.55/tests/test_01_db_creation.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/tests/test_02_simple_adds.py` & `popoll_backend-0.0.55/tests/test_02_simple_adds.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/tests/test_03_no_duplicates.py` & `popoll_backend-0.0.55/tests/test_03_no_duplicates.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/tests/test_04_update_user_entry.py` & `popoll_backend-0.0.55/tests/test_04_update_user_entry.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/tests/test_05_update_date_entry.py` & `popoll_backend-0.0.55/tests/test_05_update_date_entry.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/tests/test_06_update_answer_entry.py` & `popoll_backend-0.0.55/tests/test_06_update_answer_entry.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/tests/test_07_delete_user_entry.py` & `popoll_backend-0.0.55/tests/test_07_delete_user_entry.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/tests/test_08_delete_date_entry.py` & `popoll_backend-0.0.55/tests/test_08_delete_date_entry.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/tests/test_09_delete_user_date_entries.py` & `popoll_backend-0.0.55/tests/test_09_delete_user_date_entries.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/tests/test_10_get_users.py` & `popoll_backend-0.0.55/tests/test_10_get_users.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/tests/test_11_get_users_sort_name.py` & `popoll_backend-0.0.55/tests/test_11_get_users_sort_name.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/tests/test_12_get_dates_sort_dateTime.py` & `popoll_backend-0.0.55/tests/test_12_get_dates_sort_dateTime.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/tests/test_13_history.py` & `popoll_backend-0.0.55/tests/test_13_history.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/tests/test_14_get_answers_user.py` & `popoll_backend-0.0.55/tests/test_14_get_answers_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/tests/test_15_multi_instruments.py` & `popoll_backend-0.0.55/tests/test_15_multi_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/tests/test_16_get_date.py` & `popoll_backend-0.0.55/tests/test_16_get_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/tests/test_20_add_answer_no_dupe.py` & `popoll_backend-0.0.55/tests/test_20_add_answer_no_dupe.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.54/tests/test_21_get_dates.py` & `popoll_backend-0.0.55/tests/test_21_get_dates.py`

 * *Files identical despite different names*


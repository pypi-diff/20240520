# Comparing `tmp/gypsum_client-0.0.1.tar.gz` & `tmp/gypsum_client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gypsum_client-0.0.1.tar", last modified: Tue May  7 20:02:42 2024, max compression
+gzip compressed data, was "gypsum_client-0.1.0.tar", last modified: Mon May 20 00:32:01 2024, max compression
```

## Comparing `gypsum_client-0.0.1.tar` & `gypsum_client-0.1.0.tar`

### file list

```diff
@@ -1,46 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:42.270593 gypsum_client-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:42.258593 gypsum_client-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:42.262593 gypsum_client-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-07 20:02:42.270593 gypsum_client-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:42.266593 gypsum_client-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:42.266593 gypsum_client-0.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-07 20:02:42.270593 gypsum_client-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:42.258593 gypsum_client-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:42.266593 gypsum_client-0.0.1/src/gypsum_client/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/src/gypsum_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/src/gypsum_client/skeleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:42.266593 gypsum_client-0.0.1/src/gypsum_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-07 20:02:42.000000 gypsum_client-0.0.1/src/gypsum_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-07 20:02:42.000000 gypsum_client-0.0.1/src/gypsum_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:02:42.000000 gypsum_client-0.0.1/src/gypsum_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:02:42.000000 gypsum_client-0.0.1/src/gypsum_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-07 20:02:42.000000 gypsum_client-0.0.1/src/gypsum_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-07 20:02:42.000000 gypsum_client-0.0.1/src/gypsum_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:42.266593 gypsum_client-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/tests/test_skeleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-07 20:01:58.000000 gypsum_client-0.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:32:01.119734 gypsum_client-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:32:01.103734 gypsum_client-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:32:01.107734 gypsum_client-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-20 00:32:01.119734 gypsum_client-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:32:01.107734 gypsum_client-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:32:01.107734 gypsum_client-0.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-20 00:32:01.119734 gypsum_client-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:32:01.103734 gypsum_client-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:32:01.111734 gypsum_client-0.1.0/src/gypsum_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/clone_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/create_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/fetch_metadata_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/fetch_metadata_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/fetch_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/list_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/prepare_directory_for_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/probation_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/refresh_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/remove_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/resolve_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/s3_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/save_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/search_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/set_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/upload_api_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/upload_file_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/src/gypsum_client/validate_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:32:01.119734 gypsum_client-0.1.0/src/gypsum_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-20 00:32:01.000000 gypsum_client-0.1.0/src/gypsum_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-20 00:32:01.000000 gypsum_client-0.1.0/src/gypsum_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 00:32:01.000000 gypsum_client-0.1.0/src/gypsum_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 00:32:00.000000 gypsum_client-0.1.0/src/gypsum_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-20 00:32:01.000000 gypsum_client-0.1.0/src/gypsum_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 00:32:01.000000 gypsum_client-0.1.0/src/gypsum_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:32:01.119734 gypsum_client-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/tests/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/tests/test_fetch_metadata_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/tests/test_fetch_metadata_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/tests/test_latest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/tests/test_prepare_dir_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/tests/test_probation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/tests/test_quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/tests/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-20 00:30:34.000000 gypsum_client-0.1.0/tox.ini
```

### Comparing `gypsum_client-0.0.1/.coveragerc` & `gypsum_client-0.1.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.0.1/.github/workflows/pypi-publish.yml` & `gypsum_client-0.1.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.0.1/.github/workflows/pypi-test.yml` & `gypsum_client-0.1.0/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.0.1/.gitignore` & `gypsum_client-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.0.1/.pre-commit-config.yaml` & `gypsum_client-0.1.0/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -34,22 +34,32 @@
 #       --remove-all-unused-imports,
 #       --remove-unused-variables,
 #     ]
 
 - repo: https://github.com/PyCQA/isort
   rev: 5.13.2
   hooks:
-  - id: isort
+    - id: docformatter
+      additional_dependencies: [tomli]
+      args: [--in-place, --wrap-descriptions=120, --wrap-summaries=120]
+      # --config, ./pyproject.toml
 
 - repo: https://github.com/psf/black
   rev: 24.4.2
   hooks:
   - id: black
     language_version: python3
 
+- repo: https://github.com/astral-sh/ruff-pre-commit
+  # Ruff version.
+  rev: v0.3.7
+  hooks:
+    - id: ruff
+      args: [--fix, --exit-non-zero-on-fix]
+
 ## If like to embrace black styles even in the docs:
 # - repo: https://github.com/asottile/blacken-docs
 #   rev: v1.13.0
 #   hooks:
 #   - id: blacken-docs
 #     additional_dependencies: [black]
 
@@ -60,8 +70,8 @@
   ## You can add flake8 plugins via `additional_dependencies`:
   #  additional_dependencies: [flake8-bugbear]
 
 ## Check for misspells in documentation files:
 # - repo: https://github.com/codespell-project/codespell
 #   rev: v2.2.5
 #   hooks:
-#   - id: codespell
+#   - id: codespell
```

### Comparing `gypsum_client-0.0.1/.readthedocs.yml` & `gypsum_client-0.1.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.0.1/CONTRIBUTING.md` & `gypsum_client-0.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.0.1/LICENSE.txt` & `gypsum_client-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.0.1/PKG-INFO` & `gypsum_client-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,41 @@
-Metadata-Version: 2.1
-Name: gypsum-client
-Version: 0.0.1
-Summary: Add a short description here!
-Home-page: https://github.com/pyscaffold/pyscaffold/
-Author: Jayaram Kancherla
-Author-email: jayaram.kancherla@gmail.com
-License: MIT
-Project-URL: Documentation, https://pyscaffold.org/
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-License-File: LICENSE.txt
-Requires-Dist: importlib-metadata; python_version < "3.8"
-Provides-Extra: testing
-Requires-Dist: setuptools; extra == "testing"
-Requires-Dist: pytest; extra == "testing"
-Requires-Dist: pytest-cov; extra == "testing"
-
 <!-- These are examples of badges you might want to add to your README:
      please update the URLs accordingly
 
 [![Built Status](https://api.cirrus-ci.com/github/<USER>/gypsum-client.svg?branch=main)](https://cirrus-ci.com/github/<USER>/gypsum-client)
 [![ReadTheDocs](https://readthedocs.org/projects/gypsum-client/badge/?version=latest)](https://gypsum-client.readthedocs.io/en/stable/)
 [![Coveralls](https://img.shields.io/coveralls/github/<USER>/gypsum-client/main.svg)](https://coveralls.io/r/<USER>/gypsum-client)
-[![PyPI-Server](https://img.shields.io/pypi/v/gypsum-client.svg)](https://pypi.org/project/gypsum-client/)
+
 [![Conda-Forge](https://img.shields.io/conda/vn/conda-forge/gypsum-client.svg)](https://anaconda.org/conda-forge/gypsum-client)
-[![Monthly Downloads](https://pepy.tech/badge/gypsum-client/month)](https://pepy.tech/project/gypsum-client)
+
 [![Twitter](https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter)](https://twitter.com/gypsum-client)
 -->
 
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
+[![PyPI-Server](https://img.shields.io/pypi/v/gypsum-client.svg)](https://pypi.org/project/gypsum-client/)
+
+# Python client to the gypsum REST API
+
+
+The `gypsum_client` package provides the Python client to any instance of the [gypsum REST API](https://gypsum.artifactdb.com). This allows client (both in **R** and **Python**) packages to easily store and retrieve resources from the **gypsum** backend.
+It also provides mechanisms to allow package maintainers to easily manage upload authorizations and third-party contributions.
+
+Readers are referred to [API's documentation](https://github.com/ArtifactDB/gypsum-worker) for a description of the concepts; this guide will strictly focus on the usage of the `gypsum_client` package.
+
+**Note: check out the R/Bioconductor package for the gypsum REST API [here](https://github.com/ArtifactDB/gypsum-R).**
 
-# gypsum-client
+## Installation
 
-> Add a short description here!
+Package is published to [PyPI](https://pypi.org/project/gypsum-client/),
 
-A longer description of your project goes here...
+```sh
+pip install gypsum_client
+```
 
+Check out the [documentation](https://artifactdb.github.io/gypsum-py/) for more information.
 
 <!-- pyscaffold-notes -->
 
 ## Note
 
 This project has been set up using PyScaffold 4.5. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `gypsum_client-0.0.1/docs/Makefile` & `gypsum_client-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.0.1/docs/conf.py` & `gypsum_client-0.1.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     "sphinx.ext.autosummary",
     "sphinx.ext.viewcode",
     "sphinx.ext.coverage",
     "sphinx.ext.doctest",
     "sphinx.ext.ifconfig",
     "sphinx.ext.mathjax",
     "sphinx.ext.napoleon",
+    "sphinx_autodoc_typehints",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 
 # Enable markdown
@@ -162,20 +163,30 @@
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
 # keep_warnings = False
 
 # If this is True, todo emits a warning for each TODO entries. The default is False.
 todo_emit_warnings = True
 
+autodoc_default_options = {
+    # 'members': 'var1, var2',
+    # 'member-order': 'bysource',
+    "special-members": True,
+    "undoc-members": True,
+    "exclude-members": "__weakref__, __dict__, __str__, __module__",
+}
+
+autosummary_generate = True
+autosummary_imported_members = True
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = "alabaster"
+html_theme = "furo"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 html_theme_options = {
     "sidebar_width": "300px",
     "page_width": "1200px"
```

### Comparing `gypsum_client-0.0.1/setup.cfg` & `gypsum_client-0.1.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 [metadata]
 name = gypsum-client
-description = Add a short description here!
+description = Python cline to gypsum
 author = Jayaram Kancherla
 author_email = jayaram.kancherla@gmail.com
 license = MIT
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
-url = https://github.com/pyscaffold/pyscaffold/
+url = https://github.com/ArtifactDB/gypsum-py
 project_urls = 
-	Documentation = https://pyscaffold.org/
+	Documentation = https://github.com/ArtifactDB/gypsum-py
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
 
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
+python_requires = >=3.8
 install_requires = 
 	importlib-metadata; python_version<"3.8"
+	requests
+	filelock
+	jsonschema
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `gypsum_client-0.0.1/setup.py` & `gypsum_client-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.0.1/src/gypsum_client.egg-info/PKG-INFO` & `gypsum_client-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,65 @@
 Metadata-Version: 2.1
 Name: gypsum-client
-Version: 0.0.1
-Summary: Add a short description here!
-Home-page: https://github.com/pyscaffold/pyscaffold/
+Version: 0.1.0
+Summary: Python cline to gypsum
+Home-page: https://github.com/ArtifactDB/gypsum-py
 Author: Jayaram Kancherla
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
-Project-URL: Documentation, https://pyscaffold.org/
+Project-URL: Documentation, https://github.com/ArtifactDB/gypsum-py
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: requests
+Requires-Dist: filelock
+Requires-Dist: jsonschema
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 <!-- These are examples of badges you might want to add to your README:
      please update the URLs accordingly
 
 [![Built Status](https://api.cirrus-ci.com/github/<USER>/gypsum-client.svg?branch=main)](https://cirrus-ci.com/github/<USER>/gypsum-client)
 [![ReadTheDocs](https://readthedocs.org/projects/gypsum-client/badge/?version=latest)](https://gypsum-client.readthedocs.io/en/stable/)
 [![Coveralls](https://img.shields.io/coveralls/github/<USER>/gypsum-client/main.svg)](https://coveralls.io/r/<USER>/gypsum-client)
-[![PyPI-Server](https://img.shields.io/pypi/v/gypsum-client.svg)](https://pypi.org/project/gypsum-client/)
+
 [![Conda-Forge](https://img.shields.io/conda/vn/conda-forge/gypsum-client.svg)](https://anaconda.org/conda-forge/gypsum-client)
-[![Monthly Downloads](https://pepy.tech/badge/gypsum-client/month)](https://pepy.tech/project/gypsum-client)
+
 [![Twitter](https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter)](https://twitter.com/gypsum-client)
 -->
 
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
+[![PyPI-Server](https://img.shields.io/pypi/v/gypsum-client.svg)](https://pypi.org/project/gypsum-client/)
+
+# Python client to the gypsum REST API
+
+
+The `gypsum_client` package provides the Python client to any instance of the [gypsum REST API](https://gypsum.artifactdb.com). This allows client (both in **R** and **Python**) packages to easily store and retrieve resources from the **gypsum** backend.
+It also provides mechanisms to allow package maintainers to easily manage upload authorizations and third-party contributions.
+
+Readers are referred to [API's documentation](https://github.com/ArtifactDB/gypsum-worker) for a description of the concepts; this guide will strictly focus on the usage of the `gypsum_client` package.
+
+**Note: check out the R/Bioconductor package for the gypsum REST API [here](https://github.com/ArtifactDB/gypsum-R).**
 
-# gypsum-client
+## Installation
 
-> Add a short description here!
+Package is published to [PyPI](https://pypi.org/project/gypsum-client/),
 
-A longer description of your project goes here...
+```sh
+pip install gypsum_client
+```
 
+Check out the [documentation](https://artifactdb.github.io/gypsum-py/) for more information.
 
 <!-- pyscaffold-notes -->
 
 ## Note
 
 This project has been set up using PyScaffold 4.5. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `gypsum_client-0.0.1/tox.ini` & `gypsum_client-0.1.0/tox.ini`

 * *Files identical despite different names*


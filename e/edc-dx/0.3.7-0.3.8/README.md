# Comparing `tmp/edc-dx-0.3.7.tar.gz` & `tmp/edc_dx-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-dx-0.3.7.tar", last modified: Tue Mar 26 04:54:38 2024, max compression
+gzip compressed data, was "edc_dx-0.3.8.tar", last modified: Mon May 20 16:32:38 2024, max compression
```

## Comparing `edc-dx-0.3.7.tar` & `edc_dx-0.3.8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 04:54:38.203112 edc-dx-0.3.7/
--rw-r--r--   0 erikvw     (501) staff       (20)       78 2022-05-25 02:35:41.000000 edc-dx-0.3.7/.coveragrc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-25 02:35:41.000000 edc-dx-0.3.7/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 04:54:38.192213 edc-dx-0.3.7/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 04:54:38.195843 edc-dx-0.3.7/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2091 2024-03-08 05:54:42.000000 edc-dx-0.3.7/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-05-25 02:35:41.000000 edc-dx-0.3.7/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2024-03-08 05:54:42.000000 edc-dx-0.3.7/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-11 23:24:19.000000 edc-dx-0.3.7/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 02:35:41.000000 edc-dx-0.3.7/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2022-05-25 02:35:41.000000 edc-dx-0.3.7/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-07-07 03:33:10.000000 edc-dx-0.3.7/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      110 2023-10-09 19:55:45.000000 edc-dx-0.3.7/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1748 2024-03-26 04:54:38.203037 edc-dx-0.3.7/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      923 2023-12-14 05:31:22.000000 edc-dx-0.3.7/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-11 23:24:19.000000 edc-dx-0.3.7/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 04:54:38.196765 edc-dx-0.3.7/dx_app/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-04-18 01:09:08.000000 edc-dx-0.3.7/dx_app/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2023-04-18 01:09:08.000000 edc-dx-0.3.7/dx_app/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      544 2024-03-08 05:54:42.000000 edc-dx-0.3.7/dx_app/consents.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 04:54:38.197009 edc-dx-0.3.7/dx_app/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-04-18 01:09:08.000000 edc-dx-0.3.7/dx_app/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6301 2024-03-26 04:54:29.000000 edc-dx-0.3.7/dx_app/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2427 2024-01-24 05:33:37.000000 edc-dx-0.3.7/dx_app/visit_schedule.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 04:54:38.197777 edc-dx-0.3.7/edc_dx/
--rw-r--r--   0 erikvw     (501) staff       (20)      229 2022-10-26 02:34:21.000000 edc-dx-0.3.7/edc_dx/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      109 2022-05-25 02:35:41.000000 edc-dx-0.3.7/edc_dx/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9244 2023-04-18 01:09:08.000000 edc-dx-0.3.7/edc_dx/diagnoses.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 04:54:38.199383 edc-dx-0.3.7/edc_dx/form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)      138 2022-11-29 05:49:58.000000 edc-dx-0.3.7/edc_dx/form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1925 2023-05-24 17:07:52.000000 edc-dx-0.3.7/edc_dx/form_validators/diagnosis_form_validator_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2492 2023-05-24 17:07:52.000000 edc-dx-0.3.7/edc_dx/form_validators/result_form_validator_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 04:54:38.200392 edc-dx-0.3.7/edc_dx/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 02:35:41.000000 edc-dx-0.3.7/edc_dx/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      605 2023-04-18 01:09:08.000000 edc-dx-0.3.7/edc_dx/tests/baker_recipes.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 04:54:38.201596 edc-dx-0.3.7/edc_dx/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 02:35:41.000000 edc-dx-0.3.7/edc_dx/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 02:35:41.000000 edc-dx-0.3.7/edc_dx/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-25 02:35:41.000000 edc-dx-0.3.7/edc_dx/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-25 02:35:41.000000 edc-dx-0.3.7/edc_dx/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-25 02:35:41.000000 edc-dx-0.3.7/edc_dx/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-25 02:35:41.000000 edc-dx-0.3.7/edc_dx/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 02:35:41.000000 edc-dx-0.3.7/edc_dx/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 02:35:41.000000 edc-dx-0.3.7/edc_dx/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      542 2023-05-24 17:07:52.000000 edc-dx-0.3.7/edc_dx/tests/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)      508 2022-05-25 02:35:41.000000 edc-dx-0.3.7/edc_dx/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)     3027 2024-01-24 05:33:37.000000 edc-dx-0.3.7/edc_dx/tests/test_case_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 04:54:38.202446 edc-dx-0.3.7/edc_dx/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-04-17 11:19:20.000000 edc-dx-0.3.7/edc_dx/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7942 2023-04-18 01:09:08.000000 edc-dx-0.3.7/edc_dx/tests/tests/test_diagnoses.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8570 2024-01-24 05:33:37.000000 edc-dx-0.3.7/edc_dx/tests/tests/test_forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)      566 2022-05-25 02:35:41.000000 edc-dx-0.3.7/edc_dx/tests/tests/test_labels.py
--rw-r--r--   0 erikvw     (501) staff       (20)      252 2022-05-25 02:35:41.000000 edc-dx-0.3.7/edc_dx/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1579 2023-07-10 03:46:43.000000 edc-dx-0.3.7/edc_dx/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 04:54:38.202734 edc-dx-0.3.7/edc_dx.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1748 2024-03-26 04:54:38.000000 edc-dx-0.3.7/edc_dx.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1314 2024-03-26 04:54:38.000000 edc-dx-0.3.7/edc_dx.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-03-26 04:54:38.000000 edc-dx-0.3.7/edc_dx.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-07-09 17:35:39.000000 edc-dx-0.3.7/edc_dx.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       14 2024-03-26 04:54:38.000000 edc-dx-0.3.7/edc_dx.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1706 2023-12-14 05:31:22.000000 edc-dx-0.3.7/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2445 2023-12-14 18:21:36.000000 edc-dx-0.3.7/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1127 2024-03-26 04:54:38.203443 edc-dx-0.3.7/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:32:38.701468 edc_dx-0.3.8/
+-rw-r--r--   0 erikvw     (501) staff       (20)       78 2022-05-25 02:35:41.000000 edc_dx-0.3.8/.coveragrc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-25 02:35:41.000000 edc_dx-0.3.8/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:32:38.689871 edc_dx-0.3.8/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:32:38.693874 edc_dx-0.3.8/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2091 2024-03-08 05:54:42.000000 edc_dx-0.3.8/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-05-25 02:35:41.000000 edc_dx-0.3.8/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2024-03-08 05:54:42.000000 edc_dx-0.3.8/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-11 23:24:19.000000 edc_dx-0.3.8/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 02:35:41.000000 edc_dx-0.3.8/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2022-05-25 02:35:41.000000 edc_dx-0.3.8/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-07-07 03:33:10.000000 edc_dx-0.3.8/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      110 2023-10-09 19:55:45.000000 edc_dx-0.3.8/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1748 2024-05-20 16:32:38.701395 edc_dx-0.3.8/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      923 2023-12-14 05:31:22.000000 edc_dx-0.3.8/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-11 23:24:19.000000 edc_dx-0.3.8/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:32:38.695122 edc_dx-0.3.8/dx_app/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-04-18 01:09:08.000000 edc_dx-0.3.8/dx_app/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2023-04-18 01:09:08.000000 edc_dx-0.3.8/dx_app/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      544 2024-03-08 05:54:42.000000 edc_dx-0.3.8/dx_app/consents.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:32:38.695392 edc_dx-0.3.8/dx_app/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-04-18 01:09:08.000000 edc_dx-0.3.8/dx_app/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6301 2024-03-26 04:54:29.000000 edc_dx-0.3.8/dx_app/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2427 2024-01-24 05:33:37.000000 edc_dx-0.3.8/dx_app/visit_schedule.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:32:38.696292 edc_dx-0.3.8/edc_dx/
+-rw-r--r--   0 erikvw     (501) staff       (20)      229 2022-10-26 02:34:21.000000 edc_dx-0.3.8/edc_dx/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      109 2022-05-25 02:35:41.000000 edc_dx-0.3.8/edc_dx/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9071 2024-05-20 16:32:30.000000 edc_dx-0.3.8/edc_dx/diagnoses.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:32:38.697875 edc_dx-0.3.8/edc_dx/form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)      138 2022-11-29 05:49:58.000000 edc_dx-0.3.8/edc_dx/form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1925 2024-04-30 11:10:47.000000 edc_dx-0.3.8/edc_dx/form_validators/diagnosis_form_validator_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2492 2023-05-24 17:07:52.000000 edc_dx-0.3.8/edc_dx/form_validators/result_form_validator_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:32:38.698963 edc_dx-0.3.8/edc_dx/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 02:35:41.000000 edc_dx-0.3.8/edc_dx/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      605 2023-04-18 01:09:08.000000 edc_dx-0.3.8/edc_dx/tests/baker_recipes.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:32:38.700129 edc_dx-0.3.8/edc_dx/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 02:35:41.000000 edc_dx-0.3.8/edc_dx/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 02:35:41.000000 edc_dx-0.3.8/edc_dx/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-25 02:35:41.000000 edc_dx-0.3.8/edc_dx/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-25 02:35:41.000000 edc_dx-0.3.8/edc_dx/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-25 02:35:41.000000 edc_dx-0.3.8/edc_dx/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-25 02:35:41.000000 edc_dx-0.3.8/edc_dx/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 02:35:41.000000 edc_dx-0.3.8/edc_dx/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 02:35:41.000000 edc_dx-0.3.8/edc_dx/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      542 2023-05-24 17:07:52.000000 edc_dx-0.3.8/edc_dx/tests/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      508 2022-05-25 02:35:41.000000 edc_dx-0.3.8/edc_dx/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)     3027 2024-01-24 05:33:37.000000 edc_dx-0.3.8/edc_dx/tests/test_case_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:32:38.700911 edc_dx-0.3.8/edc_dx/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-04-17 11:19:20.000000 edc_dx-0.3.8/edc_dx/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7942 2023-04-18 01:09:08.000000 edc_dx-0.3.8/edc_dx/tests/tests/test_diagnoses.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8570 2024-01-24 05:33:37.000000 edc_dx-0.3.8/edc_dx/tests/tests/test_forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      566 2022-05-25 02:35:41.000000 edc_dx-0.3.8/edc_dx/tests/tests/test_labels.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      252 2022-05-25 02:35:41.000000 edc_dx-0.3.8/edc_dx/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1579 2023-07-10 03:46:43.000000 edc_dx-0.3.8/edc_dx/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:32:38.701106 edc_dx-0.3.8/edc_dx.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1748 2024-05-20 16:32:38.000000 edc_dx-0.3.8/edc_dx.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1314 2024-05-20 16:32:38.000000 edc_dx-0.3.8/edc_dx.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-05-20 16:32:38.000000 edc_dx-0.3.8/edc_dx.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-07-09 17:35:39.000000 edc_dx-0.3.8/edc_dx.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2024-05-20 16:32:38.000000 edc_dx-0.3.8/edc_dx.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1706 2023-12-14 05:31:22.000000 edc_dx-0.3.8/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2445 2023-12-14 18:21:36.000000 edc_dx-0.3.8/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1127 2024-05-20 16:32:38.701789 edc_dx-0.3.8/setup.cfg
```

### Comparing `edc-dx-0.3.7/.github/workflows/build.yml` & `edc_dx-0.3.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/.gitignore` & `edc_dx-0.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/.pre-commit-config.yaml` & `edc_dx-0.3.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/LICENSE` & `edc_dx-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/PKG-INFO` & `edc_dx-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-dx
-Version: 0.3.7
+Version: 0.3.8
 Summary: Classes to manage review of HIV, DM and HTN diagnoses for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-dx
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc diagnosis,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-dx-0.3.7/README.rst` & `edc_dx-0.3.8/README.rst`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/dx_app/consents.py` & `edc_dx-0.3.8/dx_app/consents.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/dx_app/models.py` & `edc_dx-0.3.8/dx_app/models.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/dx_app/visit_schedule.py` & `edc_dx-0.3.8/dx_app/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/edc_dx/diagnoses.py` & `edc_dx-0.3.8/edc_dx/diagnoses.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from edc_constants.constants import YES
 from edc_dx_review.utils import (
     get_clinical_review_baseline_model_cls,
     get_clinical_review_model_cls,
     get_initial_review_model_cls,
 )
 
-from .utils import get_diagnosis_labels, get_diagnosis_labels_prefixes
+from .utils import get_diagnosis_labels
 
 
 class InitialReviewRequired(Exception):
     pass
 
 
 class MultipleInitialReviewsExist(Exception):
@@ -75,21 +75,17 @@
     def get_dx_by_model(self, instance) -> str:
         dx = None
         for prefix in self.diagnosis_labels:
             if instance.__class__.__name__.lower().startswith(prefix.lower()):
                 dx = self.get_dx(prefix)
                 break
         if not dx:
-            models_classes = [
-                get_initial_review_model_cls(prefix)
-                for prefix in get_diagnosis_labels_prefixes()
-            ]
             raise DiagnosesError(
-                f"Invalid. Expected an instance of one of {models_classes}. "
-                f"Got {instance.__class__}"
+                f"Invalid. No diagnoses detected. "
+                f"See responses on {self.clinical_review_baseline._meta.verbose_name}."
             )
         return dx
 
     def get_dx_date(self, prefix: str) -> date | None:
         """Returns a dx date from the initial review for the condition.
 
         Raises if initial review does not exist."""
```

### Comparing `edc-dx-0.3.7/edc_dx/form_validators/diagnosis_form_validator_mixin.py` & `edc_dx-0.3.8/edc_dx/form_validators/diagnosis_form_validator_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/edc_dx/form_validators/result_form_validator_mixin.py` & `edc_dx-0.3.8/edc_dx/form_validators/result_form_validator_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/edc_dx/tests/baker_recipes.py` & `edc_dx-0.3.8/edc_dx/tests/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/edc_dx/tests/etc/user-rsa-local-private.pem` & `edc_dx-0.3.8/edc_dx/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/edc_dx/tests/etc/user-rsa-restricted-private.pem` & `edc_dx-0.3.8/edc_dx/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/edc_dx/tests/forms.py` & `edc_dx-0.3.8/edc_dx/tests/forms.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/edc_dx/tests/test_case_mixin.py` & `edc_dx-0.3.8/edc_dx/tests/test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/edc_dx/tests/tests/test_diagnoses.py` & `edc_dx-0.3.8/edc_dx/tests/tests/test_diagnoses.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/edc_dx/tests/tests/test_forms.py` & `edc_dx-0.3.8/edc_dx/tests/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/edc_dx/tests/tests/test_labels.py` & `edc_dx-0.3.8/edc_dx/tests/tests/test_labels.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/edc_dx/utils.py` & `edc_dx-0.3.8/edc_dx/utils.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/edc_dx.egg-info/PKG-INFO` & `edc_dx-0.3.8/edc_dx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-dx
-Version: 0.3.7
+Version: 0.3.8
 Summary: Classes to manage review of HIV, DM and HTN diagnoses for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-dx
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc diagnosis,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-dx-0.3.7/edc_dx.egg-info/SOURCES.txt` & `edc_dx-0.3.8/edc_dx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/pyproject.toml` & `edc_dx-0.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/runtests.py` & `edc_dx-0.3.8/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.3.7/setup.cfg` & `edc_dx-0.3.8/setup.cfg`

 * *Files identical despite different names*


# Comparing `tmp/edc-glucose-0.3.6.tar.gz` & `tmp/edc_glucose-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-glucose-0.3.6.tar", last modified: Tue Mar 26 05:01:18 2024, max compression
+gzip compressed data, was "edc_glucose-0.3.7.tar", last modified: Mon May 20 16:37:00 2024, max compression
```

## Comparing `edc-glucose-0.3.6.tar` & `edc_glucose-0.3.7.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:01:18.065902 edc-glucose-0.3.6/
--rw-r--r--   0 erikvw     (501) staff       (20)       93 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/.coveragrc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:01:18.053740 edc-glucose-0.3.6/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:01:18.057561 edc-glucose-0.3.6/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2091 2024-03-08 06:00:56.000000 edc-glucose-0.3.6/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1844 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2024-03-08 06:00:56.000000 edc-glucose-0.3.6/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-11 23:52:58.000000 edc-glucose-0.3.6/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)      107 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-07-01 21:36:03.000000 edc-glucose-0.3.6/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      110 2023-09-22 02:26:00.000000 edc-glucose-0.3.6/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1511 2024-03-26 05:01:18.065832 edc-glucose-0.3.6/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      680 2023-12-15 02:59:50.000000 edc-glucose-0.3.6/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-11 23:52:58.000000 edc-glucose-0.3.6/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:01:18.058604 edc-glucose-0.3.6/edc_glucose/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/edc_glucose/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      147 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/edc_glucose/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      112 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/edc_glucose/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)      364 2023-04-25 02:08:11.000000 edc-glucose-0.3.6/edc_glucose/fieldsets.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:01:18.061321 edc-glucose-0.3.6/edc_glucose/form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)      378 2023-06-20 14:24:57.000000 edc-glucose-0.3.6/edc_glucose/form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      429 2022-09-26 21:07:54.000000 edc-glucose-0.3.6/edc_glucose/form_validators/fasting_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      986 2023-06-20 14:24:57.000000 edc-glucose-0.3.6/edc_glucose/form_validators/fbg_form_validator_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2006 2022-09-26 21:07:54.000000 edc-glucose-0.3.6/edc_glucose/form_validators/fbg_ogtt_form_validator_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1449 2023-05-24 16:07:07.000000 edc-glucose-0.3.6/edc_glucose/form_validators/glucose_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2174 2023-09-22 02:26:00.000000 edc-glucose-0.3.6/edc_glucose/form_validators/glucose_form_validator_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3235 2022-09-26 21:07:54.000000 edc-glucose-0.3.6/edc_glucose/form_validators/ogtt_form_validator_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:01:18.061571 edc-glucose-0.3.6/edc_glucose/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/edc_glucose/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:01:18.062829 edc-glucose-0.3.6/edc_glucose/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      317 2022-10-26 14:45:42.000000 edc-glucose-0.3.6/edc_glucose/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1874 2024-01-30 05:18:59.000000 edc-glucose-0.3.6/edc_glucose/model_mixins/fasting_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1527 2022-08-19 14:56:08.000000 edc-glucose-0.3.6/edc_glucose/model_mixins/fbg_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1722 2023-04-25 02:08:11.000000 edc-glucose-0.3.6/edc_glucose/model_mixins/glucose_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      942 2022-08-19 14:56:08.000000 edc-glucose-0.3.6/edc_glucose/model_mixins/hba1c_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2243 2022-08-19 14:56:08.000000 edc-glucose-0.3.6/edc_glucose/model_mixins/ogtt_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/edc_glucose/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:01:18.063615 edc-glucose-0.3.6/edc_glucose/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/edc_glucose/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      549 2024-03-08 06:00:56.000000 edc-glucose-0.3.6/edc_glucose/tests/consents.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:01:18.064967 edc-glucose-0.3.6/edc_glucose/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/edc_glucose/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/edc_glucose/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/edc_glucose/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/edc_glucose/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/edc_glucose/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/edc_glucose/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/edc_glucose/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/edc_glucose/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1378 2024-03-26 05:01:09.000000 edc-glucose-0.3.6/edc_glucose/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:01:18.065222 edc-glucose-0.3.6/edc_glucose/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/edc_glucose/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6511 2024-01-24 06:30:35.000000 edc-glucose-0.3.6/edc_glucose/tests/tests/test_glucose_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      257 2022-06-02 01:34:00.000000 edc-glucose-0.3.6/edc_glucose/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1685 2024-01-24 06:30:35.000000 edc-glucose-0.3.6/edc_glucose/tests/visit_schedules.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1248 2022-09-26 21:07:54.000000 edc-glucose-0.3.6/edc_glucose/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:01:18.065548 edc-glucose-0.3.6/edc_glucose.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1511 2024-03-26 05:01:18.000000 edc-glucose-0.3.6/edc_glucose.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1823 2024-03-26 05:01:18.000000 edc-glucose-0.3.6/edc_glucose.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-03-26 05:01:18.000000 edc-glucose-0.3.6/edc_glucose.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-07-01 21:43:04.000000 edc-glucose-0.3.6/edc_glucose.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       12 2024-03-26 05:01:18.000000 edc-glucose-0.3.6/edc_glucose.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1716 2023-12-15 02:59:50.000000 edc-glucose-0.3.6/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1086 2024-01-29 05:35:47.000000 edc-glucose-0.3.6/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1139 2024-03-26 05:01:18.066204 edc-glucose-0.3.6/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:37:00.340441 edc_glucose-0.3.7/
+-rw-r--r--   0 erikvw     (501) staff       (20)       93 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/.coveragrc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:37:00.328330 edc_glucose-0.3.7/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:37:00.332397 edc_glucose-0.3.7/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2091 2024-03-08 06:00:56.000000 edc_glucose-0.3.7/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1844 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2024-03-08 06:00:56.000000 edc_glucose-0.3.7/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-11 23:52:58.000000 edc_glucose-0.3.7/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)      107 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-07-01 21:36:03.000000 edc_glucose-0.3.7/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      110 2023-09-22 02:26:00.000000 edc_glucose-0.3.7/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1511 2024-05-20 16:37:00.340363 edc_glucose-0.3.7/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      680 2023-12-15 02:59:50.000000 edc_glucose-0.3.7/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-11 23:52:58.000000 edc_glucose-0.3.7/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:37:00.333440 edc_glucose-0.3.7/edc_glucose/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/edc_glucose/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      147 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/edc_glucose/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      112 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/edc_glucose/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      364 2023-04-25 02:08:11.000000 edc_glucose-0.3.7/edc_glucose/fieldsets.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:37:00.335950 edc_glucose-0.3.7/edc_glucose/form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)      378 2023-06-20 14:24:57.000000 edc_glucose-0.3.7/edc_glucose/form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      429 2022-09-26 21:07:54.000000 edc_glucose-0.3.7/edc_glucose/form_validators/fasting_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      986 2023-06-20 14:24:57.000000 edc_glucose-0.3.7/edc_glucose/form_validators/fbg_form_validator_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2006 2022-09-26 21:07:54.000000 edc_glucose-0.3.7/edc_glucose/form_validators/fbg_ogtt_form_validator_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1449 2023-05-24 16:07:07.000000 edc_glucose-0.3.7/edc_glucose/form_validators/glucose_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2174 2023-09-22 02:26:00.000000 edc_glucose-0.3.7/edc_glucose/form_validators/glucose_form_validator_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3235 2022-09-26 21:07:54.000000 edc_glucose-0.3.7/edc_glucose/form_validators/ogtt_form_validator_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:37:00.336156 edc_glucose-0.3.7/edc_glucose/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/edc_glucose/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:37:00.337275 edc_glucose-0.3.7/edc_glucose/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      317 2022-10-26 14:45:42.000000 edc_glucose-0.3.7/edc_glucose/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2296 2024-05-20 16:36:51.000000 edc_glucose-0.3.7/edc_glucose/model_mixins/fasting_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1527 2022-08-19 14:56:08.000000 edc_glucose-0.3.7/edc_glucose/model_mixins/fbg_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1741 2024-05-20 16:36:51.000000 edc_glucose-0.3.7/edc_glucose/model_mixins/glucose_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      942 2022-08-19 14:56:08.000000 edc_glucose-0.3.7/edc_glucose/model_mixins/hba1c_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2243 2022-08-19 14:56:08.000000 edc_glucose-0.3.7/edc_glucose/model_mixins/ogtt_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/edc_glucose/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:37:00.338185 edc_glucose-0.3.7/edc_glucose/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/edc_glucose/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      549 2024-03-08 06:00:56.000000 edc_glucose-0.3.7/edc_glucose/tests/consents.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:37:00.339476 edc_glucose-0.3.7/edc_glucose/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/edc_glucose/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/edc_glucose/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/edc_glucose/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/edc_glucose/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/edc_glucose/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/edc_glucose/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/edc_glucose/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/edc_glucose/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1378 2024-03-26 05:01:09.000000 edc_glucose-0.3.7/edc_glucose/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:37:00.339730 edc_glucose-0.3.7/edc_glucose/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/edc_glucose/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6511 2024-01-24 06:30:35.000000 edc_glucose-0.3.7/edc_glucose/tests/tests/test_glucose_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      257 2022-06-02 01:34:00.000000 edc_glucose-0.3.7/edc_glucose/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1685 2024-01-24 06:30:35.000000 edc_glucose-0.3.7/edc_glucose/tests/visit_schedules.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1318 2024-05-20 16:36:51.000000 edc_glucose-0.3.7/edc_glucose/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:37:00.340057 edc_glucose-0.3.7/edc_glucose.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1511 2024-05-20 16:37:00.000000 edc_glucose-0.3.7/edc_glucose.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1823 2024-05-20 16:37:00.000000 edc_glucose-0.3.7/edc_glucose.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-05-20 16:37:00.000000 edc_glucose-0.3.7/edc_glucose.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-07-01 21:43:04.000000 edc_glucose-0.3.7/edc_glucose.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       12 2024-05-20 16:37:00.000000 edc_glucose-0.3.7/edc_glucose.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1716 2023-12-15 02:59:50.000000 edc_glucose-0.3.7/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1086 2024-01-29 05:35:47.000000 edc_glucose-0.3.7/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1139 2024-05-20 16:37:00.340772 edc_glucose-0.3.7/setup.cfg
```

### Comparing `edc-glucose-0.3.6/.github/workflows/build.yml` & `edc_glucose-0.3.7/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/.gitignore` & `edc_glucose-0.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/.pre-commit-config.yaml` & `edc_glucose-0.3.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/LICENSE` & `edc_glucose-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/PKG-INFO` & `edc_glucose-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-glucose
-Version: 0.3.6
+Version: 0.3.7
 Summary: Classes to collect glucose, FBG, OGTT in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-glucose
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc glucose FBG / OGTT,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-glucose-0.3.6/README.rst` & `edc_glucose-0.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/edc_glucose/form_validators/fbg_form_validator_mixin.py` & `edc_glucose-0.3.7/edc_glucose/form_validators/fbg_form_validator_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/edc_glucose/form_validators/fbg_ogtt_form_validator_mixin.py` & `edc_glucose-0.3.7/edc_glucose/form_validators/fbg_ogtt_form_validator_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/edc_glucose/form_validators/glucose_form_validator.py` & `edc_glucose-0.3.7/edc_glucose/form_validators/glucose_form_validator.py`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/edc_glucose/form_validators/glucose_form_validator_mixin.py` & `edc_glucose-0.3.7/edc_glucose/form_validators/glucose_form_validator_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/edc_glucose/form_validators/ogtt_form_validator_mixin.py` & `edc_glucose-0.3.7/edc_glucose/form_validators/ogtt_form_validator_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/edc_glucose/model_mixins/fasting_model_mixin.py` & `edc_glucose-0.3.7/edc_glucose/model_mixins/fasting_model_mixin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from __future__ import annotations
 
 from django.db import models
 from edc_constants.choices import YES_NO_NA
 from edc_constants.constants import NOT_APPLICABLE
+from edc_model.utils import duration_hm_to_timedelta
 from edc_model.validators import hm_validator
 
 
 def fasting_model_mixin_factory(
     prefix: str = None, verbose_names: dict | None = None, **kwargs
 ):
     prefix = "" if prefix is None else f"{prefix}_"
     verbose_names = verbose_names or {}
 
     class AbstractModel(models.Model):
+        def save(self, *args, **kwargs):
+            if duration_str := getattr(self, f"{prefix}fasting_duration_str", None):
+                tdelta = duration_hm_to_timedelta(duration_str)
+                setattr(self, f"{prefix}fasting_duration_delta", tdelta)
+            super().save(*args, **kwargs)
+
         class Meta:
             abstract = True
 
     opts = {
         f"{prefix}fasting": models.CharField(
             verbose_name=verbose_names.get(f"{prefix}fasting", "Has the participant fasted?"),
             max_length=15,
@@ -35,16 +42,18 @@
             null=True,
             blank=True,
             help_text=(
                 "As reported by patient. Duration of fast. Format is `HHhMMm`. "
                 "For example 1h23m, 12h7m, etc"
             ),
         ),
-        f"{prefix}fasting_duration_minutes": models.IntegerField(
-            null=True, blank=True, help_text="system calculated value"
+        f"{prefix}fasting_duration_delta": models.DurationField(
+            null=True,
+            blank=True,
+            help_text="system calculated to microseconds. (hours=microseconds/3.6e+9)",
         ),
     }
 
     opts.update(**kwargs)
 
     for name, fld_cls in opts.items():
         AbstractModel.add_to_class(name, fld_cls)
```

### Comparing `edc-glucose-0.3.6/edc_glucose/model_mixins/fbg_model_mixin.py` & `edc_glucose-0.3.7/edc_glucose/model_mixins/fbg_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/edc_glucose/model_mixins/glucose_model_mixin.py` & `edc_glucose-0.3.7/edc_glucose/model_mixins/glucose_model_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from django.db import models
 from edc_constants.constants import NOT_APPLICABLE
 from edc_lab.choices import GLUCOSE_UNITS_NA, RESULT_QUANTIFIER_NA
 
 from ..constants import GLUCOSE_HIGH_READING
-from . import fasting_model_mixin_factory
+from .fasting_model_mixin import fasting_model_mixin_factory
 
 
 def glucose_model_mixin_factory(utest_id: str, verbose_names: dict | None = None, **kwargs):
     class AbstractModel(models.Model):
         class Meta:
             abstract = True
```

### Comparing `edc-glucose-0.3.6/edc_glucose/model_mixins/hba1c_model_mixin.py` & `edc_glucose-0.3.7/edc_glucose/model_mixins/hba1c_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/edc_glucose/model_mixins/ogtt_model_mixin.py` & `edc_glucose-0.3.7/edc_glucose/model_mixins/ogtt_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/edc_glucose/tests/consents.py` & `edc_glucose-0.3.7/edc_glucose/tests/consents.py`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/edc_glucose/tests/etc/user-rsa-local-private.pem` & `edc_glucose-0.3.7/edc_glucose/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/edc_glucose/tests/etc/user-rsa-restricted-private.pem` & `edc_glucose-0.3.7/edc_glucose/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/edc_glucose/tests/models.py` & `edc_glucose-0.3.7/edc_glucose/tests/models.py`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/edc_glucose/tests/tests/test_glucose_form_validator.py` & `edc_glucose-0.3.7/edc_glucose/tests/tests/test_glucose_form_validator.py`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/edc_glucose/tests/visit_schedules.py` & `edc_glucose-0.3.7/edc_glucose/tests/visit_schedules.py`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/edc_glucose/utils.py` & `edc_glucose-0.3.7/edc_glucose/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 from django import forms
 from edc_reportable import MILLIMOLES_PER_LITER, ConversionNotHandled, convert_units
 from edc_utils.round_up import round_half_away_from_zero
 
 from .constants import GLUCOSE_HIGH_READING
 
 
-def validate_glucose_as_millimoles_per_liter(prefix: str, cleaned_data: dict = None) -> None:
+def validate_glucose_as_millimoles_per_liter(
+    prefix: str, cleaned_data: dict = None
+) -> None | Decimal:
+    converted_value = None
     min_val = Decimal("0.00")
     max_val = Decimal("30.00")
     high_value = Decimal(f"{GLUCOSE_HIGH_READING}")
     value = cleaned_data.get(f"{prefix}_value")
     units = cleaned_data.get(f"{prefix}_units")
     if value and units:
         try:
@@ -27,7 +30,8 @@
             raise forms.ValidationError(
                 {
                     f"{prefix}_value": (
                         f"This value is out-of-range. Got {converted_value} mmol/L"
                     )
                 }
             )
+    return converted_value
```

### Comparing `edc-glucose-0.3.6/edc_glucose.egg-info/PKG-INFO` & `edc_glucose-0.3.7/edc_glucose.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-glucose
-Version: 0.3.6
+Version: 0.3.7
 Summary: Classes to collect glucose, FBG, OGTT in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-glucose
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc glucose FBG / OGTT,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-glucose-0.3.6/edc_glucose.egg-info/SOURCES.txt` & `edc_glucose-0.3.7/edc_glucose.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/pyproject.toml` & `edc_glucose-0.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/runtests.py` & `edc_glucose-0.3.7/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-glucose-0.3.6/setup.cfg` & `edc_glucose-0.3.7/setup.cfg`

 * *Files identical despite different names*


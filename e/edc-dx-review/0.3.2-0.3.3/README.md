# Comparing `tmp/edc-dx-review-0.3.2.tar.gz` & `tmp/edc_dx_review-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-dx-review-0.3.2.tar", last modified: Thu Dec 14 05:37:21 2023, max compression
+gzip compressed data, was "edc_dx_review-0.3.3.tar", last modified: Mon May 20 16:34:55 2024, max compression
```

## Comparing `edc-dx-review-0.3.2.tar` & `edc_dx_review-0.3.3.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-12-14 05:37:21.904297 edc-dx-review-0.3.2/
--rw-r--r--   0 erikvw     (501) staff       (20)       99 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/.coveragrc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-12-14 05:37:21.888951 edc-dx-review-0.3.2/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-12-14 05:37:21.892548 edc-dx-review-0.3.2/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2091 2023-12-14 05:37:13.000000 edc-dx-review-0.3.2/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-05-07 01:16:31.000000 edc-dx-review-0.3.2/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-10-09 22:11:28.000000 edc-dx-review-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-11 23:26:19.000000 edc-dx-review-0.3.2/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 01:16:31.000000 edc-dx-review-0.3.2/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2022-05-07 01:16:31.000000 edc-dx-review-0.3.2/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-07-06 02:08:29.000000 edc-dx-review-0.3.2/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      110 2023-10-09 22:11:28.000000 edc-dx-review-0.3.2/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1826 2023-12-14 05:37:21.904226 edc-dx-review-0.3.2/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      984 2023-12-14 05:37:13.000000 edc-dx-review-0.3.2/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-11 23:26:19.000000 edc-dx-review-0.3.2/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-12-14 05:37:21.894764 edc-dx-review-0.3.2/edc_dx_review/
--rw-r--r--   0 erikvw     (501) staff       (20)       79 2022-10-26 02:35:15.000000 edc-dx-review-0.3.2/edc_dx_review/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      116 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/edc_dx_review/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      521 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/edc_dx_review/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      360 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/edc_dx_review/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)      643 2023-08-03 14:19:52.000000 edc-dx-review-0.3.2/edc_dx_review/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      204 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/edc_dx_review/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1276 2023-04-22 19:35:59.000000 edc-dx-review-0.3.2/edc_dx_review/fieldsets.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-12-14 05:37:21.895717 edc-dx-review-0.3.2/edc_dx_review/form_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      112 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/edc_dx_review/form_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      942 2023-08-10 17:15:33.000000 edc-dx-review-0.3.2/edc_dx_review/form_mixins/clinical_review_baseline_required_form_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-12-14 05:37:21.896335 edc-dx-review-0.3.2/edc_dx_review/form_validator_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      218 2023-04-05 03:26:58.000000 edc-dx-review-0.3.2/edc_dx_review/form_validator_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      226 2023-04-20 02:00:22.000000 edc-dx-review-0.3.2/edc_dx_review/form_validator_mixins/clinical_review_baseline_form_validator_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1097 2023-04-17 23:24:37.000000 edc-dx-review-0.3.2/edc_dx_review/form_validator_mixins/clinical_review_followup_form_validator_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      711 2022-11-29 04:36:47.000000 edc-dx-review-0.3.2/edc_dx_review/list_data.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6907 2023-04-20 03:28:55.000000 edc-dx-review-0.3.2/edc_dx_review/medical_date.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-12-14 05:37:21.897813 edc-dx-review-0.3.2/edc_dx_review/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    11691 2023-03-31 02:16:40.000000 edc-dx-review-0.3.2/edc_dx_review/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      965 2023-08-03 14:19:52.000000 edc-dx-review-0.3.2/edc_dx_review/migrations/0002_diagnosislocations_extra_value_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5011 2023-12-05 03:08:13.000000 edc-dx-review-0.3.2/edc_dx_review/migrations/0003_alter_diagnosislocations_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      524 2023-12-05 03:08:13.000000 edc-dx-review-0.3.2/edc_dx_review/migrations/0004_remove_diagnosislocations_edc_dx_revi_name_a39b40_idx_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/edc_dx_review/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-12-14 05:37:21.898335 edc-dx-review-0.3.2/edc_dx_review/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      700 2023-04-17 23:24:37.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      926 2023-04-17 23:24:37.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/clinical_review_baseline_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-12-14 05:37:21.899242 edc-dx-review-0.3.2/edc_dx_review/model_mixins/clinical_review_followup/
--rw-r--r--   0 erikvw     (501) staff       (20)      403 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/clinical_review_followup/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1511 2023-03-31 02:16:40.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/clinical_review_followup/clinical_review_followup_chol_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1478 2023-03-31 02:16:40.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/clinical_review_followup/clinical_review_followup_dm_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1505 2023-03-31 02:16:40.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/clinical_review_followup/clinical_review_followup_hiv_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1502 2023-03-31 02:16:40.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/clinical_review_followup/clinical_review_followup_htn_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      892 2023-04-17 23:24:37.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/clinical_review_followup/clinical_review_followup_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      425 2023-03-31 02:16:40.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/dx_location_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-12-14 05:37:21.900592 edc-dx-review-0.3.2/edc_dx_review/model_mixins/factory/
--rw-r--r--   0 erikvw     (501) staff       (20)      348 2023-04-17 23:24:37.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/factory/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1746 2023-04-20 02:00:22.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/factory/baseline_review_model_mixin_factory.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1526 2023-04-17 23:24:37.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/factory/calculate_date.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3222 2023-08-10 17:15:33.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/factory/dx_initial_review_model_mixin_factory.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1246 2023-04-19 02:56:59.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/factory/followup_review_model_mixin_factory.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2376 2023-04-25 02:10:14.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/factory/rx_initial_review_model_mixin_factory.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-12-14 05:37:21.901192 edc-dx-review-0.3.2/edc_dx_review/model_mixins/followup_review/
--rw-r--r--   0 erikvw     (501) staff       (20)      139 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/followup_review/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      673 2023-03-31 02:16:40.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/followup_review/followup_review_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1034 2023-03-31 02:16:40.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/followup_review/hiv_followup_review_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-12-14 05:37:21.901735 edc-dx-review-0.3.2/edc_dx_review/model_mixins/initial_review/
--rw-r--r--   0 erikvw     (501) staff       (20)      250 2023-04-17 23:24:37.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/initial_review/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1000 2023-04-17 23:24:37.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/initial_review/chol_initial_review_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3641 2023-03-31 02:16:40.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/initial_review/hiv_initial_model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1192 2023-03-31 02:16:40.000000 edc-dx-review-0.3.2/edc_dx_review/model_mixins/initial_review/ncd_initial_review_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      610 2022-11-29 04:36:47.000000 edc-dx-review-0.3.2/edc_dx_review/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)      833 2023-04-20 02:00:22.000000 edc-dx-review-0.3.2/edc_dx_review/radio_fields.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-12-14 05:37:21.901964 edc-dx-review-0.3.2/edc_dx_review/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/edc_dx_review/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-12-14 05:37:21.903376 edc-dx-review-0.3.2/edc_dx_review/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/edc_dx_review/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/edc_dx_review/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/edc_dx_review/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/edc_dx_review/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/edc_dx_review/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/edc_dx_review/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/edc_dx_review/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/edc_dx_review/tests/etc/user-salt-restricted.key
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-12-14 05:37:21.903601 edc-dx-review-0.3.2/edc_dx_review/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 01:09:57.000000 edc-dx-review-0.3.2/edc_dx_review/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7748 2023-04-20 03:28:55.000000 edc-dx-review-0.3.2/edc_dx_review/tests/tests/test_medical_date.py
--rw-r--r--   0 erikvw     (501) staff       (20)      259 2023-03-31 02:17:23.000000 edc-dx-review-0.3.2/edc_dx_review/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6700 2023-08-10 17:15:33.000000 edc-dx-review-0.3.2/edc_dx_review/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-12-14 05:37:21.903924 edc-dx-review-0.3.2/edc_dx_review.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1826 2023-12-14 05:37:21.000000 edc-dx-review-0.3.2/edc_dx_review.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     3480 2023-12-14 05:37:21.000000 edc-dx-review-0.3.2/edc_dx_review.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-12-14 05:37:21.000000 edc-dx-review-0.3.2/edc_dx_review.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-07-09 17:35:53.000000 edc-dx-review-0.3.2/edc_dx_review.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       14 2023-12-14 05:37:21.000000 edc-dx-review-0.3.2/edc_dx_review.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1720 2023-12-14 05:37:13.000000 edc-dx-review-0.3.2/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2336 2023-12-14 05:37:13.000000 edc-dx-review-0.3.2/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1149 2023-12-14 05:37:21.904617 edc-dx-review-0.3.2/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:34:55.452773 edc_dx_review-0.3.3/
+-rw-r--r--   0 erikvw     (501) staff       (20)       99 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/.coveragrc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:34:55.435956 edc_dx_review-0.3.3/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:34:55.440250 edc_dx_review-0.3.3/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2091 2024-05-20 16:34:47.000000 edc_dx_review-0.3.3/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-05-07 01:16:31.000000 edc_dx_review-0.3.3/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2024-05-20 16:34:47.000000 edc_dx_review-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-11 23:26:19.000000 edc_dx_review-0.3.3/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 01:16:31.000000 edc_dx_review-0.3.3/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2022-05-07 01:16:31.000000 edc_dx_review-0.3.3/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-07-06 02:08:29.000000 edc_dx_review-0.3.3/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      110 2023-10-09 22:11:28.000000 edc_dx_review-0.3.3/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1826 2024-05-20 16:34:55.452698 edc_dx_review-0.3.3/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      984 2023-12-14 05:37:13.000000 edc_dx_review-0.3.3/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-11 23:26:19.000000 edc_dx_review-0.3.3/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:34:55.442791 edc_dx_review-0.3.3/edc_dx_review/
+-rw-r--r--   0 erikvw     (501) staff       (20)       79 2022-10-26 02:35:15.000000 edc_dx_review-0.3.3/edc_dx_review/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      116 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/edc_dx_review/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      521 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/edc_dx_review/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      360 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/edc_dx_review/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      643 2023-08-03 14:19:52.000000 edc_dx_review-0.3.3/edc_dx_review/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      204 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/edc_dx_review/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1276 2023-04-22 19:35:59.000000 edc_dx_review-0.3.3/edc_dx_review/fieldsets.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:34:55.443733 edc_dx_review-0.3.3/edc_dx_review/form_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      112 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/edc_dx_review/form_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      942 2023-08-10 17:15:33.000000 edc_dx_review-0.3.3/edc_dx_review/form_mixins/clinical_review_baseline_required_form_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:34:55.444427 edc_dx_review-0.3.3/edc_dx_review/form_validator_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      218 2023-04-05 03:26:58.000000 edc_dx_review-0.3.3/edc_dx_review/form_validator_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      226 2023-04-20 02:00:22.000000 edc_dx_review-0.3.3/edc_dx_review/form_validator_mixins/clinical_review_baseline_form_validator_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1097 2023-04-17 23:24:37.000000 edc_dx_review-0.3.3/edc_dx_review/form_validator_mixins/clinical_review_followup_form_validator_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      711 2022-11-29 04:36:47.000000 edc_dx_review-0.3.3/edc_dx_review/list_data.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6907 2023-04-20 03:28:55.000000 edc_dx_review-0.3.3/edc_dx_review/medical_date.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:34:55.446451 edc_dx_review-0.3.3/edc_dx_review/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    11691 2023-03-31 02:16:40.000000 edc_dx_review-0.3.3/edc_dx_review/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      965 2023-08-03 14:19:52.000000 edc_dx_review-0.3.3/edc_dx_review/migrations/0002_diagnosislocations_extra_value_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5011 2023-12-05 03:08:13.000000 edc_dx_review-0.3.3/edc_dx_review/migrations/0003_alter_diagnosislocations_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      524 2023-12-05 03:08:13.000000 edc_dx_review-0.3.3/edc_dx_review/migrations/0004_remove_diagnosislocations_edc_dx_revi_name_a39b40_idx_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/edc_dx_review/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:34:55.447010 edc_dx_review-0.3.3/edc_dx_review/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      700 2023-04-17 23:24:37.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      926 2023-04-17 23:24:37.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/clinical_review_baseline_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:34:55.448104 edc_dx_review-0.3.3/edc_dx_review/model_mixins/clinical_review_followup/
+-rw-r--r--   0 erikvw     (501) staff       (20)      403 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/clinical_review_followup/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1511 2023-03-31 02:16:40.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/clinical_review_followup/clinical_review_followup_chol_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1478 2023-03-31 02:16:40.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/clinical_review_followup/clinical_review_followup_dm_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1505 2023-03-31 02:16:40.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/clinical_review_followup/clinical_review_followup_hiv_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1502 2023-03-31 02:16:40.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/clinical_review_followup/clinical_review_followup_htn_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      892 2023-04-17 23:24:37.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/clinical_review_followup/clinical_review_followup_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      425 2023-03-31 02:16:40.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/dx_location_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:34:55.449247 edc_dx_review-0.3.3/edc_dx_review/model_mixins/factory/
+-rw-r--r--   0 erikvw     (501) staff       (20)      348 2023-04-17 23:24:37.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/factory/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1746 2023-04-20 02:00:22.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/factory/baseline_review_model_mixin_factory.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1526 2023-04-17 23:24:37.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/factory/calculate_date.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3222 2023-08-10 17:15:33.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/factory/dx_initial_review_model_mixin_factory.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1246 2023-04-19 02:56:59.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/factory/followup_review_model_mixin_factory.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2376 2023-04-25 02:10:14.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/factory/rx_initial_review_model_mixin_factory.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:34:55.449850 edc_dx_review-0.3.3/edc_dx_review/model_mixins/followup_review/
+-rw-r--r--   0 erikvw     (501) staff       (20)      139 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/followup_review/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      673 2023-03-31 02:16:40.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/followup_review/followup_review_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1034 2023-03-31 02:16:40.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/followup_review/hiv_followup_review_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:34:55.450435 edc_dx_review-0.3.3/edc_dx_review/model_mixins/initial_review/
+-rw-r--r--   0 erikvw     (501) staff       (20)      250 2023-04-17 23:24:37.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/initial_review/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1000 2023-04-17 23:24:37.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/initial_review/chol_initial_review_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3641 2023-03-31 02:16:40.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/initial_review/hiv_initial_model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1192 2023-03-31 02:16:40.000000 edc_dx_review-0.3.3/edc_dx_review/model_mixins/initial_review/ncd_initial_review_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      610 2022-11-29 04:36:47.000000 edc_dx_review-0.3.3/edc_dx_review/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      833 2023-04-20 02:00:22.000000 edc_dx_review-0.3.3/edc_dx_review/radio_fields.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:34:55.450675 edc_dx_review-0.3.3/edc_dx_review/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/edc_dx_review/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:34:55.451959 edc_dx_review-0.3.3/edc_dx_review/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/edc_dx_review/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/edc_dx_review/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/edc_dx_review/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/edc_dx_review/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/edc_dx_review/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/edc_dx_review/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/edc_dx_review/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/edc_dx_review/tests/etc/user-salt-restricted.key
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:34:55.452195 edc_dx_review-0.3.3/edc_dx_review/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 01:09:57.000000 edc_dx_review-0.3.3/edc_dx_review/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7748 2023-04-20 03:28:55.000000 edc_dx_review-0.3.3/edc_dx_review/tests/tests/test_medical_date.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      259 2023-03-31 02:17:23.000000 edc_dx_review-0.3.3/edc_dx_review/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6985 2024-05-20 16:34:47.000000 edc_dx_review-0.3.3/edc_dx_review/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-05-20 16:34:55.452404 edc_dx_review-0.3.3/edc_dx_review.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1826 2024-05-20 16:34:55.000000 edc_dx_review-0.3.3/edc_dx_review.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     3480 2024-05-20 16:34:55.000000 edc_dx_review-0.3.3/edc_dx_review.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-05-20 16:34:55.000000 edc_dx_review-0.3.3/edc_dx_review.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-07-09 17:35:53.000000 edc_dx_review-0.3.3/edc_dx_review.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2024-05-20 16:34:55.000000 edc_dx_review-0.3.3/edc_dx_review.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1720 2023-12-14 05:37:13.000000 edc_dx_review-0.3.3/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2336 2023-12-14 05:37:13.000000 edc_dx_review-0.3.3/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1149 2024-05-20 16:34:55.453101 edc_dx_review-0.3.3/setup.cfg
```

### Comparing `edc-dx-review-0.3.2/.github/workflows/build.yml` & `edc_dx_review-0.3.3/.github/workflows/build.yml`

 * *Files 5% similar despite different names*

```diff
@@ -32,27 +32,27 @@
     steps:
       - name: Install pycups and words dependency
         run: |
           sudo sed -i 's/azure\.//' /etc/apt/sources.list
           sudo apt-get -y update
           sudo apt-get install libcups2-dev wamerican
 
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Get pip cache dir
         id: pip-cache
         run: |
           echo "dir=$(pip cache dir)" >>$GITHUB_OUTPUT
 
       - name: Cache
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         with:
           path: ${{ steps.pip-cache.outputs.dir }}
           key:
             ${{ matrix.python-version }}-v1-${{ hashFiles('**/setup.py') }}-${{ hashFiles('**/tox.ini') }}
           restore-keys: |
             ${{ matrix.python-version }}-v1-
```

### Comparing `edc-dx-review-0.3.2/.gitignore` & `edc_dx_review-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/.pre-commit-config.yaml` & `edc_dx_review-0.3.3/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 ---
 exclude: tests/etc/user-*
 
 repos:
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.5
+    rev: 1.7.7
     hooks:
       - id: bandit
         args:
           - "-x *test*.py"
 
   - repo: https://github.com/psf/black
-    rev: 23.9.1
+    rev: 24.2.0
     hooks:
       - id: black
         language_version: python3.11
 
   - repo: https://github.com/pycqa/flake8
-    rev: 6.1.0
+    rev: 7.0.0
     hooks:
       - id: flake8
         args:
           - "--config=setup.cfg"
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
+    rev: 5.13.2
     hooks:
       - id: isort
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.5.0
     hooks:
       - id: requirements-txt-fixer
         files: requirements/.*\.txt$
       - id: trailing-whitespace
       - id: check-added-large-files
       - id: fix-byte-order-marker
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
       - id: detect-private-key
 
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.32.0
+    rev: v1.34.0
     hooks:
       - id: yamllint
         args:
           - "--strict"
```

### Comparing `edc-dx-review-0.3.2/LICENSE` & `edc_dx_review-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/PKG-INFO` & `edc_dx_review-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-dx-review
-Version: 0.3.2
+Version: 0.3.3
 Summary: Classes to manage review of HIV, DM and HTN diagnoses for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-dx-review
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django glucose ifg ogtt clinicedc clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-dx-review-0.3.2/README.rst` & `edc_dx_review-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/auth_objects.py` & `edc_dx_review-0.3.3/edc_dx_review/auth_objects.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/choices.py` & `edc_dx_review-0.3.3/edc_dx_review/choices.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/fieldsets.py` & `edc_dx_review-0.3.3/edc_dx_review/fieldsets.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/form_mixins/clinical_review_baseline_required_form_mixin.py` & `edc_dx_review-0.3.3/edc_dx_review/form_mixins/clinical_review_baseline_required_form_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/form_validator_mixins/clinical_review_followup_form_validator_mixin.py` & `edc_dx_review-0.3.3/edc_dx_review/form_validator_mixins/clinical_review_followup_form_validator_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/list_data.py` & `edc_dx_review-0.3.3/edc_dx_review/list_data.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/medical_date.py` & `edc_dx_review-0.3.3/edc_dx_review/medical_date.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/migrations/0001_initial.py` & `edc_dx_review-0.3.3/edc_dx_review/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/migrations/0002_diagnosislocations_extra_value_and_more.py` & `edc_dx_review-0.3.3/edc_dx_review/migrations/0002_diagnosislocations_extra_value_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/migrations/0003_alter_diagnosislocations_options_and_more.py` & `edc_dx_review-0.3.3/edc_dx_review/migrations/0003_alter_diagnosislocations_options_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/migrations/0004_remove_diagnosislocations_edc_dx_revi_name_a39b40_idx_and_more.py` & `edc_dx_review-0.3.3/edc_dx_review/migrations/0004_remove_diagnosislocations_edc_dx_revi_name_a39b40_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/model_mixins/__init__.py` & `edc_dx_review-0.3.3/edc_dx_review/model_mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/model_mixins/clinical_review_baseline_model_mixin.py` & `edc_dx_review-0.3.3/edc_dx_review/model_mixins/clinical_review_baseline_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/model_mixins/clinical_review_followup/clinical_review_followup_chol_model_mixin.py` & `edc_dx_review-0.3.3/edc_dx_review/model_mixins/clinical_review_followup/clinical_review_followup_chol_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/model_mixins/clinical_review_followup/clinical_review_followup_dm_model_mixin.py` & `edc_dx_review-0.3.3/edc_dx_review/model_mixins/clinical_review_followup/clinical_review_followup_dm_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/model_mixins/clinical_review_followup/clinical_review_followup_hiv_model_mixin.py` & `edc_dx_review-0.3.3/edc_dx_review/model_mixins/clinical_review_followup/clinical_review_followup_hiv_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/model_mixins/clinical_review_followup/clinical_review_followup_htn_model_mixin.py` & `edc_dx_review-0.3.3/edc_dx_review/model_mixins/clinical_review_followup/clinical_review_followup_htn_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/model_mixins/clinical_review_followup/clinical_review_followup_model_mixin.py` & `edc_dx_review-0.3.3/edc_dx_review/model_mixins/clinical_review_followup/clinical_review_followup_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/model_mixins/factory/baseline_review_model_mixin_factory.py` & `edc_dx_review-0.3.3/edc_dx_review/model_mixins/factory/baseline_review_model_mixin_factory.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/model_mixins/factory/calculate_date.py` & `edc_dx_review-0.3.3/edc_dx_review/model_mixins/factory/calculate_date.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/model_mixins/factory/dx_initial_review_model_mixin_factory.py` & `edc_dx_review-0.3.3/edc_dx_review/model_mixins/factory/dx_initial_review_model_mixin_factory.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/model_mixins/factory/followup_review_model_mixin_factory.py` & `edc_dx_review-0.3.3/edc_dx_review/model_mixins/factory/followup_review_model_mixin_factory.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/model_mixins/factory/rx_initial_review_model_mixin_factory.py` & `edc_dx_review-0.3.3/edc_dx_review/model_mixins/factory/rx_initial_review_model_mixin_factory.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/model_mixins/followup_review/followup_review_model_mixin.py` & `edc_dx_review-0.3.3/edc_dx_review/model_mixins/followup_review/followup_review_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/model_mixins/followup_review/hiv_followup_review_model_mixin.py` & `edc_dx_review-0.3.3/edc_dx_review/model_mixins/followup_review/hiv_followup_review_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/model_mixins/initial_review/chol_initial_review_model_mixin.py` & `edc_dx_review-0.3.3/edc_dx_review/model_mixins/initial_review/chol_initial_review_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/model_mixins/initial_review/hiv_initial_model_mixins.py` & `edc_dx_review-0.3.3/edc_dx_review/model_mixins/initial_review/hiv_initial_model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/model_mixins/initial_review/ncd_initial_review_model_mixin.py` & `edc_dx_review-0.3.3/edc_dx_review/model_mixins/initial_review/ncd_initial_review_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/models.py` & `edc_dx_review-0.3.3/edc_dx_review/models.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/radio_fields.py` & `edc_dx_review-0.3.3/edc_dx_review/radio_fields.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/tests/etc/user-rsa-local-private.pem` & `edc_dx_review-0.3.3/edc_dx_review/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/tests/etc/user-rsa-restricted-private.pem` & `edc_dx_review-0.3.3/edc_dx_review/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/tests/tests/test_medical_date.py` & `edc_dx_review-0.3.3/edc_dx_review/tests/tests/test_medical_date.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/edc_dx_review/utils.py` & `edc_dx_review-0.3.3/edc_dx_review/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 from __future__ import annotations
 
 from datetime import date, datetime
+from typing import TYPE_CHECKING
 
 from django import forms
 from django.apps import apps as django_apps
 from django.conf import settings
 from django.core.exceptions import ObjectDoesNotExist
 from edc_constants.constants import HIV, YES
 from edc_model.utils import model_exists_or_raise
 from edc_visit_schedule.baseline import VisitScheduleBaselineError
 from edc_visit_schedule.utils import is_baseline
 
+if TYPE_CHECKING:
+    from edc_model.models import BaseUuidModel
+    from edc_visit_tracking.model_mixins import VisitTrackingCrfModelMixin
+
+    class CrfLikeModel(VisitTrackingCrfModelMixin, BaseUuidModel):
+        pass
+
+
 EDC_DX_REVIEW_APP_LABEL = getattr(settings, "EDC_DX_REVIEW_APP_LABEL", "edc_dx_review")
 
 
 class ModelNotDefined(Exception):
     pass
 
 
@@ -73,28 +82,29 @@
     except AttributeError:
         pass
     else:
         extra_attrs.update(data)
     return extra_attrs
 
 
-def raise_if_clinical_review_does_not_exist(subject_visit) -> None:
+def raise_if_clinical_review_does_not_exist(subject_visit) -> CrfLikeModel:
     try:
         baseline = is_baseline(instance=subject_visit)
     except VisitScheduleBaselineError as e:
         raise forms.ValidationError(str(e))
     else:
         if baseline:
             model_cls = get_clinical_review_baseline_model_cls()
         else:
             model_cls = get_clinical_review_model_cls()
         try:
-            model_exists_or_raise(subject_visit=subject_visit, model_cls=model_cls)
+            obj = model_exists_or_raise(subject_visit=subject_visit, model_cls=model_cls)
         except ObjectDoesNotExist:
             raise forms.ValidationError(f"Complete {model_cls._meta.verbose_name} CRF first.")
+    return obj
 
 
 def raise_if_both_ago_and_actual_date(
     cleaned_data: dict | None = None,
     date_fld: str | None = None,
     ago_fld: str | None = None,
     dx_ago: str | None = None,
```

### Comparing `edc-dx-review-0.3.2/edc_dx_review.egg-info/PKG-INFO` & `edc_dx_review-0.3.3/edc_dx_review.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-dx-review
-Version: 0.3.2
+Version: 0.3.3
 Summary: Classes to manage review of HIV, DM and HTN diagnoses for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-dx-review
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django glucose ifg ogtt clinicedc clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-dx-review-0.3.2/edc_dx_review.egg-info/SOURCES.txt` & `edc_dx_review-0.3.3/edc_dx_review.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/pyproject.toml` & `edc_dx_review-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/runtests.py` & `edc_dx_review-0.3.3/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-dx-review-0.3.2/setup.cfg` & `edc_dx_review-0.3.3/setup.cfg`

 * *Files identical despite different names*


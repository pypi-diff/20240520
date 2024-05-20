# Comparing `tmp/pycaching-4.4.1.tar.gz` & `tmp/pycaching-4.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycaching-4.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pycaching-4.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pycaching-4.4.1.tar` & `pycaching-4.4.2.tar`

### file list

```diff
@@ -1,120 +1,120 @@
--rw-r--r--   0        0        0      258 2024-01-29 12:25:42.239973 pycaching-4.4.1/.editorconfig
--rw-r--r--   0        0        0      141 2024-01-29 12:25:42.239973 pycaching-4.4.1/.flake8
--rw-r--r--   0        0        0      774 2024-01-29 12:25:42.239973 pycaching-4.4.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      650 2024-01-29 12:25:42.239973 pycaching-4.4.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1244 2024-01-29 12:25:42.239973 pycaching-4.4.1/.gitignore
--rw-r--r--   0        0        0      400 2024-01-29 12:25:42.239973 pycaching-4.4.1/.readthedocs.yaml
--rw-r--r--   0        0        0     5094 2024-01-29 12:25:42.239973 pycaching-4.4.1/CONTRIBUTING.rst
--rw-r--r--   0        0        0     7650 2024-01-29 12:25:42.239973 pycaching-4.4.1/LICENSE.txt
--rw-r--r--   0        0        0     9100 2024-01-29 12:25:42.239973 pycaching-4.4.1/README.rst
--rw-r--r--   0        0        0     7421 2024-01-29 12:25:42.239973 pycaching-4.4.1/docs/Makefile
--rw-r--r--   0        0        0     1994 2024-01-29 12:25:42.239973 pycaching-4.4.1/docs/api.rst
--rw-r--r--   0        0        0       88 2024-01-29 12:25:42.239973 pycaching-4.4.1/docs/appendix.rst
--rw-r--r--   0        0        0     9953 2024-01-29 12:25:42.239973 pycaching-4.4.1/docs/conf.py
--rw-r--r--   0        0        0       33 2024-01-29 12:25:42.239973 pycaching-4.4.1/docs/contributing.rst
--rw-r--r--   0        0        0      610 2024-01-29 12:25:42.239973 pycaching-4.4.1/docs/index.rst
--rw-r--r--   0        0        0      261 2024-01-29 12:25:42.239973 pycaching-4.4.1/docs/quickstart.rst
--rw-r--r--   0        0        0      571 2024-01-29 12:25:42.239973 pycaching-4.4.1/pycaching/__init__.py
--rw-r--r--   0        0        0    51736 2024-01-29 12:25:42.239973 pycaching-4.4.1/pycaching/cache.py
--rw-r--r--   0        0        0     1639 2024-01-29 12:25:42.239973 pycaching-4.4.1/pycaching/errors.py
--rw-r--r--   0        0        0    21138 2024-01-29 12:25:42.239973 pycaching-4.4.1/pycaching/geo.py
--rw-r--r--   0        0        0    20881 2024-01-29 12:25:42.239973 pycaching-4.4.1/pycaching/geocaching.py
--rw-r--r--   0        0        0     3864 2024-01-29 12:25:42.239973 pycaching-4.4.1/pycaching/log.py
--rw-r--r--   0        0        0     7925 2024-01-29 12:25:42.239973 pycaching-4.4.1/pycaching/trackable.py
--rw-r--r--   0        0        0     3855 2024-01-29 12:25:42.239973 pycaching-4.4.1/pycaching/util.py
--rw-r--r--   0        0        0     2196 2024-01-29 12:25:42.239973 pycaching-4.4.1/pyproject.toml
--rw-r--r--   0        0        0     2139 2024-01-29 12:25:42.239973 pycaching-4.4.1/test/__init__.py
--rw-r--r--   0        0        0    17074 2024-01-29 12:25:42.239973 pycaching-4.4.1/test/cassettes/advanced_search.json
--rw-r--r--   0        0        0    20618 2024-01-29 12:25:42.239973 pycaching-4.4.1/test/cassettes/advanced_search_caches_owned_by_hq.json
--rw-r--r--   0        0        0    32832 2024-01-29 12:25:42.243973 pycaching-4.4.1/test/cassettes/cache_PMO.json
--rw-r--r--   0        0        0   113134 2024-01-29 12:25:42.243973 pycaching-4.4.1/test/cassettes/cache_author_deleted.json
--rw-r--r--   0        0        0   183609 2024-01-29 12:25:42.243973 pycaching-4.4.1/test/cassettes/cache_author_normal.json
--rw-r--r--   0        0        0   191649 2024-01-29 12:25:42.243973 pycaching-4.4.1/test/cassettes/cache_explicit_load.json
--rw-r--r--   0        0        0    18136 2024-01-29 12:25:42.243973 pycaching-4.4.1/test/cassettes/cache_guidload_PMO.json
--rw-r--r--   0        0        0     6399 2024-01-29 12:25:42.243973 pycaching-4.4.1/test/cassettes/cache_guidload_fallback.json
--rw-r--r--   0        0        0    40219 2024-01-29 12:25:42.243973 pycaching-4.4.1/test/cassettes/cache_guidload_normal.json
--rw-r--r--   0        0        0   134689 2024-01-29 12:25:42.243973 pycaching-4.4.1/test/cassettes/cache_hint_lazy_loading.json
--rw-r--r--   0        0        0    60961 2024-01-29 12:25:42.243973 pycaching-4.4.1/test/cassettes/cache_hint_load_by_guid.json
--rw-r--r--   0        0        0    99634 2024-01-29 12:25:42.247973 pycaching-4.4.1/test/cassettes/cache_logbook.json
--rw-r--r--   0        0        0    40098 2024-01-29 12:25:42.247973 pycaching-4.4.1/test/cassettes/cache_logpage.json
--rw-r--r--   0        0        0   172026 2024-01-29 12:25:42.247973 pycaching-4.4.1/test/cassettes/cache_non-ascii.json
--rw-r--r--   0        0        0     6370 2024-01-29 12:25:42.247973 pycaching-4.4.1/test/cassettes/cache_normal_fail.json
--rw-r--r--   0        0        0   191649 2024-01-29 12:25:42.247973 pycaching-4.4.1/test/cassettes/cache_normal_normal.json
--rw-r--r--   0        0        0     3453 2024-01-29 12:25:42.247973 pycaching-4.4.1/test/cassettes/cache_quick_normal.json
--rw-r--r--   0        0        0     2944 2024-01-29 12:25:42.247973 pycaching-4.4.1/test/cassettes/cache_quickload_fail.json
--rw-r--r--   0        0        0   132019 2024-01-29 12:25:42.247973 pycaching-4.4.1/test/cassettes/cache_setup.json
--rw-r--r--   0        0        0   124130 2024-01-29 12:25:42.247973 pycaching-4.4.1/test/cassettes/cache_status_archived.json
--rw-r--r--   0        0        0   153377 2024-01-29 12:25:42.247973 pycaching-4.4.1/test/cassettes/cache_status_disabled.json
--rw-r--r--   0        0        0   133829 2024-01-29 12:25:42.247973 pycaching-4.4.1/test/cassettes/cache_status_enabled.json
--rw-r--r--   0        0        0     3430 2024-01-29 12:25:42.247973 pycaching-4.4.1/test/cassettes/cache_status_enabled_load_quick.json
--rw-r--r--   0        0        0   110598 2024-01-29 12:25:42.247973 pycaching-4.4.1/test/cassettes/cache_status_locked.json
--rw-r--r--   0        0        0   154706 2024-01-29 12:25:42.247973 pycaching-4.4.1/test/cassettes/cache_trackables.json
--rw-r--r--   0        0        0   154575 2024-01-29 12:25:42.251973 pycaching-4.4.1/test/cassettes/cache_type_gigaevent.json
--rw-r--r--   0        0        0   143699 2024-01-29 12:25:42.251973 pycaching-4.4.1/test/cassettes/cache_type_headquarters.json
--rw-r--r--   0        0        0   131084 2024-01-29 12:25:42.251973 pycaching-4.4.1/test/cassettes/cache_type_hq_celebration.json
--rw-r--r--   0        0        0   137851 2024-01-29 12:25:42.251973 pycaching-4.4.1/test/cassettes/cache_type_locationless.json
--rw-r--r--   0        0        0   159850 2024-01-29 12:25:42.251973 pycaching-4.4.1/test/cassettes/cache_type_projectape.json
--rw-r--r--   0        0        0     1923 2024-01-29 12:25:42.251973 pycaching-4.4.1/test/cassettes/geo_location_empty.json
--rw-r--r--   0        0        0     5710 2024-01-29 12:25:42.251973 pycaching-4.4.1/test/cassettes/geo_location_existing.json
--rw-r--r--   0        0        0     1967 2024-01-29 12:25:42.251973 pycaching-4.4.1/test/cassettes/geo_location_nonexisting.json
--rw-r--r--   0        0        0   197015 2024-01-29 12:25:42.251973 pycaching-4.4.1/test/cassettes/geo_point_utfgrid.json
--rw-r--r--   0        0        0    95750 2024-01-29 12:25:42.251973 pycaching-4.4.1/test/cassettes/geocaching__try_getting_cache_from_guid.json
--rw-r--r--   0        0        0    55296 2024-01-29 12:25:42.251973 pycaching-4.4.1/test/cassettes/geocaching__try_getting_cache_from_guid_pm_only.json
--rw-r--r--   0        0        0    34872 2024-01-29 12:25:42.251973 pycaching-4.4.1/test/cassettes/geocaching_api_rate_limit.json
--rw-r--r--   0        0        0    35466 2024-01-29 12:25:42.251973 pycaching-4.4.1/test/cassettes/geocaching_api_rate_limit_with_none.json
--rw-r--r--   0        0        0    20513 2024-01-29 12:25:42.251973 pycaching-4.4.1/test/cassettes/geocaching_my_dnfs.json
--rw-r--r--   0        0        0    20513 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/cassettes/geocaching_my_finds.json
--rw-r--r--   0        0        0     5819 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/cassettes/geocaching_quick_search.json
--rw-r--r--   0        0        0     8421 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/cassettes/geocaching_search.json
--rw-r--r--   0        0        0    32317 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/cassettes/geocaching_search_pagination.json
--rw-r--r--   0        0        0    54022 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/cassettes/geocaching_search_rect.json
--rw-r--r--   0        0        0     1950 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/cassettes/geocaching_shortcut_geocode.json
--rw-r--r--   0        0        0   191634 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/cassettes/geocaching_shortcut_getcache.json
--rw-r--r--   0        0        0    95764 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/cassettes/geocaching_shortcut_getcache_by_guid.json
--rw-r--r--   0        0        0    54940 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/cassettes/geocaching_shortcut_gettrackable.json
--rw-r--r--   0        0        0   136794 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/cassettes/trackable_kml.json
--rw-r--r--   0        0        0    51360 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/cassettes/trackable_load__existing_type.json
--rw-r--r--   0        0        0    49536 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/cassettes/trackable_load__missing_type.json
--rw-r--r--   0        0        0    37400 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/cassettes/trackable_load_page.json
--rw-r--r--   0        0        0    54937 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/cassettes/trackable_load_tid.json
--rw-r--r--   0        0        0    56263 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/cassettes/trackable_load_url.json
--rw-r--r--   0        0        0    54923 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/cassettes/trackable_setup.json
--rw-r--r--   0        0        0    43299 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/cassettes/util_attributes.json
--rw-r--r--   0        0        0     1005 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/helpers.py
--rw-r--r--   0        0        0     1137 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/sample_caches.csv
--rw-r--r--   0        0        0    29469 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/sample_utfgrid.json
--rw-r--r--   0        0        0    21121 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/test_cache.py
--rw-r--r--   0        0        0    16347 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/test_geo.py
--rw-r--r--   0        0        0    11300 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/test_geocaching.py
--rw-r--r--   0        0        0     1845 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/test_log.py
--rw-r--r--   0        0        0     6225 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/test_trackable.py
--rw-r--r--   0        0        0     3320 2024-01-29 12:25:42.255973 pycaching-4.4.1/test/test_util.py
--rw-r--r--   0        0        0        0 2024-01-29 12:25:42.255973 pycaching-4.4.1/tests_new/__init__.py
--rw-r--r--   0        0        0       65 2024-01-29 12:25:42.255973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test.json
--rw-r--r--   0        0        0       65 2024-01-29 12:25:42.255973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_file_empty.json
--rw-r--r--   0        0        0       65 2024-01-29 12:25:42.255973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_file_invalid_json.json
--rw-r--r--   0        0        0       65 2024-01-29 12:25:42.255973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_file_multiuser_empty.json
--rw-r--r--   0        0        0       65 2024-01-29 12:25:42.255973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_file_multiuser_empty_item.json
--rw-r--r--   0        0        0       65 2024-01-29 12:25:42.255973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_file_nonexisting.json
--rw-r--r--   0        0        0       65 2024-01-29 12:25:42.255973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_file_string.json
--rw-r--r--   0        0        0       65 2024-01-29 12:25:42.255973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_multiuser.json
--rw-r--r--   0        0        0       65 2024-01-29 12:25:42.255973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_multiuser_with_nonexisting_username.json
--rw-r--r--   0        0        0       65 2024-01-29 12:25:42.255973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_multiuser_with_username.json
--rw-r--r--   0        0        0       65 2024-01-29 12:25:42.255973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_password_cmd.json
--rw-r--r--   0        0        0       65 2024-01-29 12:25:42.255973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_password_cmd_ambiguous.json
--rw-r--r--   0        0        0       65 2024-01-29 12:25:42.255973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_password_cmd_invalid.json
--rw-r--r--   0        0        0       65 2024-01-29 12:25:42.255973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_with_nonexisting_username.json
--rw-r--r--   0        0        0       65 2024-01-29 12:25:42.255973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_with_username.json
--rw-r--r--   0        0        0   480589 2024-01-29 12:25:42.259973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.test_get_logged_user.json
--rw-r--r--   0        0        0   253412 2024-01-29 12:25:42.259973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.test_login.json
--rw-r--r--   0        0        0    51897 2024-01-29 12:25:42.259973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.test_login_bad_credentials.json
--rw-r--r--   0        0        0       65 2024-01-29 12:25:42.259973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.test_login_failed_because_of_load_credentials_failed.json
--rw-r--r--   0        0        0   253411 2024-01-29 12:25:42.259973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.test_login_twice_with_valid_credentials.json
--rw-r--r--   0        0        0   279122 2024-01-29 12:25:42.259973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.test_logout.json
--rw-r--r--   0        0        0    51897 2024-01-29 12:25:42.259973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.test_logout_when_relogin_is_attempted_with_invalid_credentials.json
--rw-r--r--   0        0        0       65 2024-01-29 12:25:42.259973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.test_unauthorized_request.json
--rw-r--r--   0        0        0   253412 2024-01-29 12:25:42.259973 pycaching-4.4.1/tests_new/cassettes/tests_new.test_shortcuts.test_login.json
--rw-r--r--   0        0        0     2914 2024-01-29 12:25:42.259973 pycaching-4.4.1/tests_new/conftest.py
--rw-r--r--   0        0        0     7126 2024-01-29 12:25:42.259973 pycaching-4.4.1/tests_new/test_geocaching.py
--rw-r--r--   0        0        0      553 2024-01-29 12:25:42.259973 pycaching-4.4.1/tests_new/test_shortcuts.py
--rw-r--r--   0        0        0    10307 1970-01-01 00:00:00.000000 pycaching-4.4.1/PKG-INFO
+-rw-r--r--   0        0        0      258 2024-05-20 08:42:40.898428 pycaching-4.4.2/.editorconfig
+-rw-r--r--   0        0        0      141 2024-05-20 08:42:40.898428 pycaching-4.4.2/.flake8
+-rw-r--r--   0        0        0      774 2024-05-20 08:42:40.898428 pycaching-4.4.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      650 2024-05-20 08:42:40.898428 pycaching-4.4.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1244 2024-05-20 08:42:40.898428 pycaching-4.4.2/.gitignore
+-rw-r--r--   0        0        0      400 2024-05-20 08:42:40.898428 pycaching-4.4.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     5094 2024-05-20 08:42:40.898428 pycaching-4.4.2/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     7650 2024-05-20 08:42:40.898428 pycaching-4.4.2/LICENSE.txt
+-rw-r--r--   0        0        0     9100 2024-05-20 08:42:40.898428 pycaching-4.4.2/README.rst
+-rw-r--r--   0        0        0     7421 2024-05-20 08:42:40.898428 pycaching-4.4.2/docs/Makefile
+-rw-r--r--   0        0        0     1994 2024-05-20 08:42:40.898428 pycaching-4.4.2/docs/api.rst
+-rw-r--r--   0        0        0       88 2024-05-20 08:42:40.898428 pycaching-4.4.2/docs/appendix.rst
+-rw-r--r--   0        0        0     9953 2024-05-20 08:42:40.898428 pycaching-4.4.2/docs/conf.py
+-rw-r--r--   0        0        0       33 2024-05-20 08:42:40.898428 pycaching-4.4.2/docs/contributing.rst
+-rw-r--r--   0        0        0      610 2024-05-20 08:42:40.898428 pycaching-4.4.2/docs/index.rst
+-rw-r--r--   0        0        0      261 2024-05-20 08:42:40.898428 pycaching-4.4.2/docs/quickstart.rst
+-rw-r--r--   0        0        0      571 2024-05-20 08:42:40.898428 pycaching-4.4.2/pycaching/__init__.py
+-rw-r--r--   0        0        0    51736 2024-05-20 08:42:40.902428 pycaching-4.4.2/pycaching/cache.py
+-rw-r--r--   0        0        0     1639 2024-05-20 08:42:40.902428 pycaching-4.4.2/pycaching/errors.py
+-rw-r--r--   0        0        0    21135 2024-05-20 08:42:40.902428 pycaching-4.4.2/pycaching/geo.py
+-rw-r--r--   0        0        0    20881 2024-05-20 08:42:40.902428 pycaching-4.4.2/pycaching/geocaching.py
+-rw-r--r--   0        0        0     3967 2024-05-20 08:42:40.902428 pycaching-4.4.2/pycaching/log.py
+-rw-r--r--   0        0        0     7925 2024-05-20 08:42:40.902428 pycaching-4.4.2/pycaching/trackable.py
+-rw-r--r--   0        0        0     3855 2024-05-20 08:42:40.902428 pycaching-4.4.2/pycaching/util.py
+-rw-r--r--   0        0        0     2196 2024-05-20 08:42:40.902428 pycaching-4.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2139 2024-05-20 08:42:40.902428 pycaching-4.4.2/test/__init__.py
+-rw-r--r--   0        0        0    17074 2024-05-20 08:42:40.902428 pycaching-4.4.2/test/cassettes/advanced_search.json
+-rw-r--r--   0        0        0    20618 2024-05-20 08:42:40.902428 pycaching-4.4.2/test/cassettes/advanced_search_caches_owned_by_hq.json
+-rw-r--r--   0        0        0    32832 2024-05-20 08:42:40.902428 pycaching-4.4.2/test/cassettes/cache_PMO.json
+-rw-r--r--   0        0        0   113134 2024-05-20 08:42:40.902428 pycaching-4.4.2/test/cassettes/cache_author_deleted.json
+-rw-r--r--   0        0        0   183609 2024-05-20 08:42:40.902428 pycaching-4.4.2/test/cassettes/cache_author_normal.json
+-rw-r--r--   0        0        0   191649 2024-05-20 08:42:40.906428 pycaching-4.4.2/test/cassettes/cache_explicit_load.json
+-rw-r--r--   0        0        0    18136 2024-05-20 08:42:40.906428 pycaching-4.4.2/test/cassettes/cache_guidload_PMO.json
+-rw-r--r--   0        0        0     6399 2024-05-20 08:42:40.906428 pycaching-4.4.2/test/cassettes/cache_guidload_fallback.json
+-rw-r--r--   0        0        0    40219 2024-05-20 08:42:40.906428 pycaching-4.4.2/test/cassettes/cache_guidload_normal.json
+-rw-r--r--   0        0        0   134689 2024-05-20 08:42:40.906428 pycaching-4.4.2/test/cassettes/cache_hint_lazy_loading.json
+-rw-r--r--   0        0        0    60961 2024-05-20 08:42:40.906428 pycaching-4.4.2/test/cassettes/cache_hint_load_by_guid.json
+-rw-r--r--   0        0        0    99634 2024-05-20 08:42:40.906428 pycaching-4.4.2/test/cassettes/cache_logbook.json
+-rw-r--r--   0        0        0    40098 2024-05-20 08:42:40.906428 pycaching-4.4.2/test/cassettes/cache_logpage.json
+-rw-r--r--   0        0        0   172026 2024-05-20 08:42:40.906428 pycaching-4.4.2/test/cassettes/cache_non-ascii.json
+-rw-r--r--   0        0        0     6370 2024-05-20 08:42:40.906428 pycaching-4.4.2/test/cassettes/cache_normal_fail.json
+-rw-r--r--   0        0        0   191649 2024-05-20 08:42:40.906428 pycaching-4.4.2/test/cassettes/cache_normal_normal.json
+-rw-r--r--   0        0        0     3453 2024-05-20 08:42:40.906428 pycaching-4.4.2/test/cassettes/cache_quick_normal.json
+-rw-r--r--   0        0        0     2944 2024-05-20 08:42:40.906428 pycaching-4.4.2/test/cassettes/cache_quickload_fail.json
+-rw-r--r--   0        0        0   132019 2024-05-20 08:42:40.906428 pycaching-4.4.2/test/cassettes/cache_setup.json
+-rw-r--r--   0        0        0   124130 2024-05-20 08:42:40.906428 pycaching-4.4.2/test/cassettes/cache_status_archived.json
+-rw-r--r--   0        0        0   153377 2024-05-20 08:42:40.910428 pycaching-4.4.2/test/cassettes/cache_status_disabled.json
+-rw-r--r--   0        0        0   133829 2024-05-20 08:42:40.910428 pycaching-4.4.2/test/cassettes/cache_status_enabled.json
+-rw-r--r--   0        0        0     3430 2024-05-20 08:42:40.910428 pycaching-4.4.2/test/cassettes/cache_status_enabled_load_quick.json
+-rw-r--r--   0        0        0   110598 2024-05-20 08:42:40.910428 pycaching-4.4.2/test/cassettes/cache_status_locked.json
+-rw-r--r--   0        0        0   154706 2024-05-20 08:42:40.910428 pycaching-4.4.2/test/cassettes/cache_trackables.json
+-rw-r--r--   0        0        0   154575 2024-05-20 08:42:40.910428 pycaching-4.4.2/test/cassettes/cache_type_gigaevent.json
+-rw-r--r--   0        0        0   143699 2024-05-20 08:42:40.910428 pycaching-4.4.2/test/cassettes/cache_type_headquarters.json
+-rw-r--r--   0        0        0   131084 2024-05-20 08:42:40.910428 pycaching-4.4.2/test/cassettes/cache_type_hq_celebration.json
+-rw-r--r--   0        0        0   137851 2024-05-20 08:42:40.910428 pycaching-4.4.2/test/cassettes/cache_type_locationless.json
+-rw-r--r--   0        0        0   159850 2024-05-20 08:42:40.910428 pycaching-4.4.2/test/cassettes/cache_type_projectape.json
+-rw-r--r--   0        0        0     1923 2024-05-20 08:42:40.910428 pycaching-4.4.2/test/cassettes/geo_location_empty.json
+-rw-r--r--   0        0        0     5710 2024-05-20 08:42:40.910428 pycaching-4.4.2/test/cassettes/geo_location_existing.json
+-rw-r--r--   0        0        0     1967 2024-05-20 08:42:40.910428 pycaching-4.4.2/test/cassettes/geo_location_nonexisting.json
+-rw-r--r--   0        0        0   197015 2024-05-20 08:42:40.910428 pycaching-4.4.2/test/cassettes/geo_point_utfgrid.json
+-rw-r--r--   0        0        0    95750 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/geocaching__try_getting_cache_from_guid.json
+-rw-r--r--   0        0        0    55296 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/geocaching__try_getting_cache_from_guid_pm_only.json
+-rw-r--r--   0        0        0    34872 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/geocaching_api_rate_limit.json
+-rw-r--r--   0        0        0    35466 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/geocaching_api_rate_limit_with_none.json
+-rw-r--r--   0        0        0    20513 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/geocaching_my_dnfs.json
+-rw-r--r--   0        0        0    20513 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/geocaching_my_finds.json
+-rw-r--r--   0        0        0     5819 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/geocaching_quick_search.json
+-rw-r--r--   0        0        0     8421 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/geocaching_search.json
+-rw-r--r--   0        0        0    32317 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/geocaching_search_pagination.json
+-rw-r--r--   0        0        0    54022 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/geocaching_search_rect.json
+-rw-r--r--   0        0        0     1950 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/geocaching_shortcut_geocode.json
+-rw-r--r--   0        0        0   191634 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/geocaching_shortcut_getcache.json
+-rw-r--r--   0        0        0    95764 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/geocaching_shortcut_getcache_by_guid.json
+-rw-r--r--   0        0        0    54940 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/geocaching_shortcut_gettrackable.json
+-rw-r--r--   0        0        0   136794 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/trackable_kml.json
+-rw-r--r--   0        0        0    51360 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/trackable_load__existing_type.json
+-rw-r--r--   0        0        0    49536 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/trackable_load__missing_type.json
+-rw-r--r--   0        0        0    37400 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/trackable_load_page.json
+-rw-r--r--   0        0        0    54937 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/trackable_load_tid.json
+-rw-r--r--   0        0        0    56263 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/trackable_load_url.json
+-rw-r--r--   0        0        0    54923 2024-05-20 08:42:40.914428 pycaching-4.4.2/test/cassettes/trackable_setup.json
+-rw-r--r--   0        0        0    43299 2024-05-20 08:42:40.918428 pycaching-4.4.2/test/cassettes/util_attributes.json
+-rw-r--r--   0        0        0     1005 2024-05-20 08:42:40.918428 pycaching-4.4.2/test/helpers.py
+-rw-r--r--   0        0        0     1137 2024-05-20 08:42:40.918428 pycaching-4.4.2/test/sample_caches.csv
+-rw-r--r--   0        0        0    29469 2024-05-20 08:42:40.918428 pycaching-4.4.2/test/sample_utfgrid.json
+-rw-r--r--   0        0        0    21121 2024-05-20 08:42:40.918428 pycaching-4.4.2/test/test_cache.py
+-rw-r--r--   0        0        0    16523 2024-05-20 08:42:40.918428 pycaching-4.4.2/test/test_geo.py
+-rw-r--r--   0        0        0    11300 2024-05-20 08:42:40.918428 pycaching-4.4.2/test/test_geocaching.py
+-rw-r--r--   0        0        0     1981 2024-05-20 08:42:40.918428 pycaching-4.4.2/test/test_log.py
+-rw-r--r--   0        0        0     6225 2024-05-20 08:42:40.918428 pycaching-4.4.2/test/test_trackable.py
+-rw-r--r--   0        0        0     3320 2024-05-20 08:42:40.918428 pycaching-4.4.2/test/test_util.py
+-rw-r--r--   0        0        0        0 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test.json
+-rw-r--r--   0        0        0       65 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_file_empty.json
+-rw-r--r--   0        0        0       65 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_file_invalid_json.json
+-rw-r--r--   0        0        0       65 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_file_multiuser_empty.json
+-rw-r--r--   0        0        0       65 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_file_multiuser_empty_item.json
+-rw-r--r--   0        0        0       65 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_file_nonexisting.json
+-rw-r--r--   0        0        0       65 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_file_string.json
+-rw-r--r--   0        0        0       65 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_multiuser.json
+-rw-r--r--   0        0        0       65 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_multiuser_with_nonexisting_username.json
+-rw-r--r--   0        0        0       65 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_multiuser_with_username.json
+-rw-r--r--   0        0        0       65 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_password_cmd.json
+-rw-r--r--   0        0        0       65 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_password_cmd_ambiguous.json
+-rw-r--r--   0        0        0       65 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_password_cmd_invalid.json
+-rw-r--r--   0        0        0       65 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_with_nonexisting_username.json
+-rw-r--r--   0        0        0       65 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.TestLoadCredentials.test_with_username.json
+-rw-r--r--   0        0        0   480589 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.test_get_logged_user.json
+-rw-r--r--   0        0        0   253412 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.test_login.json
+-rw-r--r--   0        0        0    51897 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.test_login_bad_credentials.json
+-rw-r--r--   0        0        0       65 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.test_login_failed_because_of_load_credentials_failed.json
+-rw-r--r--   0        0        0   253411 2024-05-20 08:42:40.918428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.test_login_twice_with_valid_credentials.json
+-rw-r--r--   0        0        0   279122 2024-05-20 08:42:40.922428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.test_logout.json
+-rw-r--r--   0        0        0    51897 2024-05-20 08:42:40.922428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.test_logout_when_relogin_is_attempted_with_invalid_credentials.json
+-rw-r--r--   0        0        0       65 2024-05-20 08:42:40.922428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.test_unauthorized_request.json
+-rw-r--r--   0        0        0   253412 2024-05-20 08:42:40.922428 pycaching-4.4.2/tests_new/cassettes/tests_new.test_shortcuts.test_login.json
+-rw-r--r--   0        0        0     2914 2024-05-20 08:42:40.922428 pycaching-4.4.2/tests_new/conftest.py
+-rw-r--r--   0        0        0     7126 2024-05-20 08:42:40.922428 pycaching-4.4.2/tests_new/test_geocaching.py
+-rw-r--r--   0        0        0      553 2024-05-20 08:42:40.922428 pycaching-4.4.2/tests_new/test_shortcuts.py
+-rw-r--r--   0        0        0    10307 1970-01-01 00:00:00.000000 pycaching-4.4.2/PKG-INFO
```

### Comparing `pycaching-4.4.1/.github/workflows/ci.yml` & `pycaching-4.4.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/.github/workflows/release.yml` & `pycaching-4.4.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/.gitignore` & `pycaching-4.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/CONTRIBUTING.rst` & `pycaching-4.4.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/LICENSE.txt` & `pycaching-4.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/README.rst` & `pycaching-4.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/docs/Makefile` & `pycaching-4.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/docs/api.rst` & `pycaching-4.4.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/docs/conf.py` & `pycaching-4.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/docs/index.rst` & `pycaching-4.4.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/pycaching/__init__.py` & `pycaching-4.4.2/pycaching/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pycaching.cache import Cache  # NOQA
 from pycaching.geo import Point, Rectangle  # NOQA
 from pycaching.geocaching import Geocaching  # NOQA
 from pycaching.log import Log  # NOQA
 from pycaching.trackable import Trackable  # NOQA
 
-__version__ = "4.4.1"  # PEP 440
+__version__ = "4.4.2"  # PEP 440
 
 
 def login(username=None, password=None):
     """A shortcut for user login.
 
     Create a :class:`.Geocaching` instance and try to login a user. See :meth:`.Geocaching.login`.
```

### Comparing `pycaching-4.4.1/pycaching/cache.py` & `pycaching-4.4.2/pycaching/cache.py`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/pycaching/errors.py` & `pycaching-4.4.2/pycaching/errors.py`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/pycaching/geo.py` & `pycaching-4.4.2/pycaching/geo.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         """
 
         # Convert to uppercase to simplify hemisphere comparisons
         string = string.upper()
         coords = string.replace("N", " ").replace("S", " ").replace("E", " ").replace("W", " ").replace("+", " ")
 
         try:
-            m = re.match(r"\s*(-?\s*\d+)\D+(\d+[\.,]\d+)\D?\s*(-?\s*\d+)\D+(\d+[\.,]\d+)", coords)
+            m = re.match(r"\s*(-?\s*\d+)\D+(\d+[\.,]\d+)\D+(-?\s*\d+)\D+(\d+[\.,]\d+)", coords)
 
             latDeg, latMin, lonDeg, lonMin = [float(part.replace(" ", "").replace(",", ".")) for part in m.groups()]
 
             if "S" in string:
                 latDeg *= -1
                 latMin *= -1
             if "W" in string:
```

### Comparing `pycaching-4.4.1/pycaching/geocaching.py` & `pycaching-4.4.2/pycaching/geocaching.py`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/pycaching/log.py` & `pycaching-4.4.2/pycaching/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,17 @@
             return cls.publish_listing
         elif filename == "1001":
             # 2 different IDs for visit
             return cls.visit
         elif filename == "68":
             # 2 different IDs for post_reviewer_note
             return cls.post_reviewer_note
+        elif filename == "6":
+            # 2 different IDs for archive
+            return cls.archive
         elif filename == "1":
             # 2 different IDs for unarchive
             return cls.unarchive
 
         try:
             return cls(filename)
         except ValueError as e:
```

### Comparing `pycaching-4.4.1/pycaching/trackable.py` & `pycaching-4.4.2/pycaching/trackable.py`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/pycaching/util.py` & `pycaching-4.4.2/pycaching/util.py`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/pyproject.toml` & `pycaching-4.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/__init__.py` & `pycaching-4.4.2/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/advanced_search.json` & `pycaching-4.4.2/test/cassettes/advanced_search.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/advanced_search_caches_owned_by_hq.json` & `pycaching-4.4.2/test/cassettes/advanced_search_caches_owned_by_hq.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_PMO.json` & `pycaching-4.4.2/test/cassettes/cache_PMO.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_author_deleted.json` & `pycaching-4.4.2/test/cassettes/cache_author_deleted.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_author_normal.json` & `pycaching-4.4.2/test/cassettes/cache_author_normal.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_explicit_load.json` & `pycaching-4.4.2/test/cassettes/cache_explicit_load.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_guidload_PMO.json` & `pycaching-4.4.2/test/cassettes/cache_guidload_PMO.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_guidload_fallback.json` & `pycaching-4.4.2/test/cassettes/cache_guidload_fallback.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_guidload_normal.json` & `pycaching-4.4.2/test/cassettes/cache_guidload_normal.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_hint_lazy_loading.json` & `pycaching-4.4.2/test/cassettes/cache_hint_lazy_loading.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_hint_load_by_guid.json` & `pycaching-4.4.2/test/cassettes/cache_hint_load_by_guid.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_logbook.json` & `pycaching-4.4.2/test/cassettes/cache_logbook.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_logpage.json` & `pycaching-4.4.2/test/cassettes/cache_logpage.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_non-ascii.json` & `pycaching-4.4.2/test/cassettes/cache_non-ascii.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_normal_fail.json` & `pycaching-4.4.2/test/cassettes/cache_normal_fail.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_normal_normal.json` & `pycaching-4.4.2/test/cassettes/cache_normal_normal.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_quick_normal.json` & `pycaching-4.4.2/test/cassettes/cache_quick_normal.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_quickload_fail.json` & `pycaching-4.4.2/test/cassettes/cache_quickload_fail.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_setup.json` & `pycaching-4.4.2/test/cassettes/cache_setup.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_status_archived.json` & `pycaching-4.4.2/test/cassettes/cache_status_archived.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_status_disabled.json` & `pycaching-4.4.2/test/cassettes/cache_status_disabled.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_status_enabled.json` & `pycaching-4.4.2/test/cassettes/cache_status_enabled.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_status_enabled_load_quick.json` & `pycaching-4.4.2/test/cassettes/cache_status_enabled_load_quick.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_status_locked.json` & `pycaching-4.4.2/test/cassettes/cache_status_locked.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_trackables.json` & `pycaching-4.4.2/test/cassettes/cache_trackables.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_type_gigaevent.json` & `pycaching-4.4.2/test/cassettes/cache_type_gigaevent.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_type_headquarters.json` & `pycaching-4.4.2/test/cassettes/cache_type_headquarters.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_type_hq_celebration.json` & `pycaching-4.4.2/test/cassettes/cache_type_hq_celebration.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_type_locationless.json` & `pycaching-4.4.2/test/cassettes/cache_type_locationless.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/cache_type_projectape.json` & `pycaching-4.4.2/test/cassettes/cache_type_projectape.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/geo_location_empty.json` & `pycaching-4.4.2/test/cassettes/geo_location_empty.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/geo_location_existing.json` & `pycaching-4.4.2/test/cassettes/geo_location_existing.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/geo_location_nonexisting.json` & `pycaching-4.4.2/test/cassettes/geo_location_nonexisting.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/geo_point_utfgrid.json` & `pycaching-4.4.2/test/cassettes/geo_point_utfgrid.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/geocaching__try_getting_cache_from_guid.json` & `pycaching-4.4.2/test/cassettes/geocaching__try_getting_cache_from_guid.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/geocaching__try_getting_cache_from_guid_pm_only.json` & `pycaching-4.4.2/test/cassettes/geocaching__try_getting_cache_from_guid_pm_only.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/geocaching_api_rate_limit.json` & `pycaching-4.4.2/test/cassettes/geocaching_api_rate_limit.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/geocaching_api_rate_limit_with_none.json` & `pycaching-4.4.2/test/cassettes/geocaching_api_rate_limit_with_none.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/geocaching_my_dnfs.json` & `pycaching-4.4.2/test/cassettes/geocaching_my_dnfs.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/geocaching_my_finds.json` & `pycaching-4.4.2/test/cassettes/geocaching_my_finds.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/geocaching_quick_search.json` & `pycaching-4.4.2/test/cassettes/geocaching_quick_search.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/geocaching_search.json` & `pycaching-4.4.2/test/cassettes/geocaching_search.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/geocaching_search_pagination.json` & `pycaching-4.4.2/test/cassettes/geocaching_search_pagination.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/geocaching_search_rect.json` & `pycaching-4.4.2/test/cassettes/geocaching_search_rect.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/geocaching_shortcut_geocode.json` & `pycaching-4.4.2/test/cassettes/geocaching_shortcut_geocode.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/geocaching_shortcut_getcache.json` & `pycaching-4.4.2/test/cassettes/geocaching_shortcut_getcache.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/geocaching_shortcut_getcache_by_guid.json` & `pycaching-4.4.2/test/cassettes/geocaching_shortcut_getcache_by_guid.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/geocaching_shortcut_gettrackable.json` & `pycaching-4.4.2/test/cassettes/geocaching_shortcut_gettrackable.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/trackable_kml.json` & `pycaching-4.4.2/test/cassettes/trackable_kml.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/trackable_load__existing_type.json` & `pycaching-4.4.2/test/cassettes/trackable_load__existing_type.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/trackable_load__missing_type.json` & `pycaching-4.4.2/test/cassettes/trackable_load__missing_type.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/trackable_load_page.json` & `pycaching-4.4.2/test/cassettes/trackable_load_page.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/trackable_load_tid.json` & `pycaching-4.4.2/test/cassettes/trackable_load_tid.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/trackable_load_url.json` & `pycaching-4.4.2/test/cassettes/trackable_load_url.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/trackable_setup.json` & `pycaching-4.4.2/test/cassettes/trackable_setup.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/cassettes/util_attributes.json` & `pycaching-4.4.2/test/cassettes/util_attributes.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/helpers.py` & `pycaching-4.4.2/test/helpers.py`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/sample_caches.csv` & `pycaching-4.4.2/test/sample_caches.csv`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/sample_utfgrid.json` & `pycaching-4.4.2/test/sample_utfgrid.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/test_cache.py` & `pycaching-4.4.2/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/test_geo.py` & `pycaching-4.4.2/test/test_geo.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,17 @@
 
         with self.subTest("degree symbol"):
             self.assertEqual(Point.from_string("N 49° 45.123 E 013° 22.123"), Point(49.75205, 13.36872))
 
         with self.subTest("comma between lat and lon"):
             self.assertEqual(Point.from_string("N 49 45.123, E 013 22.123"), Point(49.75205, 13.36872))
 
+        with self.subTest("comma and space between lat and lon"):
+            self.assertEqual(Point.from_string("N 44° 25.845 , W 72° 02.485"), Point(44.43075, -72.04142))
+
         with self.subTest("marginal values: zeroes"):
             self.assertEqual(Point.from_string("N 49 45.000 E 13 0.0"), Point(49.75, 13.0))
 
         with self.subTest("include precision"):
             self.assertIn("precision", Point(49.75, 13.0).__dict__)
 
         with self.assertRaises(ValueError):
```

### Comparing `pycaching-4.4.1/test/test_geocaching.py` & `pycaching-4.4.2/test/test_geocaching.py`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/test_log.py` & `pycaching-4.4.2/test/test_log.py`

 * *Files 18% similar despite different names*

```diff
@@ -39,17 +39,19 @@
         self.assertEqual(self.log.author, "human")
 
 
 class TestType(unittest.TestCase):
     def test_from_filename(self):
         with self.subTest("valid types"):
             self.assertEqual(Type.found_it, Type.from_filename("2"))
+            self.assertEqual(Type.archive, Type.from_filename("5"))
             self.assertEqual(Type.visit, Type.from_filename("75"))
 
         with self.subTest("special valid types"):
             self.assertEqual(Type.visit, Type.from_filename("1001"))
             self.assertEqual(Type.publish_listing, Type.from_filename("1003"))
+            self.assertEqual(Type.archive, Type.from_filename("6"))
             self.assertEqual(Type.unarchive, Type.from_filename("1"))
 
         with self.subTest("invalid type"):
             with self.assertRaises(PycachingValueError):
                 Type.from_filename("6666")
```

### Comparing `pycaching-4.4.1/test/test_trackable.py` & `pycaching-4.4.2/test/test_trackable.py`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/test/test_util.py` & `pycaching-4.4.2/test/test_util.py`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.test_get_logged_user.json` & `pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.test_get_logged_user.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.test_login.json` & `pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.test_login.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.test_login_bad_credentials.json` & `pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.test_login_bad_credentials.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.test_login_twice_with_valid_credentials.json` & `pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.test_login_twice_with_valid_credentials.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.test_logout.json` & `pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.test_logout.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/tests_new/cassettes/tests_new.test_geocaching.test_logout_when_relogin_is_attempted_with_invalid_credentials.json` & `pycaching-4.4.2/tests_new/cassettes/tests_new.test_geocaching.test_logout_when_relogin_is_attempted_with_invalid_credentials.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/tests_new/cassettes/tests_new.test_shortcuts.test_login.json` & `pycaching-4.4.2/tests_new/cassettes/tests_new.test_shortcuts.test_login.json`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/tests_new/conftest.py` & `pycaching-4.4.2/tests_new/conftest.py`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/tests_new/test_geocaching.py` & `pycaching-4.4.2/tests_new/test_geocaching.py`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/tests_new/test_shortcuts.py` & `pycaching-4.4.2/tests_new/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `pycaching-4.4.1/PKG-INFO` & `pycaching-4.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycaching
-Version: 4.4.1
+Version: 4.4.2
 Summary: Geocaching.com site crawler. Provides tools for searching, fetching caches and geocoding.
 Keywords: geocaching,crawler,geocache,cache,search,geocode,travelbug
 Author-email: Tomas Bedrich <ja@tbedrich.cz>
 Requires-Python: >= 3.5
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
```


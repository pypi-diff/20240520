# Comparing `tmp/ytmusicapi-1.7.1.tar.gz` & `tmp/ytmusicapi-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytmusicapi-1.7.1.tar", last modified: Sat May 11 16:45:32 2024, max compression
+gzip compressed data, was "ytmusicapi-1.7.2.tar", last modified: Mon May 20 19:57:38 2024, max compression
```

## Comparing `ytmusicapi-1.7.1.tar` & `ytmusicapi-1.7.2.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.624338 ytmusicapi-1.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.600338 ytmusicapi-1.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.600338 ytmusicapi-1.7.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.600338 ytmusicapi-1.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.github/workflows/docsbuild.yml
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.github/workflows/pdm.yml
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-11 16:45:32.620338 ytmusicapi-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.600338 ytmusicapi-1.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.600338 ytmusicapi-1.7.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/source/reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/source/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.600338 ytmusicapi-1.7.1/docs/source/setup/
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/source/setup/browser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/source/setup/headers_auth.json.example
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/source/setup/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/source/setup/oauth.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)    61554 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/pdm.lock
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 16:45:32.624338 ytmusicapi-1.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.604338 ytmusicapi-1.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.604338 ytmusicapi-1.7.1/tests/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/auth/test_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/auth/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.604338 ytmusicapi-1.7.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   226650 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/data/2024_03_get_album.json
--rw-r--r--   0 runner    (1001) docker     (127)  1039226 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/data/2024_03_get_playlist.json
--rw-r--r--   0 runner    (1001) docker     (127)  1004367 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/data/2024_03_get_playlist_public.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.608338 ytmusicapi-1.7.1/tests/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/mixins/test_browsing.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/mixins/test_explore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/mixins/test_library.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/mixins/test_playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/mixins/test_podcasts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/mixins/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/mixins/test_uploads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/mixins/test_watch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.608338 ytmusicapi-1.7.1/tests/setup/
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/setup/setup_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/test.example.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/tests/test_ytmusic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.608338 ytmusicapi-1.7.1/ytmusicapi/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.612338 ytmusicapi-1.7.1/ytmusicapi/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/auth/browser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.612338 ytmusicapi-1.7.1/ytmusicapi/auth/oauth/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/auth/oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/auth/oauth/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/auth/oauth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/auth/oauth/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/auth/oauth/token.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/auth/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/continuations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.612338 ytmusicapi-1.7.1/ytmusicapi/locales/
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.592338 ytmusicapi-1.7.1/ytmusicapi/locales/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.612338 ytmusicapi-1.7.1/ytmusicapi/locales/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/ar/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/ar/LC_MESSAGES/base.po
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/base.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.592338 ytmusicapi-1.7.1/ytmusicapi/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.612338 ytmusicapi-1.7.1/ytmusicapi/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/de/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/de/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.592338 ytmusicapi-1.7.1/ytmusicapi/locales/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.612338 ytmusicapi-1.7.1/ytmusicapi/locales/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/en/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/en/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.612338 ytmusicapi-1.7.1/ytmusicapi/locales/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/es/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/es/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.612338 ytmusicapi-1.7.1/ytmusicapi/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/fr/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/fr/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/hi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.612338 ytmusicapi-1.7.1/ytmusicapi/locales/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/hi/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/hi/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.616338 ytmusicapi-1.7.1/ytmusicapi/locales/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/it/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/it/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.616338 ytmusicapi-1.7.1/ytmusicapi/locales/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/ja/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/ja/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.616338 ytmusicapi-1.7.1/ytmusicapi/locales/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/ko/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/ko/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.616338 ytmusicapi-1.7.1/ytmusicapi/locales/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/nl/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/nl/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.616338 ytmusicapi-1.7.1/ytmusicapi/locales/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/pt/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/pt/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.616338 ytmusicapi-1.7.1/ytmusicapi/locales/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/ru/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/ru/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.616338 ytmusicapi-1.7.1/ytmusicapi/locales/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/tr/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/tr/LC_MESSAGES/base.po
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/update_mo.sh
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/update_po.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/ur/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.616338 ytmusicapi-1.7.1/ytmusicapi/locales/ur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/ur/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/ur/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.616338 ytmusicapi-1.7.1/ytmusicapi/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.596338 ytmusicapi-1.7.1/ytmusicapi/locales/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.616338 ytmusicapi-1.7.1/ytmusicapi/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.620338 ytmusicapi-1.7.1/ytmusicapi/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    39178 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/browsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/explore.py
--rw-r--r--   0 runner    (1001) docker     (127)    17492 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/library.py
--rw-r--r--   0 runner    (1001) docker     (127)    20529 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/podcasts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12101 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/uploads.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/mixins/watch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.620338 ytmusicapi-1.7.1/ytmusicapi/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/albums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/browsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/explore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/podcasts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/songs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/uploads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/parsers/watch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-05-11 16:45:27.000000 ytmusicapi-1.7.1/ytmusicapi/ytmusic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:45:32.620338 ytmusicapi-1.7.1/ytmusicapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-11 16:45:32.000000 ytmusicapi-1.7.1/ytmusicapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-11 16:45:32.000000 ytmusicapi-1.7.1/ytmusicapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 16:45:32.000000 ytmusicapi-1.7.1/ytmusicapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-11 16:45:32.000000 ytmusicapi-1.7.1/ytmusicapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-11 16:45:32.000000 ytmusicapi-1.7.1/ytmusicapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-11 16:45:32.000000 ytmusicapi-1.7.1/ytmusicapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.735709 ytmusicapi-1.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.711708 ytmusicapi-1.7.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.711708 ytmusicapi-1.7.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.711708 ytmusicapi-1.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.github/workflows/docsbuild.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.github/workflows/pdm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-20 19:57:38.735709 ytmusicapi-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.711708 ytmusicapi-1.7.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.715708 ytmusicapi-1.7.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/source/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/source/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.715708 ytmusicapi-1.7.2/docs/source/setup/
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/source/setup/browser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/source/setup/headers_auth.json.example
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/source/setup/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/source/setup/oauth.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    61554 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/pdm.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:57:38.735709 ytmusicapi-1.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.715708 ytmusicapi-1.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/tests/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.715708 ytmusicapi-1.7.2/tests/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/tests/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/tests/auth/test_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/tests/auth/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-20 19:57:33.000000 ytmusicapi-1.7.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.719708 ytmusicapi-1.7.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   226650 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/data/2024_03_get_album.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1039226 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/data/2024_03_get_playlist.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1004367 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/data/2024_03_get_playlist_public.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.723708 ytmusicapi-1.7.2/tests/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/mixins/test_browsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/mixins/test_explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/mixins/test_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/mixins/test_playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/mixins/test_podcasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/mixins/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/mixins/test_uploads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/mixins/test_watch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.723708 ytmusicapi-1.7.2/tests/setup/
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/setup/setup_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/test.example.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/tests/test_ytmusic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.723708 ytmusicapi-1.7.2/ytmusicapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.723708 ytmusicapi-1.7.2/ytmusicapi/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/auth/browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.727708 ytmusicapi-1.7.2/ytmusicapi/auth/oauth/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/auth/oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/auth/oauth/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/auth/oauth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/auth/oauth/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/auth/oauth/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/auth/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/continuations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.727708 ytmusicapi-1.7.2/ytmusicapi/locales/
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.727708 ytmusicapi-1.7.2/ytmusicapi/locales/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/ar/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/ar/LC_MESSAGES/base.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/base.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.727708 ytmusicapi-1.7.2/ytmusicapi/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/de/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/de/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.727708 ytmusicapi-1.7.2/ytmusicapi/locales/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/en/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/en/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.727708 ytmusicapi-1.7.2/ytmusicapi/locales/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/es/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/es/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.727708 ytmusicapi-1.7.2/ytmusicapi/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/fr/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/fr/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/hi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.727708 ytmusicapi-1.7.2/ytmusicapi/locales/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/hi/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/hi/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.727708 ytmusicapi-1.7.2/ytmusicapi/locales/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/it/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/it/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.727708 ytmusicapi-1.7.2/ytmusicapi/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/ja/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/ja/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.731708 ytmusicapi-1.7.2/ytmusicapi/locales/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/ko/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/ko/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.731708 ytmusicapi-1.7.2/ytmusicapi/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/nl/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/nl/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.731708 ytmusicapi-1.7.2/ytmusicapi/locales/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/pt/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/pt/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.731708 ytmusicapi-1.7.2/ytmusicapi/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/ru/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/ru/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.731708 ytmusicapi-1.7.2/ytmusicapi/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/tr/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/tr/LC_MESSAGES/base.po
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/update_mo.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/update_po.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/ur/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.731708 ytmusicapi-1.7.2/ytmusicapi/locales/ur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/ur/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/ur/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.707708 ytmusicapi-1.7.2/ytmusicapi/locales/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.731708 ytmusicapi-1.7.2/ytmusicapi/locales/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.711708 ytmusicapi-1.7.2/ytmusicapi/locales/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.731708 ytmusicapi-1.7.2/ytmusicapi/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.735709 ytmusicapi-1.7.2/ytmusicapi/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39178 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/browsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17492 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20529 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/podcasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12370 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/uploads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/mixins/watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.735709 ytmusicapi-1.7.2/ytmusicapi/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/albums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/browsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/podcasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/songs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/uploads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/parsers/watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-05-20 19:57:34.000000 ytmusicapi-1.7.2/ytmusicapi/ytmusic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:57:38.735709 ytmusicapi-1.7.2/ytmusicapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-20 19:57:38.000000 ytmusicapi-1.7.2/ytmusicapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-20 19:57:38.000000 ytmusicapi-1.7.2/ytmusicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:57:38.000000 ytmusicapi-1.7.2/ytmusicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 19:57:38.000000 ytmusicapi-1.7.2/ytmusicapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 19:57:38.000000 ytmusicapi-1.7.2/ytmusicapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 19:57:38.000000 ytmusicapi-1.7.2/ytmusicapi.egg-info/top_level.txt
```

### Comparing `ytmusicapi-1.7.1/.github/ISSUE_TEMPLATE/bug_report.md` & `ytmusicapi-1.7.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/.github/ISSUE_TEMPLATE/feature_request.md` & `ytmusicapi-1.7.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/.github/dependabot.yml` & `ytmusicapi-1.7.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/.github/workflows/coverage.yml` & `ytmusicapi-1.7.2/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/.github/workflows/docsbuild.yml` & `ytmusicapi-1.7.2/.github/workflows/docsbuild.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/.github/workflows/lint.yml` & `ytmusicapi-1.7.2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/.github/workflows/pythonpublish.yml` & `ytmusicapi-1.7.2/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/CONTRIBUTING.rst` & `ytmusicapi-1.7.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/LICENSE` & `ytmusicapi-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/PKG-INFO` & `ytmusicapi-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytmusicapi
-Version: 1.7.1
+Version: 1.7.2
 Summary: Unofficial API for YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ytmusicapi-1.7.1/README.rst` & `ytmusicapi-1.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/docs/Makefile` & `ytmusicapi-1.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/docs/make.bat` & `ytmusicapi-1.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/docs/source/conf.py` & `ytmusicapi-1.7.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/docs/source/faq.rst` & `ytmusicapi-1.7.2/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/docs/source/index.rst` & `ytmusicapi-1.7.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/docs/source/reference.rst` & `ytmusicapi-1.7.2/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/docs/source/setup/browser.rst` & `ytmusicapi-1.7.2/docs/source/setup/browser.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/docs/source/usage.rst` & `ytmusicapi-1.7.2/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/pdm.lock` & `ytmusicapi-1.7.2/pdm.lock`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/pyproject.toml` & `ytmusicapi-1.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/tests/README.rst` & `ytmusicapi-1.7.2/tests/README.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/tests/auth/test_browser.py` & `ytmusicapi-1.7.2/tests/auth/test_browser.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/tests/auth/test_oauth.py` & `ytmusicapi-1.7.2/tests/auth/test_oauth.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/tests/conftest.py` & `ytmusicapi-1.7.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/tests/data/2024_03_get_album.json` & `ytmusicapi-1.7.2/tests/data/2024_03_get_album.json`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/tests/data/2024_03_get_playlist.json` & `ytmusicapi-1.7.2/tests/data/2024_03_get_playlist.json`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/tests/data/2024_03_get_playlist_public.json` & `ytmusicapi-1.7.2/tests/data/2024_03_get_playlist_public.json`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/tests/mixins/test_browsing.py` & `ytmusicapi-1.7.2/tests/mixins/test_browsing.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/tests/mixins/test_explore.py` & `ytmusicapi-1.7.2/tests/mixins/test_explore.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/tests/mixins/test_library.py` & `ytmusicapi-1.7.2/tests/mixins/test_library.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/tests/mixins/test_playlists.py` & `ytmusicapi-1.7.2/tests/mixins/test_playlists.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/tests/mixins/test_podcasts.py` & `ytmusicapi-1.7.2/tests/mixins/test_podcasts.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/tests/mixins/test_search.py` & `ytmusicapi-1.7.2/tests/mixins/test_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,18 @@
         results = yt_auth.search("Martin Stig Andersen - Deteriation", ignore_spelling=True)
         assert len(results) > 0
 
     def test_search_localized(self):
         yt_local = YTMusic(language="it")
         results = yt_local.search("ABBA")
         assert all(result["resultType"] in ALL_RESULT_TYPES for result in results)
+        assert len([x for x in results if x["resultType"] == "album"]) <= 10  # album is default fallback
+
+        results = yt_local.search("ABBA", filter="songs")
+        assert all(item["resultType"] == "song" for item in results)
 
     def test_search_filters(self, yt_auth):
         query = "hip hop playlist"
         results = yt_auth.search(query, filter="songs")
         assert len(results) > 10
         assert all(item["resultType"] == "song" for item in results)
         results = yt_auth.search(query, filter="videos")
```

### Comparing `ytmusicapi-1.7.1/tests/mixins/test_uploads.py` & `ytmusicapi-1.7.2/tests/mixins/test_uploads.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/tests/mixins/test_watch.py` & `ytmusicapi-1.7.2/tests/mixins/test_watch.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/tests/setup/setup_account.py` & `ytmusicapi-1.7.2/tests/setup/setup_account.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/tests/test.example.cfg` & `ytmusicapi-1.7.2/tests/test.example.cfg`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/auth/browser.py` & `ytmusicapi-1.7.2/ytmusicapi/auth/browser.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/auth/oauth/credentials.py` & `ytmusicapi-1.7.2/ytmusicapi/auth/oauth/credentials.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/auth/oauth/models.py` & `ytmusicapi-1.7.2/ytmusicapi/auth/oauth/models.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/auth/oauth/token.py` & `ytmusicapi-1.7.2/ytmusicapi/auth/oauth/token.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/auth/types.py` & `ytmusicapi-1.7.2/ytmusicapi/auth/types.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/constants.py` & `ytmusicapi-1.7.2/ytmusicapi/constants.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/continuations.py` & `ytmusicapi-1.7.2/ytmusicapi/continuations.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/helpers.py` & `ytmusicapi-1.7.2/ytmusicapi/helpers.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/README.rst` & `ytmusicapi-1.7.2/ytmusicapi/locales/README.rst`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/ar/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.2/ytmusicapi/locales/ar/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/ar/LC_MESSAGES/base.po` & `ytmusicapi-1.7.2/ytmusicapi/locales/ar/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/base.pot` & `ytmusicapi-1.7.2/ytmusicapi/locales/base.pot`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/de/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.2/ytmusicapi/locales/de/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/de/LC_MESSAGES/base.po` & `ytmusicapi-1.7.2/ytmusicapi/locales/de/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/en/LC_MESSAGES/base.po` & `ytmusicapi-1.7.2/ytmusicapi/locales/en/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/es/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.2/ytmusicapi/locales/es/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/es/LC_MESSAGES/base.po` & `ytmusicapi-1.7.2/ytmusicapi/locales/es/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/fr/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.2/ytmusicapi/locales/fr/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/fr/LC_MESSAGES/base.po` & `ytmusicapi-1.7.2/ytmusicapi/locales/fr/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/hi/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.2/ytmusicapi/locales/hi/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/hi/LC_MESSAGES/base.po` & `ytmusicapi-1.7.2/ytmusicapi/locales/hi/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/it/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.2/ytmusicapi/locales/it/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/it/LC_MESSAGES/base.po` & `ytmusicapi-1.7.2/ytmusicapi/locales/it/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/ja/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.2/ytmusicapi/locales/ja/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/ja/LC_MESSAGES/base.po` & `ytmusicapi-1.7.2/ytmusicapi/locales/ja/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/ko/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.2/ytmusicapi/locales/ko/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/ko/LC_MESSAGES/base.po` & `ytmusicapi-1.7.2/ytmusicapi/locales/ko/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/nl/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.2/ytmusicapi/locales/nl/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/nl/LC_MESSAGES/base.po` & `ytmusicapi-1.7.2/ytmusicapi/locales/nl/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/pt/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.2/ytmusicapi/locales/pt/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/pt/LC_MESSAGES/base.po` & `ytmusicapi-1.7.2/ytmusicapi/locales/pt/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/ru/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.2/ytmusicapi/locales/ru/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/ru/LC_MESSAGES/base.po` & `ytmusicapi-1.7.2/ytmusicapi/locales/ru/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/tr/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.2/ytmusicapi/locales/tr/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/tr/LC_MESSAGES/base.po` & `ytmusicapi-1.7.2/ytmusicapi/locales/tr/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/ur/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.2/ytmusicapi/locales/ur/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/ur/LC_MESSAGES/base.po` & `ytmusicapi-1.7.2/ytmusicapi/locales/ur/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.2/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.po` & `ytmusicapi-1.7.2/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo` & `ytmusicapi-1.7.2/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po` & `ytmusicapi-1.7.2/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/mixins/_protocol.py` & `ytmusicapi-1.7.2/ytmusicapi/mixins/_protocol.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/mixins/_utils.py` & `ytmusicapi-1.7.2/ytmusicapi/mixins/_utils.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/mixins/browsing.py` & `ytmusicapi-1.7.2/ytmusicapi/mixins/browsing.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/mixins/explore.py` & `ytmusicapi-1.7.2/ytmusicapi/mixins/explore.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/mixins/library.py` & `ytmusicapi-1.7.2/ytmusicapi/mixins/library.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/mixins/playlists.py` & `ytmusicapi-1.7.2/ytmusicapi/mixins/playlists.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/mixins/podcasts.py` & `ytmusicapi-1.7.2/ytmusicapi/mixins/podcasts.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/mixins/search.py` & `ytmusicapi-1.7.2/ytmusicapi/mixins/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -201,46 +201,52 @@
         # set filter for parser
         if filter and "playlists" in filter:
             filter = "playlists"
         elif scope == scopes[1]:
             filter = scopes[1]
 
         for res in section_list:
+            result_type = category = None
+            search_result_types = self.parser.get_search_result_types()
+
             if "musicCardShelfRenderer" in res:
                 top_result = parse_top_result(
                     res["musicCardShelfRenderer"], self.parser.get_search_result_types()
                 )
                 search_results.append(top_result)
                 if not (shelf_contents := nav(res, ["musicCardShelfRenderer", "contents"], True)):
                     continue
-                type = category = None
                 # if "more from youtube" is present, remove it - it's not parseable
                 if "messageRenderer" in shelf_contents[0]:
                     category = nav(shelf_contents.pop(0), ["messageRenderer", *TEXT_RUN_TEXT])
 
             elif "musicShelfRenderer" in res:
                 shelf_contents = res["musicShelfRenderer"]["contents"]
                 category = nav(res, MUSIC_SHELF + TITLE_TEXT, True)
-                type_filter = filter or category
 
-                type = type_filter[:-1].lower() if type_filter else None
+                # if we know the filter it's easy to set the result type
+                # unfortunately uploads is modeled as a filter (historical reasons),
+                #  so we take care to not set the result type for that scope
+                if filter and not scope == scopes[1]:
+                    result_type = filter[:-1].lower()
 
             else:
                 continue
 
-            search_result_types = self.parser.get_search_result_types()
-            search_results.extend(parse_search_results(shelf_contents, search_result_types, type, category))
+            search_results.extend(
+                parse_search_results(shelf_contents, search_result_types, result_type, category)
+            )
 
             if filter:  # if filter is set, there are continuations
 
                 def request_func(additionalParams):
                     return self._send_request(endpoint, body, additionalParams)
 
                 def parse_func(contents):
-                    return parse_search_results(contents, search_result_types, type, category)
+                    return parse_search_results(contents, search_result_types, result_type, category)
 
                 search_results.extend(
                     get_continuations(
                         res["musicShelfRenderer"],
                         "musicShelfContinuation",
                         limit - len(search_results),
                         request_func,
```

### Comparing `ytmusicapi-1.7.1/ytmusicapi/mixins/uploads.py` & `ytmusicapi-1.7.2/ytmusicapi/mixins/uploads.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/mixins/watch.py` & `ytmusicapi-1.7.2/ytmusicapi/mixins/watch.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/navigation.py` & `ytmusicapi-1.7.2/ytmusicapi/navigation.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/parsers/_utils.py` & `ytmusicapi-1.7.2/ytmusicapi/parsers/_utils.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/parsers/albums.py` & `ytmusicapi-1.7.2/ytmusicapi/parsers/albums.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/parsers/browsing.py` & `ytmusicapi-1.7.2/ytmusicapi/parsers/browsing.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/parsers/explore.py` & `ytmusicapi-1.7.2/ytmusicapi/parsers/explore.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/parsers/i18n.py` & `ytmusicapi-1.7.2/ytmusicapi/parsers/i18n.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/parsers/library.py` & `ytmusicapi-1.7.2/ytmusicapi/parsers/library.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/parsers/playlists.py` & `ytmusicapi-1.7.2/ytmusicapi/parsers/playlists.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/parsers/podcasts.py` & `ytmusicapi-1.7.2/ytmusicapi/parsers/podcasts.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/parsers/search.py` & `ytmusicapi-1.7.2/ytmusicapi/parsers/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,29 +57,27 @@
 
 
 def parse_search_result(data, search_result_types, result_type, category):
     default_offset = (not result_type or result_type == "album") * 2
     search_result = {"category": category}
     video_type = nav(data, [*PLAY_BUTTON, "playNavigationEndpoint", *NAVIGATION_VIDEO_TYPE], True)
 
-    # try to determine the result type based on the first run
-    if result_type not in ALL_RESULT_TYPES:  # i.e. localized result_type
-        result_type = get_search_result_type(get_item_text(data, 1), search_result_types)
-
     # determine result type based on browseId
     #  if there was no category title (i.e. for extra results in Top Result)
     if not result_type:
         if browse_id := nav(data, NAVIGATION_BROWSE_ID, True):
             mapping = {
-                "VMPL": "playlist",
+                "VM": "playlist",
                 "RD": "playlist",
+                "VL": "playlist",
                 "MPLA": "artist",
                 "MPRE": "album",
                 "MPSP": "podcast",
                 "MPED": "episode",
+                "UC": "artist",
             }
             result_type = next(
                 iter(type for prefix, type in mapping.items() if browse_id.startswith(prefix)), None
             )
         else:
             result_type = "song" if video_type == "MUSIC_VIDEO_TYPE_ATV" else "video"
```

### Comparing `ytmusicapi-1.7.1/ytmusicapi/parsers/songs.py` & `ytmusicapi-1.7.2/ytmusicapi/parsers/songs.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/parsers/uploads.py` & `ytmusicapi-1.7.2/ytmusicapi/parsers/uploads.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/parsers/watch.py` & `ytmusicapi-1.7.2/ytmusicapi/parsers/watch.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/setup.py` & `ytmusicapi-1.7.2/ytmusicapi/setup.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi/ytmusic.py` & `ytmusicapi-1.7.2/ytmusicapi/ytmusic.py`

 * *Files identical despite different names*

### Comparing `ytmusicapi-1.7.1/ytmusicapi.egg-info/PKG-INFO` & `ytmusicapi-1.7.2/ytmusicapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytmusicapi
-Version: 1.7.1
+Version: 1.7.2
 Summary: Unofficial API for YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ytmusicapi-1.7.1/ytmusicapi.egg-info/SOURCES.txt` & `ytmusicapi-1.7.2/ytmusicapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*


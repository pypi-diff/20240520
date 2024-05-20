# Comparing `tmp/ccs_govuk_frontend_jinja-1.0.0.tar.gz` & `tmp/ccs_govuk_frontend_jinja-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs_govuk_frontend_jinja-1.0.0.tar", last modified: Wed Apr 24 12:50:48 2024, max compression
+gzip compressed data, was "ccs_govuk_frontend_jinja-1.1.0.tar", last modified: Mon May 20 08:33:00 2024, max compression
```

## Comparing `ccs_govuk_frontend_jinja-1.0.0.tar` & `ccs_govuk_frontend_jinja-1.1.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.326867 ccs_govuk_frontend_jinja-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-24 12:50:48.326867 ccs_govuk_frontend_jinja-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.326867 ccs_govuk_frontend_jinja-1.0.0/ccs_govuk_frontend_jinja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-24 12:50:48.000000 ccs_govuk_frontend_jinja-1.0.0/ccs_govuk_frontend_jinja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-24 12:50:48.000000 ccs_govuk_frontend_jinja-1.0.0/ccs_govuk_frontend_jinja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:50:48.000000 ccs_govuk_frontend_jinja-1.0.0/ccs_govuk_frontend_jinja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 12:50:48.000000 ccs_govuk_frontend_jinja-1.0.0/ccs_govuk_frontend_jinja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 12:50:48.000000 ccs_govuk_frontend_jinja-1.0.0/ccs_govuk_frontend_jinja.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.318867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.318867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.314867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.318867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/accordion/
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/accordion/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.318867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/back-link/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/back-link/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.318867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/breadcrumbs/
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/breadcrumbs/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.318867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/button/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/button/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.318867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/character-count/
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/character-count/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.318867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/checkboxes/
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/checkboxes/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.318867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/cookie-banner/
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/cookie-banner/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.318867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/date-input/
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/date-input/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.318867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/details/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/details/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.318867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/error-message/
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/error-message/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.318867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/error-summary/
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/error-summary/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.318867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/exit-this-page/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/exit-this-page/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/fieldset/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/fieldset/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/file-upload/
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/file-upload/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/footer/
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/footer/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/header/
--rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/header/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/hint/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/hint/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/input/
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/input/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/inset-text/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/inset-text/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/label/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/label/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/notification-banner/
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/notification-banner/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/pagination/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/panel/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/panel/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/password-input/
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/password-input/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/phase-banner/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/phase-banner/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/radios/
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/radios/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/select/
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/select/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/skip-link/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/skip-link/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/summary-list/
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/summary-list/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/table/
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/table/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/tabs/
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/tabs/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/tag/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/tag/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/task-list/
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/task-list/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/textarea/
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/textarea/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/warning-text/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/warning-text/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/macros/
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/macros/attributes.html
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/macros/i18n.html
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/template.html
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-24 12:50:48.326867 ccs_govuk_frontend_jinja-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:50:48.322867 ccs_govuk_frontend_jinja-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-24 12:50:41.000000 ccs_govuk_frontend_jinja-1.0.0/tests/test_components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.832563 ccs_govuk_frontend_jinja-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-05-20 08:33:00.832563 ccs_govuk_frontend_jinja-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.832563 ccs_govuk_frontend_jinja-1.1.0/ccs_govuk_frontend_jinja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-05-20 08:33:00.000000 ccs_govuk_frontend_jinja-1.1.0/ccs_govuk_frontend_jinja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-20 08:33:00.000000 ccs_govuk_frontend_jinja-1.1.0/ccs_govuk_frontend_jinja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 08:33:00.000000 ccs_govuk_frontend_jinja-1.1.0/ccs_govuk_frontend_jinja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 08:33:00.000000 ccs_govuk_frontend_jinja-1.1.0/ccs_govuk_frontend_jinja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 08:33:00.000000 ccs_govuk_frontend_jinja-1.1.0/ccs_govuk_frontend_jinja.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.824563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.824563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.824563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.824563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/accordion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/accordion/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/back-link/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/back-link/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/breadcrumbs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/breadcrumbs/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/button/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/button/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/character-count/
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/character-count/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/checkboxes/
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/checkboxes/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/cookie-banner/
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/cookie-banner/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/date-input/
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/date-input/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/details/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/details/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/error-message/
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/error-message/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/error-summary/
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/error-summary/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/exit-this-page/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/exit-this-page/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/fieldset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/fieldset/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/file-upload/
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/file-upload/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/footer/
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/footer/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/header/
+-rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/header/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/hint/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/hint/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/input/
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/input/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/inset-text/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/inset-text/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/label/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/label/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/notification-banner/
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/notification-banner/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/pagination/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/panel/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/panel/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/password-input/
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/password-input/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.828563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/phase-banner/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/phase-banner/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.832563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/radios/
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/radios/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.832563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/select/
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/select/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.832563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/skip-link/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/skip-link/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.832563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/summary-list/
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/summary-list/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.832563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/table/
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/table/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.832563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/tabs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/tabs/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.832563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/tag/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/tag/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.832563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/task-list/
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/task-list/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.832563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/textarea/
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/textarea/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.832563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/warning-text/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/warning-text/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.832563 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/macros/attributes.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/macros/i18n.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/template.html
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-20 08:33:00.832563 ccs_govuk_frontend_jinja-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:33:00.832563 ccs_govuk_frontend_jinja-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-20 08:32:54.000000 ccs_govuk_frontend_jinja-1.1.0/tests/test_components.py
```

### Comparing `ccs_govuk_frontend_jinja-1.0.0/LICENSE` & `ccs_govuk_frontend_jinja-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/PKG-INFO` & `ccs_govuk_frontend_jinja-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccs-govuk-frontend-jinja
-Version: 1.0.0
+Version: 1.1.0
 Summary: GOV.UK Frontend Jinja Macros
 Home-page: https://github.com/tim-s-ccs/govuk-frontend-jinja
 Author: CCS
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `ccs_govuk_frontend_jinja-1.0.0/README.md` & `ccs_govuk_frontend_jinja-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/ccs_govuk_frontend_jinja.egg-info/PKG-INFO` & `ccs_govuk_frontend_jinja-1.1.0/ccs_govuk_frontend_jinja.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccs-govuk-frontend-jinja
-Version: 1.0.0
+Version: 1.1.0
 Summary: GOV.UK Frontend Jinja Macros
 Home-page: https://github.com/tim-s-ccs/govuk-frontend-jinja
 Author: CCS
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `ccs_govuk_frontend_jinja-1.0.0/ccs_govuk_frontend_jinja.egg-info/SOURCES.txt` & `ccs_govuk_frontend_jinja-1.1.0/ccs_govuk_frontend_jinja.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/accordion/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/accordion/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/breadcrumbs/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/breadcrumbs/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/button/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/button/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/character-count/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/character-count/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/checkboxes/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/checkboxes/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/cookie-banner/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/cookie-banner/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/date-input/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/date-input/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/details/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/details/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/error-message/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/error-message/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/error-summary/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/error-summary/macro.html`

 * *Files 5% similar despite different names*

```diff
@@ -13,25 +13,27 @@
     </h2>
     <div class="govuk-error-summary__body">
       {% if caller or params.descriptionHtml or params.descriptionText %}
       <p>
         {{ caller() if caller else (params.descriptionHtml | safe | trim | indent(8) if params.descriptionHtml else params.descriptionText) }}
       </p>
       {% endif %}
-      <ul class="govuk-list govuk-error-summary__list">
-      {% for item in params.errorList %}
-        <li>
-        {% if item.href %}
-          <a href="{{ item.href }}"
-            {{- govukAttributes(item.attributes) }}>
-            {{- item.html | safe | trim | indent(12) if item.html else item.text -}}
-          </a>
-        {% else %}
-          {{ item.html | safe | trim | indent(10) if item.html else item.text }}
-        {% endif %}
-        </li>
-      {% endfor %}
-      </ul>
+      {% if params.errorList | length %}
+        <ul class="govuk-list govuk-error-summary__list">
+        {% for item in params.errorList %}
+          <li>
+          {% if item.href %}
+            <a href="{{ item.href }}"
+              {{- govukAttributes(item.attributes) }}>
+              {{- item.html | safe | trim | indent(12) if item.html else item.text -}}
+            </a>
+          {% else %}
+            {{ item.html | safe | trim | indent(10) if item.html else item.text }}
+          {% endif %}
+          </li>
+        {% endfor %}
+        </ul>
+      {% endif %}
     </div>
   </div>
 </div>
 {% endmacro %}
```

#### html2text {}

```diff
@@ -7,15 +7,16 @@
 the focusing js at the alert, resulting in information getting missed in screen
 reader announcements #}
 ********** {{{{ ppaarraammss..ttiittlleeHHttmmll || ssaaffee || ttrriimm || iinnddeenntt((66)) iiff ppaarraammss..ttiittlleeHHttmmll eellssee
 ppaarraammss..ttiittlleeTTeexxtt }}}} **********
 {% if caller or params.descriptionHtml or params.descriptionText %}
 {{ caller() if caller else (params.descriptionHtml | safe | trim | indent(8) if
 params.descriptionHtml else params.descriptionText) }}
-{% endif %}
+{% endif %} {% if params.errorList | length %}
     * {% for item in params.errorList %}
     * {% if item.href %} {- govukAttributes(item.attributes) }}> {{- item.html
       | safe | trim | indent(12) if item.html else item.text -}}
 {% else %} {{ item.html | safe | trim | indent(10) if item.html else item.text
 }} {% endif %}
 {% endfor %}
+{% endif %}
 {% endmacro %}
```

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/exit-this-page/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/exit-this-page/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/fieldset/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/fieldset/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/file-upload/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/file-upload/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/footer/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/footer/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/header/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/header/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/input/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/select/macro.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,16 @@
-{% macro govukInput(params) %}
+{% macro govukSelect(params) %}
 {% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes %}
 {% from "govuk_frontend_jinja/components/error-message/macro.html" import govukErrorMessage %}
 {% from "govuk_frontend_jinja/components/hint/macro.html" import govukHint %}
 {% from "govuk_frontend_jinja/components/label/macro.html" import govukLabel %}
 
 {#- a record of other elements that we need to associate with the input using
   aria-describedby – for example hints or error messages -#}
-{% set describedBy = params.describedBy if params.describedBy else "" -%}
-
-{%- set hasPrefix = true if params.prefix and (params.prefix.text or params.prefix.html) else false %}
-{%- set hasSuffix = true if params.suffix and (params.suffix.text or params.suffix.html) else false %}
-{%- set hasBeforeInput = true if params.formGroup and params.formGroup.beforeInput and (params.formGroup.beforeInput.text or params.formGroup.beforeInput.html) else false %}
-{%- set hasAfterInput = true if params.formGroup and params.formGroup.afterInput and (params.formGroup.afterInput.text or params.formGroup.afterInput.html) else false %}
-
-{%- macro _inputElement(params) -%}
-  <input class="govuk-input {%- if params.classes %} {{ params.classes }}{% endif %} {%- if params.errorMessage %} govuk-input--error{% endif %}" id="{{ params.id }}" name="{{ params.name }}" type="{{ params.type | default("text", true) }}"
-    {%- if (params.spellcheck == false) or (params.spellcheck == true) %} spellcheck="{{ params.spellcheck | lower }}"{% endif %}
-    {%- if params.value %} value="{{ params.value }}"{% endif %}
-    {%- if params.disabled %} disabled{% endif %}
-    {%- if describedBy %} aria-describedby="{{ describedBy }}"{% endif %}
-    {%- if params.autocomplete %} autocomplete="{{ params.autocomplete }}"{% endif %}
-    {%- if params.pattern %} pattern="{{ params.pattern }}"{% endif %}
-    {%- if params.inputmode %} inputmode="{{ params.inputmode }}"{% endif %}
-    {%- if params.autocapitalize %} autocapitalize="{{ params.autocapitalize }}"{% endif %}
-    {{- govukAttributes(params.attributes) }}>
-{%- endmacro -%}
-
-{%- macro _affixItem(affix, type) %}
-  <div class="govuk-input__{{ type }} {%- if affix.classes %} {{ affix.classes }}{% endif %}" aria-hidden="true" {{- govukAttributes(affix.attributes) }}>
-    {{- affix.html | safe | trim | indent(4) if affix.html else affix.text -}}
-  </div>
-{%- endmacro -%}
-
+{% set describedBy = params.describedBy if params.describedBy else "" %}
 <div class="govuk-form-group {%- if params.errorMessage %} govuk-form-group--error{% endif %} {%- if params.formGroup and params.formGroup.classes %} {{ params.formGroup.classes }}{% endif %}"
   {{- govukAttributes(params.formGroup.attributes if params.formGroup else {}) }}>
   {{ govukLabel({
     'html': params.label.html,
     'text': params.label.text,
     'classes': params.label.classes,
     'isPageHeading': params.label.isPageHeading,
@@ -61,30 +36,35 @@
     'classes': params.errorMessage.classes,
     'attributes': params.errorMessage.attributes,
     'html': params.errorMessage.html,
     'text': params.errorMessage.text,
     'visuallyHiddenText': params.errorMessage.visuallyHiddenText
   }) | trim | indent(2) }}
 {% endif %}
-
-{%- if hasPrefix or hasSuffix or hasBeforeInput or hasAfterInput %}
-  <div class="govuk-input__wrapper {%- if params.inputWrapper and params.inputWrapper.classes %} {{ params.inputWrapper.classes }}{% endif %}"
-  {{- govukAttributes(params.inputWrapper.attributes if params.inputWrapper else {}) }}>
-    {% if hasBeforeInput %}
-      {{- params.formGroup.beforeInput.html | safe | trim | indent(4, true) if params.formGroup.beforeInput.html else params.formGroup.beforeInput.text }}
-    {% endif %}
-    {% if hasPrefix %}
-      {{- _affixItem(params.prefix, "prefix") | indent(2, true) }}
-    {% endif %}
-    {{ _inputElement(params) }}
-    {% if hasSuffix %}
-      {{- _affixItem(params.suffix, "suffix") | indent(2, true) }}
-    {% endif %}
-    {% if hasAfterInput %}
-      {{- params.formGroup.afterInput.html | safe | trim | indent(4, true) if params.formGroup.afterInput.html else params.formGroup.afterInput.text }}
+{% if params.formGroup and params.formGroup.beforeInput %}
+  {{ params.formGroup.beforeInput.html | safe | trim | indent(2) if params.formGroup.beforeInput.html else params.formGroup.beforeInput.text }}
+{% endif %}
+  <select class="govuk-select
+    {%- if params.classes %} {{ params.classes }}{% endif %}{%- if params.errorMessage %} govuk-select--error{% endif %}" id="{{ params.id }}" name="{{ params.name }}"
+    {%- if params.disabled %} disabled{% endif %}
+    {%- if describedBy %} aria-describedby="{{ describedBy }}"{% endif %}
+    {{- govukAttributes(params.attributes) }}>
+    {% if 'items' in params and params['items'] | length %}
+      {% for item in params['items'] %}
+        {% if item %}
+          {# Allow selecting by text content (the value for an option when no value attribute is specified) #}
+          {% set effectiveValue = item.value | default(item.text) %}
+          <option {%- if item.value is not undefined %} value="{{ item.value }}"{% endif %}
+            {{- govukAttributes(item.attributes) }}
+            {{-" selected" if item.selected | default((effectiveValue == params.value and item.selected != false) if params.value else false, true) }}
+            {{-" disabled" if item.disabled }}>
+            {{- item.text -}}
+          </option>
+        {% endif %}
+      {% endfor %}
     {% endif %}
-  </div>
-{% else %}
-  {{ _inputElement(params) }}
+  </select>
+{% if params.formGroup and params.formGroup.afterInput %}
+  {{ params.formGroup.afterInput.html | safe | trim | indent(2) if params.formGroup.afterInput.html else params.formGroup.afterInput.text }}
 {% endif %}
 </div>
 {% endmacro %}
```

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/label/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/label/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/notification-banner/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/notification-banner/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/pagination/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/pagination/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/panel/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/panel/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/password-input/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/password-input/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/phase-banner/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/phase-banner/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/radios/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/radios/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/summary-list/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/summary-list/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/table/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/table/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/tabs/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/tabs/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/task-list/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/task-list/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/textarea/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/textarea/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/components/warning-text/macro.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/components/warning-text/macro.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/macros/attributes.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/macros/attributes.html`

 * *Files 3% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         "optional": false
       } %}
 
       {#- Output ` name` only (no value) for boolean attributes -#}
       {% if options.optional is true and options.value is true %}
         {% set ns.attributesHtml = '{} {}'.format(ns.attributesHtml, name | escape) %}
       {#- Skip optional empty attributes or output ` name="value"` pair by default -#}
-      {% elif (options.optional is true and options.value not in [undefined, null, false]) or options.optional is not true %}
+      {% elif (options.optional is true and options.value not in [undefined, null] and options.value is not false) or options.optional is not true %}
         {% set ns.attributesHtml = '{} {}="{}"'.format(ns.attributesHtml, name | escape, options.value | escape) %}
       {% endif %}
     {% endfor %}
   {% endif -%}
 
   {{- ns.attributesHtml | safe -}}
 {%- endmacro %}
```

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/macros/i18n.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/macros/i18n.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/govuk_frontend_jinja/templates/template.html` & `ccs_govuk_frontend_jinja-1.1.0/govuk_frontend_jinja/templates/template.html`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/setup.py` & `ccs_govuk_frontend_jinja-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `ccs_govuk_frontend_jinja-1.0.0/tests/test_components.py` & `ccs_govuk_frontend_jinja-1.1.0/tests/test_components.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,17 @@
     (r"\s{2,}", ""),
     (r"\n", ""),
 ]
 
 STRING_REPLACERS = [
     ('value="False"', 'value="false"'),
     ('attribute="True"', 'attribute="true"'),
+    ("inputclass", "input class"),
+    ('spellcheck="True"', 'spellcheck="true"'),
+    ('spellcheck="False"', 'spellcheck="false"'),
 ]
 
 
 def html_to_one_line(html: str):
     for replacer in REGEX_REPLACERS:
         html = re.sub(*replacer, html)
```


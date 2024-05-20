# Comparing `tmp/ccs-digitalmarketplace-frontend-jinja-2.5.0.tar.gz` & `tmp/ccs-digitalmarketplace-frontend-jinja-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs-digitalmarketplace-frontend-jinja-2.5.0.tar", last modified: Thu May 16 11:33:28 2024, max compression
+gzip compressed data, was "ccs-digitalmarketplace-frontend-jinja-2.6.0.tar", last modified: Mon May 20 08:56:00 2024, max compression
```

## Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0.tar` & `ccs-digitalmarketplace-frontend-jinja-2.6.0.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.551092 ccs-digitalmarketplace-frontend-jinja-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-16 11:33:28.551092 ccs-digitalmarketplace-frontend-jinja-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.543092 ccs-digitalmarketplace-frontend-jinja-2.5.0/app/
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.543092 ccs-digitalmarketplace-frontend-jinja-2.5.0/ccs_digitalmarketplace_frontend_jinja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-16 11:33:28.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/ccs_digitalmarketplace_frontend_jinja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-16 11:33:28.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/ccs_digitalmarketplace_frontend_jinja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 11:33:28.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/ccs_digitalmarketplace_frontend_jinja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-16 11:33:28.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/ccs_digitalmarketplace_frontend_jinja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 11:33:28.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/ccs_digitalmarketplace_frontend_jinja.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.543092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.543092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.543092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.543092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/alert/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/alert/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.543092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/attachment/
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/attachment/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.543092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/banner/
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/banner/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.543092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/character-count-from-form/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/character-count-from-form/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.543092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/checkboxes-from-form/
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/checkboxes-from-form/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.543092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/compliance-communication-attachment-row/
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/compliance-communication-attachment-row/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.543092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/compliance-communication-attachments/
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/compliance-communication-attachments/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/cookie-banner/
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/cookie-banner/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/documents/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/documents/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/file-upload-from-form/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/file-upload-from-form/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/footer/
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/footer/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/header/
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/header/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/input-from-form/
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/input-from-form/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/list-input/
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/list-input/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/option-select/
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/option-select/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/previous-next-pagination/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/previous-next-pagination/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.539092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/boolean/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/boolean/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/character-count/
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/character-count/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/checkbox-tree/
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/checkbox-tree/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/checkboxes/
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/checkboxes/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/date/
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/date/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/format-hint/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/format-hint/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/list/
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/list/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/multiquestion/
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/multiquestion/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/number/
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/number/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/pricing/
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/pricing/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/radios/
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/radios/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/text/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/text/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/upload/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/upload/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/radios-from-form/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/radios-from-form/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/search-box/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/search-box/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.547092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/select/
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/select/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.551092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/select-country-from-form/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/select-country-from-form/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.551092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.543092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.551092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/boolean/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/boolean/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.551092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/checkbox-tree/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/checkbox-tree/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.551092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/list/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/list/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.551092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/list-items/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/list-items/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.551092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/multiquestion/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/multiquestion/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.551092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/number/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/number/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.551092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/radios/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/radios/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.551092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/service-id/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/service-id/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.551092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/text/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/text/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.551092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/upload/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/upload/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.551092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/system-message-banner/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/system-message-banner/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.551092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/temporary-message/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/temporary-message/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.551092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/errors/400.html
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/errors/403.html
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/errors/404.html
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/errors/410.html
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/errors/500.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:33:28.551092 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/layouts/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/layouts/_custom_dimensions.html
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/layouts/_site_verification.html
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 11:33:28.551092 ccs-digitalmarketplace-frontend-jinja-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-16 11:33:19.000000 ccs-digitalmarketplace-frontend-jinja-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.916844 ccs-digitalmarketplace-frontend-jinja-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-20 08:56:00.916844 ccs-digitalmarketplace-frontend-jinja-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.904844 ccs-digitalmarketplace-frontend-jinja-2.6.0/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/ccs_digitalmarketplace_frontend_jinja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-20 08:56:00.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/ccs_digitalmarketplace_frontend_jinja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-20 08:56:00.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/ccs_digitalmarketplace_frontend_jinja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 08:56:00.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/ccs_digitalmarketplace_frontend_jinja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-20 08:56:00.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/ccs_digitalmarketplace_frontend_jinja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 08:56:00.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/ccs_digitalmarketplace_frontend_jinja.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.904844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.904844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/alert/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/alert/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/attachment/
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/attachment/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/banner/
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/banner/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/character-count-from-form/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/character-count-from-form/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/checkboxes-from-form/
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/checkboxes-from-form/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/compliance-communication-attachment-row/
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/compliance-communication-attachment-row/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/compliance-communication-attachments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/compliance-communication-attachments/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/cookie-banner/
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/cookie-banner/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/documents/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/file-upload-from-form/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/file-upload-from-form/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/footer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/footer/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/header/
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/header/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/input-from-form/
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/input-from-form/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/list-input/
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/list-input/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/option-select/
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/option-select/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/previous-next-pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/previous-next-pagination/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.904844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/boolean/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/boolean/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/character-count/
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/character-count/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/checkbox-tree/
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/checkbox-tree/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/checkboxes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/checkboxes/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/date/
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/date/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/format-hint/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/format-hint/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.908844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/list/
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/list/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/multiquestion/
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/multiquestion/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/number/
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/number/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/pricing/
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/pricing/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/radios/
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/radios/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/text/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/text/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/upload/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/upload/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/radios-from-form/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/radios-from-form/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/search-box/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/search-box/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/select/
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/select/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/select-country-from-form/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/select-country-from-form/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.904844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/boolean/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/boolean/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/checkbox-tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/checkbox-tree/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/list/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/list/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/list-items/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/list-items/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/multiquestion/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/multiquestion/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/number/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/number/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/radios/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/radios/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/service-id/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/service-id/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/text/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/upload/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/upload/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/system-message-banner/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/system-message-banner/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.912844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/temporary-message/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/temporary-message/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.916844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/errors/400.html
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/errors/403.html
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/errors/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/errors/410.html
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/errors/500.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:56:00.916844 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/layouts/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/layouts/_custom_dimensions.html
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/layouts/_site_verification.html
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 08:56:00.916844 ccs-digitalmarketplace-frontend-jinja-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-20 08:55:53.000000 ccs-digitalmarketplace-frontend-jinja-2.6.0/setup.py
```

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/LICENCE` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/LICENCE`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/README.md` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/app/__init__.py` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/ccs_digitalmarketplace_frontend_jinja.egg-info/SOURCES.txt` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/ccs_digitalmarketplace_frontend_jinja.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/alert/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/alert/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/attachment/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/attachment/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/banner/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/banner/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/character-count-from-form/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/character-count-from-form/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/checkboxes-from-form/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/checkboxes-from-form/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/compliance-communication-attachment-row/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/compliance-communication-attachment-row/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/compliance-communication-attachments/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/compliance-communication-attachments/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/cookie-banner/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/cookie-banner/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/documents/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/documents/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/file-upload-from-form/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/file-upload-from-form/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/footer/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/footer/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/header/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/header/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/input-from-form/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/input-from-form/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/list-input/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/list-input/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/option-select/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/option-select/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/previous-next-pagination/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/previous-next-pagination/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/boolean/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/boolean/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/character-count/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/character-count/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/checkbox-tree/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/checkbox-tree/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/checkboxes/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/checkboxes/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/date/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/date/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/list/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/list/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/multiquestion/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/multiquestion/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/number/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/number/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/pricing/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/pricing/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/radios/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/radios/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/text/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/text/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/upload/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/question/macros/upload/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/radios-from-form/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/radios-from-form/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/search-box/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/search-box/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/select/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/select/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/select-country-from-form/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/select-country-from-form/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/boolean/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/boolean/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/checkbox-tree/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/checkbox-tree/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/list/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/list/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/multiquestion/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/multiquestion/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/radios/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/summary-content/macros/radios/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/components/temporary-message/macro.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/components/temporary-message/macro.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/errors/403.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/errors/403.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/errors/404.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/errors/404.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/errors/410.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/errors/410.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/digitalmarketplace_frontend_jinja/templates/layouts/_custom_dimensions.html` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/digitalmarketplace_frontend_jinja/templates/layouts/_custom_dimensions.html`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-2.5.0/setup.py` & `ccs-digitalmarketplace-frontend-jinja-2.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,12 +27,12 @@
     description='Jinja templates for Digital Marketplace apps.',
     long_description=__doc__,
     packages=find_packages(),
     package_data={'digitalmarketplace_frontend_jinja': components},
     include_package_data=True,
     install_requires=[
         'jinja2>3',
-        'ccs-govuk-frontend-jinja>=1,<2',
+        'ccs-govuk-frontend-jinja>=1.1,<2',
         'ccs-digitalmarketplace-utils>=66.0.1',
     ],
     python_requires=">=3.10,<3.13",
 )
```


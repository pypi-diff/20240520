# Comparing `tmp/switch_api-0.5.6.tar.gz` & `tmp/switch_api-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "switch_api-0.5.6.tar", last modified: Tue May 14 03:33:57 2024, max compression
+gzip compressed data, was "switch_api-0.5.7.tar", last modified: Mon May 20 04:20:00 2024, max compression
```

## Comparing `switch_api-0.5.6.tar` & `switch_api-0.5.7.tar`

### file list

```diff
@@ -1,79 +1,77 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/
--rw-r--r--   0 vsts      (1001) docker     (127)      249 2024-05-14 03:33:49.000000 switch_api-0.5.6/AUTHORS.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    36804 2024-05-14 03:33:49.000000 switch_api-0.5.6/HISTORY.md
--rw-r--r--   0 vsts      (1001) docker     (127)     1093 2024-05-14 03:33:49.000000 switch_api-0.5.6/LICENCE
--rw-r--r--   0 vsts      (1001) docker     (127)       74 2024-05-14 03:33:49.000000 switch_api-0.5.6/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    38078 2024-05-14 03:33:57.927328 switch_api-0.5.6/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      590 2024-05-14 03:33:49.000000 switch_api-0.5.6/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-05-14 03:33:49.000000 switch_api-0.5.6/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       62 2024-05-14 03:33:57.931328 switch_api-0.5.6/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1448 2024-05-14 03:33:49.000000 switch_api-0.5.6/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.923328 switch_api-0.5.6/switch_api/
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.923328 switch_api-0.5.6/switch_api/_authentication/
--rw-r--r--   0 vsts      (1001) docker     (127)      391 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_authentication/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8127 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_authentication/_authentication.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.923328 switch_api-0.5.6/switch_api/_authentication/_credentials_store/
--rw-r--r--   0 vsts      (1001) docker     (127)      393 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_authentication/_credentials_store/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5851 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_authentication/_credentials_store/_credentials_store.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.923328 switch_api-0.5.6/switch_api/_authentication/_msal/
--rw-r--r--   0 vsts      (1001) docker     (127)      361 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_authentication/_msal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8752 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_authentication/_msal/_custom_application.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.923328 switch_api-0.5.6/switch_api/_guide/
--rw-r--r--   0 vsts      (1001) docker     (127)      455 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_guide/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3108 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_guide/main.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2093 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_guide/processor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/_utils/
--rw-r--r--   0 vsts      (1001) docker     (127)      462 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4205 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_utils/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5952 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_utils/_marketplace.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14920 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_utils/_platform.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23502 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_utils/_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/analytics/
--rw-r--r--   0 vsts      (1001) docker     (127)      642 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/analytics/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14655 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/analytics/analytics.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/cache/
--rw-r--r--   0 vsts      (1001) docker     (127)      480 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/cache/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6985 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/cache/cache.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/controls/
--rw-r--r--   0 vsts      (1001) docker     (127)      487 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/controls/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      803 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/controls/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11630 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/controls/_mqtt.py
--rw-r--r--   0 vsts      (1001) docker     (127)      325 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/controls/constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13320 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/controls/controls.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8458 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/controls/mqtt.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/dataset/
--rw-r--r--   0 vsts      (1001) docker     (127)      558 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7724 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/dataset/dataset.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/email/
--rw-r--r--   0 vsts      (1001) docker     (127)      472 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/email/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4935 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/email/email_sender.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/error_handlers/
--rw-r--r--   0 vsts      (1001) docker     (127)     2066 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/error_handlers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15754 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/error_handlers/error_handlers.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/extensions/
--rw-r--r--   0 vsts      (1001) docker     (127)     1038 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/extensions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7519 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/extensions/extensions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1652 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/extensions/field_meta.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2970 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/extensions/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1406 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/extensions/pipeline.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3359 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/initialize.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/integration/
--rw-r--r--   0 vsts      (1001) docker     (127)     1872 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/integration/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12939 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/integration/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36653 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/integration/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (127)   117136 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/integration/integration.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (127)     3359 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    88414 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/pipeline/automation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35931 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/pipeline/definitions.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30536 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/pipeline/pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/platform_insights/
--rw-r--r--   0 vsts      (1001) docker     (127)      542 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/platform_insights/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2214 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/platform_insights/platform_insights.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.923328 switch_api-0.5.6/switch_api.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    38078 2024-05-14 03:33:57.000000 switch_api-0.5.6/switch_api.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1909 2024-05-14 03:33:57.000000 switch_api-0.5.6/switch_api.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-14 03:33:57.000000 switch_api-0.5.6/switch_api.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      148 2024-05-14 03:33:57.000000 switch_api-0.5.6/switch_api.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-14 03:33:57.000000 switch_api-0.5.6/switch_api.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-20 04:20:00.501301 switch_api-0.5.7/
+-rw-r--r--   0 vsts      (1001) docker     (127)      249 2024-05-20 04:19:53.000000 switch_api-0.5.7/AUTHORS.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    36960 2024-05-20 04:19:53.000000 switch_api-0.5.7/HISTORY.md
+-rw-r--r--   0 vsts      (1001) docker     (127)     1093 2024-05-20 04:19:53.000000 switch_api-0.5.7/LICENCE
+-rw-r--r--   0 vsts      (1001) docker     (127)       74 2024-05-20 04:19:53.000000 switch_api-0.5.7/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    38234 2024-05-20 04:20:00.501301 switch_api-0.5.7/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      590 2024-05-20 04:19:53.000000 switch_api-0.5.7/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-05-20 04:19:53.000000 switch_api-0.5.7/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       62 2024-05-20 04:20:00.505301 switch_api-0.5.7/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1448 2024-05-20 04:19:53.000000 switch_api-0.5.7/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-20 04:20:00.497301 switch_api-0.5.7/switch_api/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-20 04:20:00.497301 switch_api-0.5.7/switch_api/_authentication/
+-rw-r--r--   0 vsts      (1001) docker     (127)      391 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/_authentication/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8127 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/_authentication/_authentication.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-20 04:20:00.497301 switch_api-0.5.7/switch_api/_authentication/_credentials_store/
+-rw-r--r--   0 vsts      (1001) docker     (127)      393 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/_authentication/_credentials_store/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5851 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/_authentication/_credentials_store/_credentials_store.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-20 04:20:00.497301 switch_api-0.5.7/switch_api/_authentication/_msal/
+-rw-r--r--   0 vsts      (1001) docker     (127)      361 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/_authentication/_msal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8752 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/_authentication/_msal/_custom_application.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-20 04:20:00.497301 switch_api-0.5.7/switch_api/_guide/
+-rw-r--r--   0 vsts      (1001) docker     (127)      455 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/_guide/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3108 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/_guide/main.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2093 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/_guide/processor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-20 04:20:00.501301 switch_api-0.5.7/switch_api/_utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)      462 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/_utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4205 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/_utils/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5952 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/_utils/_marketplace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14920 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/_utils/_platform.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23502 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/_utils/_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-20 04:20:00.501301 switch_api-0.5.7/switch_api/analytics/
+-rw-r--r--   0 vsts      (1001) docker     (127)      642 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/analytics/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14655 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/analytics/analytics.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-20 04:20:00.501301 switch_api-0.5.7/switch_api/cache/
+-rw-r--r--   0 vsts      (1001) docker     (127)      480 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/cache/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6985 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/cache/cache.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-20 04:20:00.501301 switch_api-0.5.7/switch_api/controls/
+-rw-r--r--   0 vsts      (1001) docker     (127)      487 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/controls/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      803 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/controls/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12443 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/controls/_mqtt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13320 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/controls/controls.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-20 04:20:00.501301 switch_api-0.5.7/switch_api/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (127)      558 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7724 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/dataset/dataset.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-20 04:20:00.501301 switch_api-0.5.7/switch_api/email/
+-rw-r--r--   0 vsts      (1001) docker     (127)      472 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/email/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4935 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/email/email_sender.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-20 04:20:00.501301 switch_api-0.5.7/switch_api/error_handlers/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2066 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/error_handlers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15754 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/error_handlers/error_handlers.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-20 04:20:00.501301 switch_api-0.5.7/switch_api/extensions/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1038 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/extensions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7519 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/extensions/extensions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1652 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/extensions/field_meta.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2970 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/extensions/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1406 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/extensions/pipeline.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3359 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/initialize.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-20 04:20:00.501301 switch_api-0.5.7/switch_api/integration/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1872 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/integration/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12939 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/integration/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36653 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/integration/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   117297 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/integration/integration.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-20 04:20:00.501301 switch_api-0.5.7/switch_api/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3359 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    88430 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/pipeline/automation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35931 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/pipeline/definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30536 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/pipeline/pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-20 04:20:00.501301 switch_api-0.5.7/switch_api/platform_insights/
+-rw-r--r--   0 vsts      (1001) docker     (127)      542 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/platform_insights/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2214 2024-05-20 04:19:53.000000 switch_api-0.5.7/switch_api/platform_insights/platform_insights.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-20 04:20:00.497301 switch_api-0.5.7/switch_api.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    38234 2024-05-20 04:20:00.000000 switch_api-0.5.7/switch_api.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1848 2024-05-20 04:20:00.000000 switch_api-0.5.7/switch_api.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-20 04:20:00.000000 switch_api-0.5.7/switch_api.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      148 2024-05-20 04:20:00.000000 switch_api-0.5.7/switch_api.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-20 04:20:00.000000 switch_api-0.5.7/switch_api.egg-info/top_level.txt
```

### Comparing `switch_api-0.5.6/HISTORY.md` & `switch_api-0.5.7/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # History
 
+## 0.5.7
+### Modified
+In the `controls` module: 
+- Modified `submit_control` method
+  - Returns sensor control values upon control request acknowledgement
+
 ## 0.5.5
 ### Added
 In the `pipeline` module: 
 - Added a new task `IQTask`
   - Additional abstract property `module_type` that accepts strings. This should define the type of IQ module. 
   - Abstract method `process` must be instantiated for the task to be registered.
```

### Comparing `switch_api-0.5.6/LICENCE` & `switch_api-0.5.7/LICENCE`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/PKG-INFO` & `switch_api-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switch_api
-Version: 0.5.6
+Version: 0.5.7
 Summary: A complete package for data ingestion into the Switch Automation Platform.
 Home-page: UNKNOWN
 Author: Switch Automation Pty Ltd.
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -34,14 +34,20 @@
 
 ```bash
 pip install switch_api
 ```
 
 # History
 
+## 0.5.7
+### Modified
+In the `controls` module: 
+- Modified `submit_control` method
+  - Returns sensor control values upon control request acknowledgement
+
 ## 0.5.5
 ### Added
 In the `pipeline` module: 
 - Added a new task `IQTask`
   - Additional abstract property `module_type` that accepts strings. This should define the type of IQ module. 
   - Abstract method `process` must be instantiated for the task to be registered.
```

### Comparing `switch_api-0.5.6/README.md` & `switch_api-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/setup.py` & `switch_api-0.5.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     author="Switch Automation Pty Ltd.",
     description="A complete package for data ingestion into the Switch Automation Platform.",
     long_description=open('README.md', 'r').read() +
     '\n\n' + open('HISTORY.md', 'r').read(),
     long_description_content_type='text/markdown',
     license='MIT License',
     name="switch_api",
-    version="0.5.6",
+    version="0.5.7",
     packages=find_packages(include=["switch_api", "switch_api.*"]),
     install_requires=['pandas', 'requests', 'azure-storage-blob', 'pandera[io]==0.7.1', 'azure-servicebus',
                       'msal>=1.11.0', 'paho-mqtt==1.6.1', 'uvicorn==0.22.0', 'fastapi==0.98.0', 'pyodbc==4.0.39'],
     python_requires=">=3.8.0",
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         "License :: OSI Approved :: MIT License",
```

### Comparing `switch_api-0.5.6/switch_api/__init__.py` & `switch_api-0.5.7/switch_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,8 +35,8 @@
 # _ch.setLevel(logging.INFO)  # sets the handler info
 # _ch.setFormatter(logging.Formatter(INFOFORMATTER))  # sets the handler formatting
 #
 # # adds the handler to the global variable: log
 # log.addHandler(_ch)
 # https://dev.to/joaomcteixeira/setting-up-python-logging-for-a-library-app-6ml
 
-__version__ = "0.5.6"
+__version__ = "0.5.7"
```

### Comparing `switch_api-0.5.6/switch_api/_authentication/_authentication.py` & `switch_api-0.5.7/switch_api/_authentication/_authentication.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/_authentication/_credentials_store/_credentials_store.py` & `switch_api-0.5.7/switch_api/_authentication/_credentials_store/_credentials_store.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/_authentication/_msal/_custom_application.py` & `switch_api-0.5.7/switch_api/_authentication/_msal/_custom_application.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/_guide/main.py` & `switch_api-0.5.7/switch_api/_guide/main.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/_guide/processor.py` & `switch_api-0.5.7/switch_api/_guide/processor.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/_utils/_constants.py` & `switch_api-0.5.7/switch_api/_utils/_constants.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/_utils/_marketplace.py` & `switch_api-0.5.7/switch_api/_utils/_marketplace.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/_utils/_platform.py` & `switch_api-0.5.7/switch_api/_utils/_platform.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/_utils/_utils.py` & `switch_api-0.5.7/switch_api/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/analytics/__init__.py` & `switch_api-0.5.7/switch_api/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/analytics/analytics.py` & `switch_api-0.5.7/switch_api/analytics/analytics.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/cache/cache.py` & `switch_api-0.5.7/switch_api/cache/cache.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/controls/_constants.py` & `switch_api-0.5.7/switch_api/controls/_constants.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/controls/_mqtt.py` & `switch_api-0.5.7/switch_api/controls/_mqtt.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         self.installation_id = installation_id
         self.is_connected = False
         self.is_gateway_connected = False
         self.request_status = 0
         self.connection_timeout = WS_MQTT_CONNECTION_TIMEOUT
 
         self.sensor_count = 0
+        self.sensor_request: list[dict] = []
         self.sensor_results: list[dict] = []
 
         self.mqttc = mqtt.Client(client_id=client_id, transport='websockets')
         self.mqttc.tls_set()
         self.mqttc.username_pw_set(username, password)
         self.mqttc.on_connect = self._on_connect
         self.mqttc.on_message = self._on_message
@@ -94,15 +95,15 @@
         """
         if rc == 0:
             logger.info(
                 f"Connected to MQTT broker: {self.host_address} port:{self.port}")
 
             topics_to_subscribe = [
                 {"topic": self.client_id, "qos": 0},
-                {"topic": f"control-result/pid/{self.project_id}/site/{self.installation_id}", "qos": 1},
+                # {"topic": f"control-result/pid/{self.project_id}/site/{self.installation_id}", "qos": 1},
                 {"topic": f"state/pid/{self.project_id}/site/{self.installation_id}/#", "qos": 1},
             ]
 
             for topic in topics_to_subscribe:
                 url = topic["topic"]
                 qos = topic["qos"]
                 logger.info(f"Subscribing to topic: {url}     qos:{qos}")
@@ -128,16 +129,17 @@
         payload = json.loads(payload_str)
 
         topic = message.topic
         action = payload.get('action')
 
         if topic == self.client_id and action == CONTROL_REQUEST_ACTION_ACK:
             self._process_acknowledgement(payload=payload)
-        elif topic == f'control-result/pid/{self.project_id}/site/{self.installation_id}' and action == CONTROL_REQUEST_ACTION_RESULT:
-            self._process_notification(payload=payload)
+            self._process_write_acknowledgement(payload=payload)
+        # elif topic == f'control-result/pid/{self.project_id}/site/{self.installation_id}' and action == CONTROL_REQUEST_ACTION_RESULT:
+        #     self._process_notification(payload=payload)
         elif topic.startswith('state/pid') and topic.endswith('svc/janus'):
             self._process_gateway_connected(payload=payload)
 
     def connect(self, timeout: int = WS_MQTT_CONNECTION_TIMEOUT) -> bool:
         """Initiate connection to MQTT Broker.
 
         Parameters
@@ -171,14 +173,15 @@
             Message broker topic to pulish message to
         sensors : dict
             Sensors to request control and update value
         """
         logger.info(f'Sending Control Request for {sensors}')
 
         self.sensor_results = []
+        self.sensor_request = sensors
         self.sensor_count = len(sensors)
         topic = f'control/pid/{self.project_id}/site/{self.installation_id}'
 
         payload = self._build_control_request_payload(sensors=sensors)
         payload_json = json.dumps(payload)
 
         logger.info(f'Payload = {payload_json}')
@@ -253,14 +256,35 @@
 
         status = payload.get("status", -1)
         logger.info(
             f'Control Request Acknowledgment. Mac={payload["mac"]} Status={status_messages.get(status, "Unknown status")}')
 
         self.request_status = status
 
+    def _process_write_acknowledgement(self, payload: dict):
+        """Process mqtt message for control result acknowledgement as write command successful
+        and return sensor list request sent as a response.
+
+        Parameters
+        ----------
+        payload : dict
+
+            Message payload
+        """
+
+        for item in self.sensor_request:
+            sensor_control_result = {
+                'sensorId': item["sensorId"],
+                'controlValue': item["controlValue"],
+                'presentValue': item["controlValue"],
+                'status': 1,
+            }
+
+            self.sensor_results.append(sensor_control_result)
+
     def _process_notification(self, payload: dict):
         """Process mqtt message for control result notification
 
         Parameters
         ----------
         payload : dict
             Message payload
```

### Comparing `switch_api-0.5.6/switch_api/controls/controls.py` & `switch_api-0.5.7/switch_api/controls/controls.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/dataset/__init__.py` & `switch_api-0.5.7/switch_api/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/dataset/dataset.py` & `switch_api-0.5.7/switch_api/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/email/email_sender.py` & `switch_api-0.5.7/switch_api/email/email_sender.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/error_handlers/__init__.py` & `switch_api-0.5.7/switch_api/error_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/error_handlers/error_handlers.py` & `switch_api-0.5.7/switch_api/error_handlers/error_handlers.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/extensions/__init__.py` & `switch_api-0.5.7/switch_api/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/extensions/extensions.py` & `switch_api-0.5.7/switch_api/extensions/extensions.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/extensions/field_meta.py` & `switch_api-0.5.7/switch_api/extensions/field_meta.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/extensions/helpers.py` & `switch_api-0.5.7/switch_api/extensions/helpers.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/extensions/pipeline.py` & `switch_api-0.5.7/switch_api/extensions/pipeline.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/initialize.py` & `switch_api-0.5.7/switch_api/initialize.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/integration/__init__.py` & `switch_api-0.5.7/switch_api/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/integration/_utils.py` & `switch_api-0.5.7/switch_api/integration/_utils.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/integration/helpers.py` & `switch_api-0.5.7/switch_api/integration/helpers.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/integration/integration.py` & `switch_api-0.5.7/switch_api/integration/integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,14 +517,15 @@
     elif response.status_code == 200 and len(response.text) > 0:
         response_data_frame = pandas.read_json(response.text)
         logger.info('Dataframe response row count = %s',
                     str(response_data_frame.shape[0]))
 
     return response_data_frame
 
+# TODO confirm FlowExtensionDriver - TaskID = '66c59782-5fbe-40ee-bba0-200e336cc8d6' is not longer in use and if so, remove this method from the python package.
 @_with_func_attrs(df_required_columns=['DriverClassName', 'DriverDeviceType', 'PropertyName', 'DeviceCode', 'DeviceName', 'SensorName', 'SensorTemplate',
                         'SensorUnitOfMeasure', 'EquipmentClass', 'EquipmentLabel'])
 def upsert_device_sensors_ext(df: pandas.DataFrame, api_inputs: ApiInputs, tag_columns: list = None,
                           metadata_columns: list = None, save_additional_columns_as_slices: bool = False):
     """Upsert device(s) and sensor(s)
 
     Required fields are:
```

### Comparing `switch_api-0.5.6/switch_api/pipeline/__init__.py` & `switch_api-0.5.7/switch_api/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/pipeline/automation.py` & `switch_api-0.5.7/switch_api/pipeline/automation.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from azure.servicebus import ServiceBusClient, ServiceBusReceiveMode
 from .._utils._utils import _is_valid_regex, ApiInputs, _column_name_cap, DataFeedFileProcessOutput
 from .._utils._marketplace import add_marketplace_item
 from .._utils._constants import (argus_prefix, EXPECTED_DELIVERY, MAPPING_ENTITIES,
                                  QUEUE_NAME, ERROR_TYPE, SCHEDULE_TIMEZONE, DEPLOY_TYPE, TASK_PRIORITY, TASK_FRAMEWORK, GUIDES_EXTERNAL_TYPES, GUIDES_SCOPE)
 from .._utils._platform import _get_ingestion_service_bus_connection_string, Blob
 from .pipeline import (Task, QueueTask, IntegrationTask, LogicModuleTask, AnalyticsTask, EventWorkOrderTask,
-                       DiscoverableIntegrationTask, BlobTask, Guide)
+                       DiscoverableIntegrationTask, BlobTask, Guide, IQTask)
 from ..extensions import ExtensionTask, replace_extensions_imports, has_extensions_support
 from .definitions import (IntegrationDeviceDefinition, EventWorkOrderFieldDefinition, AnalyticsSettings,
                           IntegrationSettings, IntegrationDeviceConfigPropertyDefinition)
 
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
@@ -1136,15 +1136,15 @@
         df = pandas.read_json(StringIO(response.text), typ='Series').to_frame().T
         df.columns = _column_name_cap(df.columns)
 
         return df
 
     @staticmethod
     def deploy_on_timer(task: Union[Task, IntegrationTask, DiscoverableIntegrationTask, QueueTask,
-                                    AnalyticsTask, LogicModuleTask, EventWorkOrderTask],
+                                    AnalyticsTask, LogicModuleTask, EventWorkOrderTask, IQTask],
                         api_inputs: ApiInputs, data_feed_id: uuid.UUID, expected_delivery: EXPECTED_DELIVERY,
                         cron_schedule: str, queue_name: QUEUE_NAME = "task", settings: dict = None,
                         schedule_timezone: SCHEDULE_TIMEZONE = 'Local', timezone_offset_minutes: int = None,
                         data_feed_name: str = None, task_priority: TASK_PRIORITY = 'default',
                         task_framework: TASK_FRAMEWORK = 'PythonScriptFramework'):
         """Deploy driver to run on timer.
```

### Comparing `switch_api-0.5.6/switch_api/pipeline/definitions.py` & `switch_api-0.5.7/switch_api/pipeline/definitions.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/pipeline/pipeline.py` & `switch_api-0.5.7/switch_api/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/platform_insights/__init__.py` & `switch_api-0.5.7/switch_api/platform_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api/platform_insights/platform_insights.py` & `switch_api-0.5.7/switch_api/platform_insights/platform_insights.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.6/switch_api.egg-info/PKG-INFO` & `switch_api-0.5.7/switch_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switch-api
-Version: 0.5.6
+Version: 0.5.7
 Summary: A complete package for data ingestion into the Switch Automation Platform.
 Home-page: UNKNOWN
 Author: Switch Automation Pty Ltd.
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -34,14 +34,20 @@
 
 ```bash
 pip install switch_api
 ```
 
 # History
 
+## 0.5.7
+### Modified
+In the `controls` module: 
+- Modified `submit_control` method
+  - Returns sensor control values upon control request acknowledgement
+
 ## 0.5.5
 ### Added
 In the `pipeline` module: 
 - Added a new task `IQTask`
   - Additional abstract property `module_type` that accepts strings. This should define the type of IQ module. 
   - Abstract method `process` must be instantiated for the task to be registered.
```

### Comparing `switch_api-0.5.6/switch_api.egg-info/SOURCES.txt` & `switch_api-0.5.7/switch_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,15 @@
 switch_api/analytics/__init__.py
 switch_api/analytics/analytics.py
 switch_api/cache/__init__.py
 switch_api/cache/cache.py
 switch_api/controls/__init__.py
 switch_api/controls/_constants.py
 switch_api/controls/_mqtt.py
-switch_api/controls/constants.py
 switch_api/controls/controls.py
-switch_api/controls/mqtt.py
 switch_api/dataset/__init__.py
 switch_api/dataset/dataset.py
 switch_api/email/__init__.py
 switch_api/email/email_sender.py
 switch_api/error_handlers/__init__.py
 switch_api/error_handlers/error_handlers.py
 switch_api/extensions/__init__.py
```


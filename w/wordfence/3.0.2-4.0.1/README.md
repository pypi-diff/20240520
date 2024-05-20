# Comparing `tmp/wordfence-3.0.2.tar.gz` & `tmp/wordfence-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordfence-3.0.2.tar", last modified: Mon Feb 12 19:07:15 2024, max compression
+gzip compressed data, was "wordfence-4.0.1.tar", last modified: Mon May 20 18:26:29 2024, max compression
```

## Comparing `wordfence-3.0.2.tar` & `wordfence-4.0.1.tar`

### file list

```diff
@@ -1,124 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.618790 wordfence-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-12 19:07:07.000000 wordfence-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44045 2024-02-12 19:07:15.614790 wordfence-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-02-12 19:07:07.000000 wordfence-3.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-02-12 19:07:07.000000 wordfence-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 19:07:15.618790 wordfence-3.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.602790 wordfence-3.0.2/wordfence/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.606790 wordfence-3.0.2/wordfence/api/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/api/intelligence.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/api/licensing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/api/noc1.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/api/noc4.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/api/noc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.606790 wordfence-3.0.2/wordfence/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/auto_complete.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.606790 wordfence-3.0.2/wordfence/cli/banner/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/banner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/banner/banner.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6493 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.606790 wordfence-3.0.2/wordfence/cli/config/
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/config/base_config_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/config/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/config/config_items.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/config/ini_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/config/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.610790 wordfence-3.0.2/wordfence/cli/configure/
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/configure/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/configure/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/configurer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.610790 wordfence-3.0.2/wordfence/cli/countsites/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/countsites/countsites.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/countsites/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/email.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.610790 wordfence-3.0.2/wordfence/cli/help/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/help/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/help/help.py
--rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/licensing.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/mailing_lists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.610790 wordfence-3.0.2/wordfence/cli/malwarescan/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/malwarescan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/malwarescan/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8649 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/malwarescan/malwarescan.py
--rw-r--r--   0 runner    (1001) docker     (127)    20021 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/malwarescan/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     7135 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/malwarescan/reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.610790 wordfence-3.0.2/wordfence/cli/remediate/
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/remediate/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/remediate/remediate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/remediate/reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)    20224 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/subcommands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.610790 wordfence-3.0.2/wordfence/cli/terms/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/terms/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/terms/terms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/terms_management.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.610790 wordfence-3.0.2/wordfence/cli/version/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/version/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/version/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.610790 wordfence-3.0.2/wordfence/cli/vulnscan/
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/vulnscan/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/vulnscan/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9665 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/vulnscan/reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)    12696 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/cli/vulnscan/vulnscan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.610790 wordfence-3.0.2/wordfence/intel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/intel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/intel/signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)    13096 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/intel/vulnerabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.610790 wordfence-3.0.2/wordfence/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/logging/formatting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.610790 wordfence-3.0.2/wordfence/php/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/php/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/php/lexing.py
--rw-r--r--   0 runner    (1001) docker     (127)    50838 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/php/parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.614790 wordfence-3.0.2/wordfence/scanning/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/scanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/scanning/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/scanning/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/scanning/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)    29984 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/scanning/scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.614790 wordfence-3.0.2/wordfence/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/util/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/util/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/util/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/util/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/util/pcre.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/util/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/util/terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/util/test_versioning.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/util/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/util/unicode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/util/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/util/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/util/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/util/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/util/versioning.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.614790 wordfence-3.0.2/wordfence/wordpress/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/wordpress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/wordpress/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/wordpress/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/wordpress/identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/wordpress/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/wordpress/remediator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15346 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/wordpress/site.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-02-12 19:07:07.000000 wordfence-3.0.2/wordfence/wordpress/theme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:07:15.614790 wordfence-3.0.2/wordfence.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44045 2024-02-12 19:07:15.000000 wordfence-3.0.2/wordfence.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-02-12 19:07:15.000000 wordfence-3.0.2/wordfence.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 19:07:15.000000 wordfence-3.0.2/wordfence.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-12 19:07:15.000000 wordfence-3.0.2/wordfence.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-12 19:07:15.000000 wordfence-3.0.2/wordfence.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-12 19:07:15.000000 wordfence-3.0.2/wordfence.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.058680 wordfence-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 18:26:22.000000 wordfence-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44045 2024-05-20 18:26:29.058680 wordfence-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-20 18:26:23.000000 wordfence-4.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-20 18:26:22.000000 wordfence-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 18:26:29.058680 wordfence-4.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.038680 wordfence-4.0.1/wordfence/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.042680 wordfence-4.0.1/wordfence/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/api/intelligence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/api/licensing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/api/noc1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/api/noc4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/api/noc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.042680 wordfence-4.0.1/wordfence/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/auto_complete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.042680 wordfence-4.0.1/wordfence/cli/banner/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/banner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/banner/banner.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6530 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.046680 wordfence-4.0.1/wordfence/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/config/base_config_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/config/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/config/config_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/config/ini_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/config/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.046680 wordfence-4.0.1/wordfence/cli/configure/
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/configure/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/configure/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/configurer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.046680 wordfence-4.0.1/wordfence/cli/countsites/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/countsites/countsites.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/countsites/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.046680 wordfence-4.0.1/wordfence/cli/help/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/help/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/help/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/licensing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/mailing_lists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.046680 wordfence-4.0.1/wordfence/cli/malwarescan/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/malwarescan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/malwarescan/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16197 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/malwarescan/malwarescan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20021 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/malwarescan/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7135 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/malwarescan/reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.046680 wordfence-4.0.1/wordfence/cli/remediate/
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/remediate/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/remediate/remediate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/remediate/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20224 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/subcommands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.046680 wordfence-4.0.1/wordfence/cli/terms/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/terms/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/terms/terms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/terms_management.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.046680 wordfence-4.0.1/wordfence/cli/version/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/version/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/version/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.050680 wordfence-4.0.1/wordfence/cli/vulnscan/
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/vulnscan/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/vulnscan/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9665 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/vulnscan/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12696 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/cli/vulnscan/vulnscan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.050680 wordfence-4.0.1/wordfence/intel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/intel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/intel/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13096 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/intel/vulnerabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.050680 wordfence-4.0.1/wordfence/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/logging/formatting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.050680 wordfence-4.0.1/wordfence/php/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/php/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/php/lexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50838 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/php/parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.050680 wordfence-4.0.1/wordfence/scanning/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/scanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/scanning/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/scanning/filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.050680 wordfence-4.0.1/wordfence/scanning/matching/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/scanning/matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/scanning/matching/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/scanning/matching/pcre.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/scanning/matching/vectorscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36945 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/scanning/scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.054680 wordfence-4.0.1/wordfence/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/direct_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/library.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.054680 wordfence-4.0.1/wordfence/util/pcre/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/pcre/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/pcre/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/pcre/pcre.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/test_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/unicode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.054680 wordfence-4.0.1/wordfence/util/vectorscan/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/vectorscan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13703 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/vectorscan/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/vectorscan/vectorscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/util/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.058680 wordfence-4.0.1/wordfence/wordpress/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/wordpress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/wordpress/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/wordpress/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/wordpress/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/wordpress/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/wordpress/remediator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15346 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/wordpress/site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-20 18:26:22.000000 wordfence-4.0.1/wordfence/wordpress/theme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:26:29.058680 wordfence-4.0.1/wordfence.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44045 2024-05-20 18:26:29.000000 wordfence-4.0.1/wordfence.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-20 18:26:29.000000 wordfence-4.0.1/wordfence.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:26:29.000000 wordfence-4.0.1/wordfence.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 18:26:29.000000 wordfence-4.0.1/wordfence.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 18:26:29.000000 wordfence-4.0.1/wordfence.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 18:26:29.000000 wordfence-4.0.1/wordfence.egg-info/top_level.txt
```

### Comparing `wordfence-3.0.2/LICENSE` & `wordfence-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/PKG-INFO` & `wordfence-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordfence
-Version: 3.0.2
+Version: 4.0.1
 Summary: Command-line malware scanner powered by Wordfence
 Author-email: Wordfence <opensource@wordfence.com>
 Maintainer-email: Wordfence <opensource@wordfence.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -697,15 +697,15 @@
 
 # Wordfence CLI
 
  Wordfence CLI is an open source, high performance, multi-process security scanner, written in Python, that quickly scans network filesystems to detect PHP/other malware and WordPress vulnerabilities. CLI is parallelizable, can be scheduled, can accept input via pipe, and can pipe output to other commands.
 
 ## Installation
 
-We have a number of installation methods to install Wordfence CLI in our [installation documentation](https://github.com/wordfence/wordfence-cli/blob/v3.0.2/docs/Installation.md) which we'd recommend reviewing to get you scanning for malware in as few steps as possible. 
+We have a number of installation methods to install Wordfence CLI in our [installation documentation](https://github.com/wordfence/wordfence-cli/blob/v4.0.1/docs/Installation.md) which we'd recommend reviewing to get you scanning for malware in as few steps as possible. 
 
 We recommend installing using `pip`:
 
 	pip install wordfence
 
 If you'd like to install Wordfence CLI manually or use CLI for development, you can clone the GitHub repo to your local environment:
 
@@ -724,32 +724,32 @@
 
 ### Obtaining a license
 
 Visit [https://www.wordfence.com/products/wordfence-cli/](https://www.wordfence.com/products/wordfence-cli/) to obtain a license to download our signature set.
 
 ## Usage
 
-You can run `wordfence help` for a full list of options that can be passed to Wordfence CLI. Read more about the [configuration options](https://github.com/wordfence/wordfence-cli/blob/v3.0.2/docs/Configuration.md) that can be passed to Wordfence CLI.
+You can run `wordfence help` for a full list of options that can be passed to Wordfence CLI. Read more about the [configuration options](https://github.com/wordfence/wordfence-cli/blob/v4.0.1/docs/Configuration.md) that can be passed to Wordfence CLI.
 
 #### Scanning a directory for malware
 
 Recursively scanning the `/var/www` directory for malware:
 
 	wordfence malware-scan /var/www
 
-A [full list of examples for the malware scan](https://github.com/wordfence/wordfence-cli/blob/v3.0.2/docs/malware-scan/Examples.md) is included in our documentation.
+A [full list of examples for the malware scan](https://github.com/wordfence/wordfence-cli/blob/v4.0.1/docs/malware-scan/Examples.md) is included in our documentation.
 
 #### Scanning a WordPress installation for vulnerabilities
 
 Scanning the `/var/www/wordpress` directory for vulnerabilities. 
 
 	wordfence vuln-scan /var/www/wordpress
 
-A [full list of examples for the vulnerability scan](https://github.com/wordfence/wordfence-cli/blob/v3.0.2/docs/vuln-scan/Examples.md) is included in our documentation.
+A [full list of examples for the vulnerability scan](https://github.com/wordfence/wordfence-cli/blob/v4.0.1/docs/vuln-scan/Examples.md) is included in our documentation.
 
 ## Documentation
 
-The full documentation for Wordfence CLI can be found [here](https://github.com/wordfence/wordfence-cli/blob/v3.0.2/docs/) which includes installation instructions, configuration options, detailed examples, and frequently asked questions.
+The full documentation for Wordfence CLI can be found [here](https://github.com/wordfence/wordfence-cli/blob/v4.0.1/docs/) which includes installation instructions, configuration options, detailed examples, and frequently asked questions.
 
 ## License
 
-Wordfence CLI is open source, licensed under GPLv3. The license can be found [here](https://github.com/wordfence/wordfence-cli/blob/v3.0.2/LICENSE).
+Wordfence CLI is open source, licensed under GPLv3. The license can be found [here](https://github.com/wordfence/wordfence-cli/blob/v4.0.1/LICENSE).
```

### Comparing `wordfence-3.0.2/README.md` & `wordfence-4.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Wordfence CLI
 
  Wordfence CLI is an open source, high performance, multi-process security scanner, written in Python, that quickly scans network filesystems to detect PHP/other malware and WordPress vulnerabilities. CLI is parallelizable, can be scheduled, can accept input via pipe, and can pipe output to other commands.
 
 ## Installation
 
-We have a number of installation methods to install Wordfence CLI in our [installation documentation](https://github.com/wordfence/wordfence-cli/blob/v3.0.2/docs/Installation.md) which we'd recommend reviewing to get you scanning for malware in as few steps as possible. 
+We have a number of installation methods to install Wordfence CLI in our [installation documentation](https://github.com/wordfence/wordfence-cli/blob/v4.0.1/docs/Installation.md) which we'd recommend reviewing to get you scanning for malware in as few steps as possible. 
 
 We recommend installing using `pip`:
 
 	pip install wordfence
 
 If you'd like to install Wordfence CLI manually or use CLI for development, you can clone the GitHub repo to your local environment:
 
@@ -27,32 +27,32 @@
 
 ### Obtaining a license
 
 Visit [https://www.wordfence.com/products/wordfence-cli/](https://www.wordfence.com/products/wordfence-cli/) to obtain a license to download our signature set.
 
 ## Usage
 
-You can run `wordfence help` for a full list of options that can be passed to Wordfence CLI. Read more about the [configuration options](https://github.com/wordfence/wordfence-cli/blob/v3.0.2/docs/Configuration.md) that can be passed to Wordfence CLI.
+You can run `wordfence help` for a full list of options that can be passed to Wordfence CLI. Read more about the [configuration options](https://github.com/wordfence/wordfence-cli/blob/v4.0.1/docs/Configuration.md) that can be passed to Wordfence CLI.
 
 #### Scanning a directory for malware
 
 Recursively scanning the `/var/www` directory for malware:
 
 	wordfence malware-scan /var/www
 
-A [full list of examples for the malware scan](https://github.com/wordfence/wordfence-cli/blob/v3.0.2/docs/malware-scan/Examples.md) is included in our documentation.
+A [full list of examples for the malware scan](https://github.com/wordfence/wordfence-cli/blob/v4.0.1/docs/malware-scan/Examples.md) is included in our documentation.
 
 #### Scanning a WordPress installation for vulnerabilities
 
 Scanning the `/var/www/wordpress` directory for vulnerabilities. 
 
 	wordfence vuln-scan /var/www/wordpress
 
-A [full list of examples for the vulnerability scan](https://github.com/wordfence/wordfence-cli/blob/v3.0.2/docs/vuln-scan/Examples.md) is included in our documentation.
+A [full list of examples for the vulnerability scan](https://github.com/wordfence/wordfence-cli/blob/v4.0.1/docs/vuln-scan/Examples.md) is included in our documentation.
 
 ## Documentation
 
-The full documentation for Wordfence CLI can be found [here](https://github.com/wordfence/wordfence-cli/blob/v3.0.2/docs/) which includes installation instructions, configuration options, detailed examples, and frequently asked questions.
+The full documentation for Wordfence CLI can be found [here](https://github.com/wordfence/wordfence-cli/blob/v4.0.1/docs/) which includes installation instructions, configuration options, detailed examples, and frequently asked questions.
 
 ## License
 
-Wordfence CLI is open source, licensed under GPLv3. The license can be found [here](https://github.com/wordfence/wordfence-cli/blob/v3.0.2/LICENSE).
+Wordfence CLI is open source, licensed under GPLv3. The license can be found [here](https://github.com/wordfence/wordfence-cli/blob/v4.0.1/LICENSE).
```

### Comparing `wordfence-3.0.2/pyproject.toml` & `wordfence-4.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/api/intelligence.py` & `wordfence-4.0.1/wordfence/api/intelligence.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/api/licensing.py` & `wordfence-4.0.1/wordfence/api/licensing.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union
+from typing import Union, Optional
 
 from .exceptions import ApiException
 
 
 LICENSE_URL = 'https://www.wordfence.com/products/wordfence-cli/'
 
 
@@ -32,12 +32,18 @@
                 'License required',
                 'A valid Wordfence CLI license is required'
             )
 
 
 class LicenseSpecific:
 
-    def __init__(self, license: License):
+    def __init__(self, license: Optional[License]):
         self.license = license
 
     def is_compatible_with_license(self, license: License):
-        return self.license == license
+        return self.license is None or self.license == license
+
+    def assign_license(self, license: Optional[License]):
+        self.license = license
+
+    def clear_license(self):
+        self.assign_license(None)
```

### Comparing `wordfence-3.0.2/wordfence/api/noc_client.py` & `wordfence-4.0.1/wordfence/api/noc_client.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/auto_complete.py` & `wordfence-4.0.1/wordfence/cli/auto_complete.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/banner/banner.py` & `wordfence-4.0.1/wordfence/cli/banner/banner.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/cli.py` & `wordfence-4.0.1/wordfence/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,21 +174,25 @@
             subcommand = self.subcommand_definition.initialize_subcommand(
                     context
                 )
             self.exception_handler.subcommand = subcommand
             return subcommand.invoke()
 
 
-def main():
+def invoke_cli():
     exception_handler = ExceptionHandler()
     try:
         cli = WordfenceCli(exception_handler)
         return cli.invoke()
     except BaseException as exception:  # noqa: B036
         return exception_handler.process_exception(exception)
     except KeyboardInterrupt:
         return 130
 
 
-if __name__ == '__main__':
-    exit_code = main()
+def main():
+    exit_code = invoke_cli()
     sys.exit(exit_code)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `wordfence-3.0.2/wordfence/cli/config/__init__.py` & `wordfence-4.0.1/wordfence/cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/config/base_config_definitions.py` & `wordfence-4.0.1/wordfence/cli/config/base_config_definitions.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/config/cli_parser.py` & `wordfence-4.0.1/wordfence/cli/config/cli_parser.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/config/config.py` & `wordfence-4.0.1/wordfence/cli/config/config.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/config/config_items.py` & `wordfence-4.0.1/wordfence/cli/config/config_items.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/config/ini_parser.py` & `wordfence-4.0.1/wordfence/cli/config/ini_parser.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/configure/configure.py` & `wordfence-4.0.1/wordfence/cli/configure/configure.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/configure/definition.py` & `wordfence-4.0.1/wordfence/cli/configure/definition.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/configurer.py` & `wordfence-4.0.1/wordfence/cli/configurer.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/context.py` & `wordfence-4.0.1/wordfence/cli/context.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 from typing import Optional, Any, Callable, Set, Union
 
 from ..version import __version__, __version_name__
-from ..util import pcre
+from ..util import pcre, vectorscan
+from ..util.text import yes_no
 from ..api import noc1, intelligence
 from ..util.caching import Cache, CacheDirectory, RuntimeCache, \
         InvalidCachedValueException, CacheException
 from ..util.input import has_terminal_input, has_terminal_output
 from ..util.io import resolve_path
 from ..api.licensing import License, LicenseRequiredException, \
         LicenseSpecific, to_license
@@ -152,25 +153,43 @@
         return self._wfi_client
 
     def get_mailer(self) -> Mailer:
         if self._mailer is None:
             self._mailer = Mailer(self.config)
         return self._mailer
 
+    def has_pcre(self) -> bool:
+        return pcre.AVAILABLE
+
+    def has_vectorscan(self) -> bool:
+        return vectorscan.AVAILABLE
+
     def display_version(self) -> None:
         if __version_name__ is None:
             name_suffix = ''
         else:
             name_suffix = f' "{__version_name__}"'
         print(f"Wordfence CLI {__version__}{name_suffix}")
-        jit_support_text = 'Yes' if pcre.HAS_JIT_SUPPORT else 'No'
-        print(
-                f"PCRE Version: {pcre.VERSION} - "
-                f"JIT Supported: {jit_support_text}"
-            )
+        has_pcre = self.has_pcre()
+        pcre_support_text = yes_no(has_pcre)
+        if has_pcre:
+            jit_support_text = yes_no(pcre.HAS_JIT_SUPPORT)
+            pcre_support_text += (
+                    f" - PCRE Version: {pcre.VERSION}"
+                    f" (JIT Supported: {jit_support_text})"
+                )
+        print(f'PCRE Supported: {pcre_support_text}')
+        has_vectorscan = self.has_vectorscan()
+        vectorscan_support_text = yes_no(has_vectorscan)
+        if has_vectorscan:
+            vectorscan_support_text += (
+                    f' - Version: {vectorscan.VERSION} (API Version: '
+                    f'{vectorscan.API_VERSION})'
+                )
+        print(f'Vectorscan Supported: {vectorscan_support_text}')
 
     def has_terminal_output(self) -> bool:
         return has_terminal_output()
 
     def has_terminal_input(self) -> bool:
         return has_terminal_input()
```

### Comparing `wordfence-3.0.2/wordfence/cli/countsites/countsites.py` & `wordfence-4.0.1/wordfence/cli/countsites/countsites.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/countsites/definition.py` & `wordfence-4.0.1/wordfence/cli/countsites/definition.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/email.py` & `wordfence-4.0.1/wordfence/cli/email.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/helper.py` & `wordfence-4.0.1/wordfence/cli/helper.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/io.py` & `wordfence-4.0.1/wordfence/cli/io.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/licensing.py` & `wordfence-4.0.1/wordfence/cli/licensing.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/mailing_lists.py` & `wordfence-4.0.1/wordfence/cli/mailing_lists.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/malwarescan/progress.py` & `wordfence-4.0.1/wordfence/cli/malwarescan/progress.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/malwarescan/reporting.py` & `wordfence-4.0.1/wordfence/cli/malwarescan/reporting.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/remediate/definition.py` & `wordfence-4.0.1/wordfence/cli/remediate/definition.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/remediate/remediate.py` & `wordfence-4.0.1/wordfence/cli/remediate/remediate.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/remediate/reporting.py` & `wordfence-4.0.1/wordfence/cli/remediate/reporting.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/reporting.py` & `wordfence-4.0.1/wordfence/cli/reporting.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/subcommands.py` & `wordfence-4.0.1/wordfence/cli/subcommands.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/terms/terms.py` & `wordfence-4.0.1/wordfence/cli/terms/terms.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/terms_management.py` & `wordfence-4.0.1/wordfence/cli/terms_management.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/vulnscan/definition.py` & `wordfence-4.0.1/wordfence/cli/vulnscan/definition.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/vulnscan/reporting.py` & `wordfence-4.0.1/wordfence/cli/vulnscan/reporting.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/cli/vulnscan/vulnscan.py` & `wordfence-4.0.1/wordfence/cli/vulnscan/vulnscan.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/intel/vulnerabilities.py` & `wordfence-4.0.1/wordfence/intel/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/logging/__init__.py` & `wordfence-4.0.1/wordfence/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/logging/formatting.py` & `wordfence-4.0.1/wordfence/logging/formatting.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/php/lexing.py` & `wordfence-4.0.1/wordfence/php/lexing.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/php/parsing.py` & `wordfence-4.0.1/wordfence/php/parsing.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/scanning/filtering.py` & `wordfence-4.0.1/wordfence/scanning/filtering.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/scanning/matching.py` & `wordfence-4.0.1/wordfence/scanning/matching/pcre.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,92 @@
 import signal
+from typing import Optional
 
-from ..intel.signatures import CommonString, Signature, SignatureSet
-from ..logging import log
-from ..util.pcre import PcrePattern, PcreException, PcreJitStack, \
+from ...intel.signatures import CommonString, Signature, SignatureSet
+from ...logging import log
+from ...util import pcre
+from ...util.pcre import PcrePattern, PcreException, PcreJitStack, \
         PcreOptions, PCRE_DEFAULT_OPTIONS
 
+from .matching import Matcher, BaseMatcherContext, TimeoutException, \
+        MatchWorkspace, MatchEngineCompilerOptions, MatchEngineOptions, \
+        DEFAULT_TIMEOUT
 
-DEFAULT_TIMEOUT = 1  # Seconds
 
+if not pcre.AVAILABLE:
+    raise RuntimeError('PCRE is not available')
 
-class TimeoutException(Exception):
-    pass
 
+class PcreCommonString:
 
-class MatchResult:
+    def __init__(self, common_string: CommonString, pcre_options: PcreOptions):
+        self.common_string = common_string
+        self.pattern = PcrePattern(common_string.string, pcre_options)
 
-    def __init__(self, matches: list):
-        self.matches = matches
 
-    def matches(self) -> bool:
-        return len(self.matches) > 0
+class PcreSignature:
 
+    def __init__(self, signature: Signature, pcre_options: PcreOptions):
+        self.signature = signature
+        self.anchored_to_start = self._is_anchored_to_start()
+        self.pcre_options = pcre_options
+        if not signature.has_common_strings():
+            self.compile()
 
-class Matcher:
+    def _is_anchored_to_start(self) -> bool:
+        try:
+            first_character = self.signature.rule[0]
+            return first_character == '^'
+        except IndexError:
+            # Patterns shouldn't be empty, but if they are, they're not
+            # anchored
+            return False
 
-    def __init__(
-                self,
-                signature_set: SignatureSet,
-                timeout: int = DEFAULT_TIMEOUT,
-                match_all: bool = False
-            ):
-        self.signature_set = signature_set
-        self.timeout = timeout
-        self.match_all = match_all
+    def is_valid(self) -> bool:
+        return self.get_pattern() is not None
 
-    def prepare():
-        pass
+    def compile(self) -> None:
+        try:
+            rule = self.signature.rule
+            self.pattern = PcrePattern(rule, self.pcre_options)
+        except BaseException as error:  # noqa: B036
+            log.error('Regex compilation for signature ' +
+                      str(self.signature.identifier) +
+                      ' failed: ' +
+                      str(error) +
+                      ', pattern: ' +
+                      repr(rule))
+            self.pattern = None
+
+    def get_pattern(self) -> PcrePattern:
+        # Signature patterns are compiled lazily as they are only needed if
+        # common strings are matched and compiling all takes several seconds
+        if not hasattr(self, 'pattern'):
+            self.compile()
+        return self.pattern
 
 
-class MatcherContext:
-    pass
+class PcreMatchWorkspace(MatchWorkspace):
 
+    def __init__(self):
+        self.jit_stack = None
 
-class RegexMatcherContext(MatcherContext):
+    def __enter__(self):
+        self.jit_stack = PcreJitStack()
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback) -> None:
+        self.jit_stack.__exit__(exc_type, exc_value, traceback)
 
-    def __init__(self, matcher):
-        self.matcher = matcher
+
+class PcreMatcherContext(BaseMatcherContext):
+
+    def __init__(self, matcher: Matcher):
+        super().__init__(matcher)
         self.common_string_states = self._initialize_common_string_states()
-        self.matches = {}
-        self.timeouts = set()
 
     def _initialize_common_string_states(self) -> list:
         states = []
         for _common_string in self.matcher.common_strings:
             states.append(False)
         return states
 
@@ -85,160 +119,134 @@
                 possible_signatures.append(signature)
         return possible_signatures
 
     def _match_signature(
                 self,
                 signature: Signature,
                 chunk: bytes,
-                start: bool = False
+                start: bool = False,
+                jit_stack: Optional[PcreJitStack] = None
             ) -> bool:
         if not signature.is_valid():
             print('Signature is not valid')
             return False
         if signature.anchored_to_start and not start:
             return False
         try:
             signal.setitimer(signal.ITIMER_VIRTUAL, self.matcher.timeout)
-            match = signature.get_pattern().match(chunk)
+            match = signature.get_pattern().match(chunk, jit_stack)
             signal.setitimer(signal.ITIMER_VIRTUAL, 0)  # Clear timeout
             if match is not None:
-                self.matches[signature.signature.identifier] = \
-                        match.matched_string
+                self._record_match(
+                        identifier=signature.signature.identifier,
+                        matched=match.matched_string
+                    )
                 return True
         except PcreException as e:
             log.debug(
                     'Signature matching failed for '
                     f'{signature.signature.identifier}, {e}'
                 )
         except TimeoutException:
             self.timeouts.add(signature.signature.identifier)
         return False
 
     def process_chunk(
                 self,
                 chunk: bytes,
-                jit_stack: PcreJitStack,
                 start: bool = False,
+                workspace: Optional[MatchWorkspace] = None
             ) -> bool:
         possible_signatures = self._check_common_strings(chunk)
         for signature in self.matcher.signatures_without_common_strings:
-            if self._match_signature(signature, chunk, start) and \
-                    not self.matcher.match_all:
+            if self._match_signature(
+                        signature, chunk, start, workspace.jit_stack
+                    ) and not self.matcher.match_all:
                 return True
         for signature in possible_signatures:
-            if self._match_signature(signature, chunk, start) and \
-                    not self.matcher.match_all:
+            if self._match_signature(
+                        signature, chunk, start, workspace.jit_stack
+                    ) and not self.matcher.match_all:
                 return True
         return False
 
     def __enter__(self):
         def handle_timeout(signum, frame):
             raise TimeoutException()
 
         self._previous_alarm_handler = signal.signal(
                 signal.SIGVTALRM,
                 handle_timeout
             )
         if self._previous_alarm_handler is None:
             self._previous_alarm_handler = signal.SIG_DFL
-        return self
+        return super().__enter__()
 
     def __exit__(self, exc_type, exc_value, traceback) -> None:
         signal.signal(signal.SIGVTALRM, self._previous_alarm_handler)
 
 
-class RegexCommonString:
-
-    def __init__(self, common_string: CommonString, pcre_options: PcreOptions):
-        self.common_string = common_string
-        self.pattern = PcrePattern(common_string.string, pcre_options)
-
-
-class RegexSignature:
-
-    def __init__(self, signature: Signature, pcre_options: PcreOptions):
-        self.signature = signature
-        self.anchored_to_start = self._is_anchored_to_start()
-        self.pcre_options = pcre_options
-        if not signature.has_common_strings():
-            self.compile()
-
-    def _is_anchored_to_start(self) -> bool:
-        try:
-            first_character = self.signature.rule[0]
-            return first_character == '^'
-        except IndexError:
-            # Patterns shouldn't be empty, but if they are, they're not
-            # anchored
-            return False
-
-    def is_valid(self) -> bool:
-        return self.get_pattern() is not None
-
-    def compile(self) -> None:
-        try:
-            rule = self.signature.rule
-            self.pattern = PcrePattern(rule, self.pcre_options)
-        except BaseException as error:  # noqa: B036
-            log.error('Regex compilation for signature ' +
-                      str(self.signature.identifier) +
-                      ' failed: ' +
-                      str(error) +
-                      ', pattern: ' +
-                      repr(rule))
-            self.pattern = None
-
-    def get_pattern(self) -> PcrePattern:
-        # Signature patterns are compiled lazily as they are only needed if
-        # common strings are matched and compiling all takes several seconds
-        if not hasattr(self, 'pattern'):
-            self.compile()
-        return self.pattern
-
-
-class RegexMatcher(Matcher):
+class PcreMatcher(Matcher):
 
     def __init__(
                 self,
                 signature_set: SignatureSet,
                 timeout: int = DEFAULT_TIMEOUT,
                 match_all: bool = False,
                 pcre_options: PcreOptions = PCRE_DEFAULT_OPTIONS,
                 lazy: bool = False
             ):
-        super().__init__(signature_set, timeout, match_all)
         self.pcre_options = pcre_options
-        if not lazy:
-            self.prepare()
+        super().__init__(signature_set, timeout, match_all, lazy)
 
     def _extract_signatures_without_common_strings(self) -> list:
         signatures = []
         for signature in self.signatures.values():
             if not signature.signature.has_common_strings():
                 signatures.append(signature)
         return signatures
 
     def _compile_common_strings(self) -> None:
         self.common_strings = [
-                RegexCommonString(common_string, self.pcre_options)
+                PcreCommonString(common_string, self.pcre_options)
                 for common_string in self.signature_set.common_strings
             ]
 
     def _compile_signatures(self) -> None:
         self.signatures = {}
         for identifier, signature in self.signature_set.signatures.items():
-            self.signatures[identifier] = RegexSignature(
+            self.signatures[identifier] = PcreSignature(
                     signature,
                     self.pcre_options
                 )
 
     def _compile_regexes(self) -> None:
         self._compile_common_strings()
         self._compile_signatures()
         self.signatures_without_common_strings = \
             self._extract_signatures_without_common_strings()
 
-    def prepare(self) -> None:
+    def _prepare(self) -> None:
         self._compile_regexes()
 
-    def create_context(self) -> RegexMatcherContext:
-        return RegexMatcherContext(self)
+    def create_context(self) -> PcreMatcherContext:
+        return PcreMatcherContext(self)
+
+    def create_workspace(self) -> PcreMatchWorkspace:
+        return PcreMatchWorkspace()
+
+
+def create_compiler(options: MatchEngineCompilerOptions) -> None:
+    return None
+
+
+def validate_pre_compiled_data(source: bytes) -> bool:
+    return False  # Pre-compilation is not supported
+
+
+def create_matcher(options: MatchEngineOptions) -> PcreMatcher:
+    return PcreMatcher(
+            options.signature_set,
+            match_all=options.match_all,
+            pcre_options=options.pcre_options,
+            lazy=options.lazy
+        )
```

### Comparing `wordfence-3.0.2/wordfence/scanning/scanner.py` & `wordfence-4.0.1/wordfence/scanning/scanner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 import os
 import queue
 import time
 import traceback
-from ctypes import c_bool, c_uint
+import dataclasses
+from ctypes import c_bool, c_uint, c_char
 from enum import IntEnum
-from multiprocessing import Queue, Process, Value, get_start_method
+from multiprocessing import Queue, Process, Value, Array, get_start_method
 from dataclasses import dataclass
-from typing import Set, Optional, Callable, Dict, NamedTuple, Tuple, List
+from typing import Set, Optional, Callable, Dict, NamedTuple, Tuple, List, \
+    Union, BinaryIO
 from logging import Handler
 
 from .exceptions import ScanningException, ScanningIoException
-from .matching import Matcher, RegexMatcher
+from .matching import MatchEngine, MatchEngineOptions, Matcher, MatchWorkspace
 from .filtering import FileFilter, filter_any
 from ..util import timing
 from ..util.io import StreamReader, is_symlink_loop, is_symlink_and_loop, \
     get_all_parents, PathSet
-from ..util.pcre import PcreOptions, PCRE_DEFAULT_OPTIONS, PcreJitStack
+from ..util.direct_io import DirectIoBuffer, DirectIoReader
 from ..util.units import scale_byte_unit
-from ..intel.signatures import SignatureSet
 from ..logging import log, remove_initial_handler, VERBOSE
+from ..util.profiling import Profiler, ProfileEvent, EventTimer, \
+    LogProfileWriterFactory, FileProfileWriterFactory
 
 MAX_PENDING_FILES = 1000  # Arbitrary limit
 MAX_PENDING_RESULTS = 100
 QUEUE_READ_TIMEOUT = 0
+RESULT_QUEUE_READ_TIMEOUT = 1
 PROGRESS_UPDATE_INTERVAL = 100
 DEFAULT_CHUNK_SIZE = 1024 * 1024
+PATH_NAME_LIMIT = 4096
 FILE_LOCATOR_WORKER_INDEX = 0
 """Used by the file locator process when sending events"""
 
 
 USES_FORK = get_start_method() == 'fork'
 
 
@@ -63,14 +68,62 @@
     COMPLETED = 0
     FILE_QUEUE_EMPTIED = 1
     FILE_PROCESSED = 2
     EXCEPTION = 3
     FATAL_EXCEPTION = 4
     PROGRESS_UPDATE = 5
     LOG_MESSAGE = 6
+    PROFILE_EVENT = 7
+
+
+class ScanEvent:
+
+    # TODO: Define custom (more compact) pickle serialization format for this
+    # class as a potential performance improvement
+
+    def __init__(
+                self,
+                type: int,
+                data=None,
+                worker_index: Optional[int] = None
+            ):
+        self.type = type
+        self.data = data
+        self.worker_index = worker_index
+
+
+class ScanProfileEvent(ScanEvent):
+
+    def __init__(
+                self,
+                event: ProfileEvent,
+                worker_index: Optional[int] = None
+            ):
+        super().__init__(ScanEventType.PROFILE_EVENT, event, worker_index)
+
+
+def _put_profile_event(
+            queue: Queue,
+            event: Optional[Union[ProfileEvent, EventTimer]]
+        ) -> None:
+    if event is None:
+        return
+    if isinstance(event, EventTimer):
+        event = event.stop()
+    queue.put(ScanProfileEvent(event))
+
+
+def _event_timer(
+            condition: bool,
+            name: str,
+            is_global: bool = False
+        ) -> Optional[EventTimer]:
+    if not condition:
+        return None
+    return EventTimer(name, is_global=is_global)
 
 
 class EventQueueLogHandler(Handler):
 
     def __init__(self, event_queue: Queue, worker_index: int):
         self._event_queue = event_queue
         self._worker_index = worker_index
@@ -98,25 +151,27 @@
     remove_initial_handler()
     log.addHandler(handler)
 
 
 @dataclass
 class Options:
     paths: Set[str]
-    signatures: SignatureSet
+    match_engine_options: MatchEngineOptions
     workers: int = 1
     chunk_size: int = DEFAULT_CHUNK_SIZE
     path_source: Optional[StreamReader] = None
     scanned_content_limit: Optional[int] = None
     file_filter: Optional[FileFilter] = None
-    match_all: bool = False
-    pcre_options: PcreOptions = PCRE_DEFAULT_OPTIONS
-    allow_io_errors: bool = False,
-    debug: bool = False,
+    allow_io_errors: bool = False
+    debug: bool = False
     logging_initializer: Callable[[], None] = None
+    match_engine: MatchEngine = MatchEngine.get_default()
+    profile: bool = False,
+    profile_path: Optional[str] = None,
+    direct_io: bool = False
 
 
 class Status(IntEnum):
     LOCATING_FILES = 0
     PROCESSING_FILES = 1
     COMPLETE = 2
     FAILED = 3
@@ -219,96 +274,98 @@
                 self,
                 input_queue_size: int = 10,
                 output_queue_size: int = MAX_PENDING_FILES,
                 file_filter: FileFilter = None,
                 use_log_events: bool = False,
                 event_queue: Optional[Queue] = None,
                 allow_io_errors: bool = False,
-                logging_initializer: Callable[[], None] = None
+                logging_initializer: Callable[[], None] = None,
+                profile: bool = False
             ):
         self._input_queue = Queue(input_queue_size)
         self.output_queue = Queue(output_queue_size)
         self.file_filter = file_filter \
             if file_filter is not None \
             else FileFilter([filter_any])
         if use_log_events and not event_queue:
             raise ValueError('Using log events requires an event queue')
         self._use_log_events = use_log_events
         self._event_queue = event_queue
         self.allow_io_errors = allow_io_errors
         self._logging_initializer = logging_initializer
+        self.profile = profile
         self._path_count = 0
         self._skipped_count = Value('i', 0)
         super().__init__(name='file-locator')
 
     def add_path(self, path: str) -> bool:
         try:
             self._input_queue.put(path, block=False)
             self._path_count += 1
             log.info(f'Scanning path: {path}')
             return True
         except queue.Full:
             return False
 
-    def finalize_paths(self):
-        self._input_queue.put(None)
+    def finalize_paths(self) -> bool:
+        try:
+            self._input_queue.put(None, block=False)
+        except queue.Full:
+            return False
         if self._path_count < 1:
             raise ScanConfigurationException(
                     'At least one scan path must be specified'
                 )
+        return True
 
     def get_next_file(self):
         return self.output_queue.get()
 
+    def _put_profile_event(
+                self,
+                event: Optional[Union[ProfileEvent, EventTimer]]
+            ) -> None:
+        if not self.profile:
+            return
+        _put_profile_event(self._event_queue, event)
+
     def run(self):
+        timer = _event_timer(self.profile, 'file_locator_all', is_global=True)
         if self._logging_initializer is not None:
             self._logging_initializer()
         if self._use_log_events:
             use_event_queue_log_handler(
                     self._event_queue,
                     FILE_LOCATOR_WORKER_INDEX
                 )
         try:
             skipped_count = 0
             scanned_paths = PathSet()
             while (path := self._input_queue.get()) is not None:
+                path_timer = _event_timer(self.profile, 'file_locator_path')
                 locator = FileLocator(
                         path=path,
                         file_filter=self.file_filter,
                         queue=self.output_queue,
                         allow_io_errors=self.allow_io_errors,
                         scanned_paths=scanned_paths
                     )
                 locator.locate()
                 skipped_count += locator.skipped_count
+                self._put_profile_event(path_timer)
         except ScanningException as exception:
             self.output_queue.put(ExceptionContainer(exception))
         self._skipped_count.value = skipped_count
         self.output_queue.put(None)
+        self._put_profile_event(timer)
 
     def get_skipped_count(self) -> int:
         return self._skipped_count.value
 
 
-class ScanEvent:
-
-    # TODO: Define custom (more compact) pickle serialization format for this
-    # class as a potential performance improvement
-
-    def __init__(
-                self,
-                type: int,
-                data=None,
-                worker_index: Optional[int] = None
-            ):
-        self.type = type
-        self.data = data
-        self.worker_index = worker_index
-
-
 class ScanProgressMonitor(Process):
 
     def __init__(self, status: Value, event_queue: Queue):
         super().__init__(name='progress-monitor')
         self._event_queue = event_queue
         self._status = status
 
@@ -332,105 +389,160 @@
                 work_queue: Queue,
                 event_queue: Queue,
                 matcher: Matcher,
                 chunk_size: int = DEFAULT_CHUNK_SIZE,
                 scanned_content_limit: Optional[int] = None,
                 use_log_events: bool = False,
                 allow_io_errors: bool = False,
-                logging_initializer: Callable[[], None] = None
+                logging_initializer: Callable[[], None] = None,
+                profile: bool = False,
+                direct_io: bool = False
             ):
         self.index = index
         self._status = status
         self._work_queue = work_queue
         self._event_queue = event_queue
         self._matcher = matcher
         self._chunk_size = chunk_size
         self._working = True
         self._scanned_content_limit = scanned_content_limit
         self._use_log_events = use_log_events
         self._allow_io_errors = allow_io_errors
         self._logging_initializer = logging_initializer
-        self.complete = Value(c_bool, False)
+        self._profile = profile
+        self._opener = self._open_direct if direct_io else self._open
+        self._direct_io = direct_io
+        self.complete = Value(c_bool, lock=False)
+        self.last_file = Array(c_char, PATH_NAME_LIMIT + 1, lock=False)
+        self._timer = None
         super().__init__(name=self._generate_name())
 
     def _generate_name(self) -> str:
         return 'worker-' + str(self.index)
 
+    def _open(self, path: str) -> BinaryIO:
+        return open(path, 'rb')
+
+    def _open_direct(self, path: str) -> DirectIoReader:
+        return DirectIoReader(path, self._direct_io_buffer)
+
     def work(self):
-        self._working = True
-        self._matcher.prepare()
-        log.debug(f'Worker {self.index} started, PID:' + str(os.getpid()))
-        with PcreJitStack() as jit_stack:
-            while self._working:
-                try:
-                    item = self._work_queue.get(timeout=QUEUE_READ_TIMEOUT)
-                    if item is None:
-                        self._put_event(ScanEventType.FILE_QUEUE_EMPTIED)
-                        self._complete()
-                    elif isinstance(item, ExceptionContainer):
-                        if isinstance(item.exception, ScanningIoException):
-                            self._put_io_error(item)
+        self._timer = _event_timer(
+                self._profile,
+                'scan_worker',
+                is_global=True
+            )
+        if self._direct_io:
+            self._direct_io_buffer = DirectIoBuffer(self._chunk_size)
+        try:
+            self._working = True
+            self._matcher.prepare(thread=True)
+            log.debug(f'Worker {self.index} started, PID:' + str(os.getpid()))
+            with self._matcher.create_workspace() as workspace:
+                while self._working:
+                    try:
+                        item = self._work_queue.get(timeout=QUEUE_READ_TIMEOUT)
+                        if item is None:
+                            self._put_event(ScanEventType.FILE_QUEUE_EMPTIED)
+                            self._complete()
+                        elif isinstance(item, ExceptionContainer):
+                            if isinstance(item.exception, ScanningIoException):
+                                self._put_io_error(item)
+                            else:
+                                self._put_event(
+                                        ScanEventType.FATAL_EXCEPTION,
+                                        {'exception': item}
+                                    )
                         else:
-                            self._put_event(
-                                    ScanEventType.FATAL_EXCEPTION,
-                                    {'exception': item}
-                                )
-                    else:
-                        try:
-                            self._process_file(item, jit_stack)
-                        except OSError as error:
-                            self._put_io_error(ExceptionContainer(error))
-                except queue.Empty:
-                    if self._status.value == Status.PROCESSING_FILES:
-                        self._complete()
+                            timer = _event_timer(self._profile, 'process_file')
+                            try:
+                                self._process_file(item, workspace)
+                            except OSError as error:
+                                self._put_io_error(ExceptionContainer(error))
+                            except Exception as error:
+                                self._put_error(ExceptionContainer(error))
+                            self._put_profile_event(timer)
+                    except queue.Empty:
+                        if self._status.value == Status.PROCESSING_FILES:
+                            self._complete()
+        except Exception as error:
+            self._put_error(ExceptionContainer(error))
 
     def _put_event(self, event_type: ScanEventType, data: dict = None) -> None:
         if data is None:
             data = {}
         self._event_queue.put(
                 ScanEvent(event_type, data, worker_index=self.index),
             )
 
-    def _put_io_error(self, error) -> None:
-        event_type = ScanEventType.EXCEPTION if self._allow_io_errors \
-                else ScanEventType.FATAL_EXCEPTION
+    def _put_error(self, error, fatal: bool = True) -> None:
+        event_type = ScanEventType.FATAL_EXCEPTION if fatal \
+                else ScanEventType.EXCEPTION
         self._put_event(
                 event_type,
                 {'exception': error}
             )
 
+    def _put_io_error(self, error) -> None:
+        self._put_error(error, not self._allow_io_errors)
+
+    def _put_profile_event(
+                self,
+                event: Optional[Union[ProfileEvent, EventTimer]]
+            ) -> None:
+        _put_profile_event(self._event_queue, event)
+
     def _complete(self):
         self._working = False
         self.complete.value = True
+        if self._timer is not None:
+            self._put_profile_event(self._timer.stop())
         self._put_event(ScanEventType.COMPLETED)
 
     def is_complete(self) -> bool:
         return self.complete.value
 
     def _get_next_chunk_size(self, length: int) -> int:
         if self._scanned_content_limit is None:
             return self._chunk_size
         elif length >= self._scanned_content_limit:
             return 0
         else:
             return min(self._scanned_content_limit - length, self._chunk_size)
 
-    def _process_file(self, path: str, jit_stack: PcreJitStack):
+    def _process_file(self, path: str, workspace: Optional[MatchWorkspace]):
+        self.last_file.value = path.encode('ascii')[:PATH_NAME_LIMIT] + b'\0'
         log.log(VERBOSE, f'Processing file: {path}')
-        with open(path, mode='rb') as file, \
+        if 'malware-demo' in path:
+            import sys
+            sys.exit(1)
+        open_timer = _event_timer(self._profile, 'open_file')
+        with self._opener(path) as file, \
                 self._matcher.create_context() as context:
+            self._put_profile_event(open_timer)
             length = 0
             while (chunk_size := self._get_next_chunk_size(length)):
+                chunk_timer = _event_timer(self._profile, 'read_chunk')
                 chunk = file.read(chunk_size)
+                self._put_profile_event(chunk_timer)
                 if not chunk:
                     break
                 first = length == 0
                 length += len(chunk)
-                if context.process_chunk(chunk, first, jit_stack):
-                    break
+                match_timer = _event_timer(self._profile, 'match_chunk')
+                try:
+                    if context.process_chunk(
+                                chunk,
+                                start=first,
+                                workspace=workspace
+                            ):
+                        break
+                finally:
+                    self._put_profile_event(match_timer)
+            context.finalize_content()
             self._put_event(
                     ScanEventType.FILE_PROCESSED,
                     {
                         'path': path,
                         'length': length,
                         'matches': context.matches,
                         'timeouts': context.timeouts
@@ -472,14 +584,15 @@
 
     def __init__(self, worker_count: int):
         self.counts = self._initialize_int_metric(worker_count)
         self.bytes = self._initialize_int_metric(worker_count)
         self.matches = self._initialize_int_metric(worker_count)
         self.timeouts = self._initialize_int_metric(worker_count)
         self.skipped_files = 0
+        self.failed_files = 0
 
     def _initialize_int_metric(self, worker_count: int):
         return [0] * worker_count
 
     def record_result(self, worker_index: int, result: ScanResult):
         self.counts[worker_index] += 1
         self.bytes[worker_index] += result.read_length
@@ -518,21 +631,24 @@
     def __init__(self, elapsed_time: int, metrics: ScanMetrics):
         self.elapsed_time = elapsed_time
         self.metrics = metrics
 
 
 ScanResultCallback = Callable[[ScanResult], None]
 ProgressReceiverCallback = Callable[[ScanProgressUpdate], None]
-ScanFinishedCallback = Callable[[ScanMetrics, timing.Timer], None]
+ScanFinishedCallback = Callable[
+        [ScanMetrics, timing.Timer, Optional[Profiler]], None
+    ]
 
 
 class ScanFinishedMessages(NamedTuple):
     results: str
     timeouts: Optional[str]
     skipped: Optional[str]
+    failed: Optional[str]
 
 
 def get_scan_finished_messages(
             metrics: ScanMetrics,
             timer: timing.Timer
         ) -> ScanFinishedMessages:
     match_count = metrics.get_total_matches()
@@ -552,31 +668,41 @@
                 f'{metrics.skipped_files} file(s) were skipped as they did '
                 'not match the configured include patterns. Use '
                 '--include-all-files (or -a) to include all files in the scan.'
             )
     else:
         skipped_message = None
 
+    if metrics.failed_files > 0:
+        failed_message = (
+                f'Processing of {metrics.failed_files} file(s) failed'
+            )
+    else:
+        failed_message = None
+
     return ScanFinishedMessages(
             results_message,
             timeouts_message,
-            skipped_message
+            skipped_message,
+            failed_message
         )
 
 
 def default_scan_finished_handler(
             metrics: ScanMetrics,
-            timer: timing.Timer
+            timer: timing.Timer,
         ) -> None:
     """Used as the default ScanFinishedCallback"""
     messages = get_scan_finished_messages(metrics, timer)
     if messages.timeouts:
         log.warning(messages.timeouts)
     if messages.skipped:
         log.warning(messages.skipped)
+    if messages.failed:
+        log.error(messages.failed)
     log.info(messages.results)
     return messages
 
 
 class ScanWorkerPool:
 
     def __init__(
@@ -589,15 +715,17 @@
                 timer: timing.Timer,
                 progress_receiver: Optional[ProgressReceiverCallback] = None,
                 chunk_size: int = DEFAULT_CHUNK_SIZE,
                 scanned_content_limit: Optional[int] = None,
                 use_log_events: bool = False,
                 allow_io_errors: bool = False,
                 debug: bool = False,
-                logging_initializer: Callable[[], None] = False
+                logging_initializer: Callable[[], None] = False,
+                profiler: Optional[Profiler] = None,
+                direct_io: bool = False
             ):
         self.size = size
         self._matcher = matcher
         self._work_queue = work_queue
         self._event_queue = event_queue
         self.metrics = metrics
         self._timer = timer
@@ -605,14 +733,16 @@
         self._chunk_size = chunk_size
         self._scanned_content_limit = scanned_content_limit
         self._started = False
         self._use_log_events = use_log_events
         self._allow_io_errors = allow_io_errors
         self._debug = debug
         self._logging_initializer = logging_initializer
+        self._profiler = profiler
+        self._direct_io = direct_io
         self._completed = False
 
     def __enter__(self):
         self.start()
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
@@ -637,14 +767,32 @@
         if self._progress_timer is None:
             return False
         elapsed = self._progress_timer.get_elapsed(
                 timing.unit_milliseconds
             )
         return elapsed >= PROGRESS_UPDATE_INTERVAL
 
+    def _initialize_worker(self, index: int) -> ScanWorker:
+        worker = ScanWorker(
+                index,
+                self._status,
+                self._work_queue,
+                self._event_queue,
+                self._matcher,
+                self._chunk_size,
+                self._scanned_content_limit,
+                self._use_log_events,
+                self._allow_io_errors,
+                self._logging_initializer,
+                self._profiler is not None,
+                self._direct_io
+            )
+        worker.start()
+        return worker
+
     def start(self):
         if self._started:
             raise ScanningException('Worker pool has already been started')
         self._status = Value(c_uint, Status.LOCATING_FILES)
         self._workers = []
         if self.has_progress_receiver():
             self._progress_timer = timing.Timer()
@@ -654,27 +802,15 @@
                 )
             self._monitor.start()
             self._send_progress_update()
         else:
             self._progress_timer = None
             self._monitor = None
         for i in range(self.size):
-            worker = ScanWorker(
-                    i,
-                    self._status,
-                    self._work_queue,
-                    self._event_queue,
-                    self._matcher,
-                    self._chunk_size,
-                    self._scanned_content_limit,
-                    self._use_log_events,
-                    self._allow_io_errors,
-                    self._logging_initializer
-                )
-            worker.start()
+            worker = self._initialize_worker(i)
             self._workers.append(worker)
         self._started = True
 
     def _assert_started(self):
         if not self._started:
             raise ScanningException('Worker pool has not been started')
 
@@ -695,26 +831,51 @@
     def is_complete(self) -> bool:
         self._assert_started()
         for worker in self._workers:
             if not worker.is_complete():
                 return False
         return True
 
+    def check_workers(self) -> None:
+        for worker in self._workers:
+            if worker.exitcode is not None and worker.exitcode != 0:
+                last_file = worker.last_file.value.decode('ascii')
+                if len(worker.last_file.value) == 0:
+                    raise Exception(
+                            'Worker exited abnormally (code: '
+                            f'{worker.exitcode}) before processing any file'
+                        )
+                else:
+                    log.warning(
+                            f'Worker exited abnormally (code: '
+                            f'{worker.exitcode})  while processing {last_file}'
+                        )
+                    log.info(f'Restarting worker {worker.index}...')
+                    self._workers[worker.index] = \
+                        self._initialize_worker(worker.index)
+                    self.metrics.failed_files += 1
+
     def await_results(
                 self,
                 result_processor: ScanResultCallback,
                 final: bool = True
             ):
         if self._completed:
             return True
         self._assert_started()
         while True:
             try:
-                event = self._event_queue.get(block=final)
+                self.check_workers()
+                event = self._event_queue.get(
+                        block=final,
+                        timeout=RESULT_QUEUE_READ_TIMEOUT
+                    )
             except queue.Empty:
+                if final:
+                    continue
                 return False
             if event is None:
                 log.debug('All workers have completed and all results have '
                           'been processed.')
                 self._status.value = Status.COMPLETE
                 self._send_progress_update()
                 self._completed = True
@@ -761,14 +922,17 @@
                 raise event.data['exception']
             elif event.type == ScanEventType.PROGRESS_UPDATE:
                 if self._is_progress_update_due():
                     self._send_progress_update()
             elif event.type == ScanEventType.LOG_MESSAGE:
                 message: str = event.data['message']
                 log.log(event.data['level'], message)
+            elif event.type == ScanEventType.PROFILE_EVENT:
+                if self._profiler is not None:
+                    self._profiler.add_event(event.data)
         return False
 
     def is_failed(self) -> bool:
         return self._status.value == Status.FAILED
 
 
 class Scanner:
@@ -778,81 +942,99 @@
         self.failed = 0
         self.active = []
 
     def _handle_worker_error(self, error: Exception):
         self.failed += 1
         raise error
 
+    def _initialize_matcher(self) -> Matcher:
+        engine = self.options.match_engine
+        options = dataclasses.replace(self.options.match_engine_options)
+        options.lazy = not USES_FORK
+        return engine.create_matcher(options)
+
     def scan(
                 self,
                 result_processor: ScanResultCallback,
                 progress_receiver: Optional[ProgressReceiverCallback] = None,
                 scan_finished_handler: ScanFinishedCallback =
                 default_scan_finished_handler,
                 use_log_events: bool = False
             ) -> ScanMetrics:
         """Run a scan"""
         timer = timing.Timer()
+        profiler = Profiler() if self.options.profile else None
         event_queue = Queue(MAX_PENDING_RESULTS)
         file_locator_process = FileLocatorProcess(
                 file_filter=self.options.file_filter,
                 use_log_events=use_log_events,
-                event_queue=event_queue if use_log_events else None,
+                event_queue=event_queue if (
+                        use_log_events or profiler is not None
+                    ) else None,
                 allow_io_errors=self.options.allow_io_errors,
-                logging_initializer=self.options.logging_initializer
+                logging_initializer=self.options.logging_initializer,
+                profile=profiler is not None
             )
         file_locator_process.start()
         self.active.append(file_locator_process)
         worker_count = self.options.workers
         if worker_count < 1:
             raise ScanConfigurationException(
                     'Scans require at least one worker'
                 )
         log.debug("Using " + str(worker_count) + " worker(s)...")
-        matcher = RegexMatcher(
-                    self.options.signatures,
-                    match_all=self.options.match_all,
-                    pcre_options=self.options.pcre_options,
-                    lazy=not USES_FORK
-                )
+        matcher = self._initialize_matcher()
         metrics = ScanMetrics(worker_count)
         with ScanWorkerPool(
                     size=worker_count,
                     work_queue=file_locator_process.output_queue,
                     event_queue=event_queue,
                     matcher=matcher,
                     metrics=metrics,
                     timer=timer,
                     progress_receiver=progress_receiver,
                     chunk_size=self.options.chunk_size,
                     scanned_content_limit=self.options.scanned_content_limit,
                     use_log_events=use_log_events,
                     allow_io_errors=self.options.allow_io_errors,
                     debug=self.options.debug,
-                    logging_initializer=self.options.logging_initializer
+                    logging_initializer=self.options.logging_initializer,
+                    profiler=profiler,
+                    direct_io=self.options.direct_io
                 ) as worker_pool:
             def add_path(path: str):
                 while not file_locator_process.add_path(path):
                     worker_pool.await_results(result_processor, final=False)
             self.active.append(worker_pool)
             for path in self.options.paths:
                 add_path(path)
             if self.options.path_source is not None:
                 log.debug('Reading input paths...')
                 while True:
                     path = self.options.path_source.read_entry()
                     if path is None:
                         break
                     add_path(path)
-            file_locator_process.finalize_paths()
+            while not file_locator_process.finalize_paths():
+                worker_pool.await_results(result_processor, final=False)
             log.debug('Awaiting results...')
             worker_pool.await_results(result_processor)
         timer.stop()
         scan_finished_handler = scan_finished_handler if scan_finished_handler\
             else default_scan_finished_handler
         metrics.skipped_files = file_locator_process.get_skipped_count()
         scan_finished_handler(metrics, timer)
+        if profiler is not None:
+            profiler.complete()
+            if self.options.profile_path is None:
+                writer_factory = LogProfileWriterFactory()
+            else:
+                writer_factory = FileProfileWriterFactory(
+                        self.options.profile_path
+                    )
+            with writer_factory as writer:
+                profiler.output_results(writer)
         return (metrics, timer)
 
     def terminate(self) -> None:
         for active in self.active:
             active.terminate()
```

### Comparing `wordfence-3.0.2/wordfence/util/caching.py` & `wordfence-4.0.1/wordfence/util/caching.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import pickle
 import base64
 import time
 import shutil
-from typing import Any, Callable, Optional, Set
+from typing import Any, Callable, Optional, Set, Iterable
 
 from .io import FileLock, LockType
 from .serialization import limited_deserialize
 from ..logging import log
 
 
 DURATION_ONE_DAY = 86400
@@ -21,14 +21,17 @@
     pass
 
 
 class InvalidCachedValueException(CacheException):
     pass
 
 
+CacheFilter = Callable[[Any], Any]
+
+
 class Cache:
 
     def __init__(self):
         self.filters = []
 
     def _serialize_value(self, value: Any) -> Any:
         return value
@@ -41,31 +44,44 @@
 
     def _load(self, key: str, max_age: Optional[int]) -> Any:
         raise NotImplementedError('Loading is not implemented for this cache')
 
     def put(self, key: str, value) -> None:
         self._save(key, self._serialize_value(value))
 
-    def get(self, key: str, max_age: Optional[int] = None) -> Any:
+    def get(
+                self,
+                key: str,
+                max_age: Optional[int] = None,
+                additional_filters: Optional[Iterable[CacheFilter]] = None
+            ) -> Any:
         return self.filter_value(
-                self._deserialize_value(self._load(key, max_age))
+                self._deserialize_value(self._load(key, max_age)),
+                additional_filters
             )
 
     def remove(self, key: str) -> None:
         raise NotImplementedError('Removing is not implemented for this cache')
 
     def purge(self) -> None:
         pass
 
-    def add_filter(self, filter: Callable[[Any], Any]) -> None:
+    def add_filter(self, filter: CacheFilter) -> None:
         self.filters.append(filter)
 
-    def filter_value(self, value: Any) -> Any:
+    def filter_value(
+                self,
+                value: Any,
+                additional_filters: Optional[Iterable[CacheFilter]] = None
+            ) -> Any:
         for filter in self.filters:
             value = filter(value)
+        if additional_filters is not None:
+            for filter in additional_filters:
+                value = filter(value)
         return value
 
 
 class RuntimeCache(Cache):
 
     def __init__(self):
         super().__init__()
@@ -165,26 +181,34 @@
 
 class Cacheable:
 
     def __init__(
                 self,
                 key: str,
                 initializer: Callable[[], Any],
-                max_age: Optional[int] = None
+                max_age: Optional[int] = None,
+                filters: Optional[Iterable[CacheFilter]] = None
             ):
         self.key = key
         self._initializer = initializer
         self.max_age = max_age
+        self.filters = filters
 
     def _initialize_value(self) -> Any:
         return self._initializer()
 
     def get(self, cache: Cache) -> Any:
         try:
-            value = cache.get(self.key, self.max_age)
+            value = cache.get(self.key, self.max_age, self.filters)
         except (
                 NoCachedValueException,
                 InvalidCachedValueException
                 ):
             value = self._initialize_value()
-            cache.put(self.key, value)
+            self.set(cache, value)
         return value
+
+    def set(self, cache: Cache, value: Any) -> None:
+        cache.put(self.key, value)
+
+    def delete(self, cache: Cache) -> Any:
+        cache.remove(self.key)
```

### Comparing `wordfence-3.0.2/wordfence/util/html.py` & `wordfence-4.0.1/wordfence/util/html.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/util/input.py` & `wordfence-4.0.1/wordfence/util/input.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/util/io.py` & `wordfence-4.0.1/wordfence/util/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -276,7 +276,23 @@
             if loop_callback is not None:
                 loop_callback(str(item.path))
             continue
         if item.is_dir():
             yield from iterate_files(item.path, parents, loop_callback)
         else:
             yield item.path
+
+
+def get_umask() -> int:
+    current = os.umask(0)
+    os.umask(current)
+    return current
+
+
+def umask_mode(mode: int) -> int:
+    umask = get_umask()
+    return mode & ~umask
+
+
+def chmod_with_umask(path: str, mode: int = 0o666) -> int:
+    mode = umask_mode(mode)
+    os.chmod(path, mode)
```

### Comparing `wordfence-3.0.2/wordfence/util/pcre.py` & `wordfence-4.0.1/wordfence/util/pcre/bindings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,35 @@
-from ctypes import cdll, c_char_p, c_void_p, c_int, c_ulong, c_ubyte, byref, \
+from ctypes import c_char_p, c_void_p, c_int, c_ulong, c_ubyte, byref, \
         Structure, POINTER, CFUNCTYPE
-from ctypes.util import find_library
 from enum import IntEnum
 from typing import Optional
 
+from ..library import load_library, LibraryNotAvailableException
 
-class PcreException(Exception):
-    pass
-
-
-class PcreLibraryNotAvailableException(PcreException):
-    pass
+from .pcre import PcreException, PcreLibraryNotAvailableException, \
+    PcreOptions, \
+    PCRE_DEFAULT_OPTIONS
 
-
-library_name = find_library('pcre')
-if library_name is None:
-    raise PcreLibraryNotAvailableException('Failed to locate libpcre')
 try:
-    pcre = cdll.LoadLibrary(library_name)
-except OSError as e:
-    raise PcreLibraryNotAvailableException('Failed to load libpcre') from e
+    pcre = load_library('pcre')
+except LibraryNotAvailableException:
+    raise PcreLibraryNotAvailableException('Failed to load libpcre')
 
 
 _pcre_version = pcre.pcre_version
 _pcre_version.argtypes = []
 _pcre_version.restype = c_char_p
 VERSION = _pcre_version().decode('ascii')
 
 
 class PcreError(IntEnum):
     NOMATCH = -1
     NULL = -2
     BADOPTION = -3
-    BADMAGIN = -4
+    BADMAGIC = -4
     UNKNOWN_OPCODE = -5
     NOMEMORY = -6
     NOSUBSTRING = -7
     MATCHLIMIT = -8
     CALLOUT = -9
     BADUTF = -10
     BASEUTF_OFFSET = -11
@@ -170,21 +163,18 @@
     _pcre_jit_exec.restype = c_int
 
 
 PCRE_EXTRA_MATCH_LIMIT = 0x0012
 PCRE_EXTRA_MATCH_LIMIT_RECURSION = 0x0010
 PCRE_STUDY_JIT_COMPILE = 0x0001
 PCRE_STUDY_EXTRA_NEEDED = 0x0008
-PCRE_CASELESS = 0x00000001
 
 
 PCRE_JIT_STACK_MIN_SIZE = 32 * 1024
 PCRE_JIT_STACK_MAX_SIZE = 64 * 1024
-PCRE_DEFAULT_MATCH_LIMIT = 1000000
-PCRE_DEFAULT_MATCH_LIMIT_RECURSION = 100000
 
 
 class PcreJitStack:
 
     def __init__(
                 self,
                 min_size: int = PCRE_JIT_STACK_MIN_SIZE,
@@ -223,39 +213,14 @@
 
 class PcreMatch:
 
     def __init__(self, matched_string: bytes):
         self.matched_string = matched_string
 
 
-class PcreOptions:
-
-    def __init__(
-                self,
-                caseless: bool = False,
-                match_limit: int = PCRE_DEFAULT_MATCH_LIMIT,
-                match_limit_recursion: int = PCRE_DEFAULT_MATCH_LIMIT_RECURSION
-            ):
-        self.caseless = caseless
-        self.match_limit = match_limit
-        self.match_limit_recursion = match_limit_recursion
-        self._compilation_options = None
-
-    def _get_compilation_options(self) -> c_int:
-        if self._compilation_options is None:
-            options = 0
-            if self.caseless:
-                options |= PCRE_CASELESS
-            self._compilation_options = c_int(options)
-        return self._compilation_options
-
-
-PCRE_DEFAULT_OPTIONS = PcreOptions()
-
-
 class PcrePattern:
 
     def __init__(
                 self,
                 pattern: str,
                 options: PcreOptions = PCRE_DEFAULT_OPTIONS
             ):
```

### Comparing `wordfence-3.0.2/wordfence/util/terminal.py` & `wordfence-4.0.1/wordfence/util/terminal.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/util/test_versioning.py` & `wordfence-4.0.1/wordfence/util/test_versioning.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/util/timing.py` & `wordfence-4.0.1/wordfence/util/timing.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/util/units.py` & `wordfence-4.0.1/wordfence/util/units.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/util/updater.py` & `wordfence-4.0.1/wordfence/util/updater.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/util/url.py` & `wordfence-4.0.1/wordfence/util/url.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/util/validation.py` & `wordfence-4.0.1/wordfence/util/validation.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/util/versioning.py` & `wordfence-4.0.1/wordfence/util/versioning.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/wordpress/extension.py` & `wordfence-4.0.1/wordfence/wordpress/extension.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/wordpress/identifier.py` & `wordfence-4.0.1/wordfence/wordpress/identifier.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/wordpress/plugin.py` & `wordfence-4.0.1/wordfence/wordpress/plugin.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/wordpress/remediator.py` & `wordfence-4.0.1/wordfence/wordpress/remediator.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/wordpress/site.py` & `wordfence-4.0.1/wordfence/wordpress/site.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence/wordpress/theme.py` & `wordfence-4.0.1/wordfence/wordpress/theme.py`

 * *Files identical despite different names*

### Comparing `wordfence-3.0.2/wordfence.egg-info/PKG-INFO` & `wordfence-4.0.1/wordfence.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordfence
-Version: 3.0.2
+Version: 4.0.1
 Summary: Command-line malware scanner powered by Wordfence
 Author-email: Wordfence <opensource@wordfence.com>
 Maintainer-email: Wordfence <opensource@wordfence.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -697,15 +697,15 @@
 
 # Wordfence CLI
 
  Wordfence CLI is an open source, high performance, multi-process security scanner, written in Python, that quickly scans network filesystems to detect PHP/other malware and WordPress vulnerabilities. CLI is parallelizable, can be scheduled, can accept input via pipe, and can pipe output to other commands.
 
 ## Installation
 
-We have a number of installation methods to install Wordfence CLI in our [installation documentation](https://github.com/wordfence/wordfence-cli/blob/v3.0.2/docs/Installation.md) which we'd recommend reviewing to get you scanning for malware in as few steps as possible. 
+We have a number of installation methods to install Wordfence CLI in our [installation documentation](https://github.com/wordfence/wordfence-cli/blob/v4.0.1/docs/Installation.md) which we'd recommend reviewing to get you scanning for malware in as few steps as possible. 
 
 We recommend installing using `pip`:
 
 	pip install wordfence
 
 If you'd like to install Wordfence CLI manually or use CLI for development, you can clone the GitHub repo to your local environment:
 
@@ -724,32 +724,32 @@
 
 ### Obtaining a license
 
 Visit [https://www.wordfence.com/products/wordfence-cli/](https://www.wordfence.com/products/wordfence-cli/) to obtain a license to download our signature set.
 
 ## Usage
 
-You can run `wordfence help` for a full list of options that can be passed to Wordfence CLI. Read more about the [configuration options](https://github.com/wordfence/wordfence-cli/blob/v3.0.2/docs/Configuration.md) that can be passed to Wordfence CLI.
+You can run `wordfence help` for a full list of options that can be passed to Wordfence CLI. Read more about the [configuration options](https://github.com/wordfence/wordfence-cli/blob/v4.0.1/docs/Configuration.md) that can be passed to Wordfence CLI.
 
 #### Scanning a directory for malware
 
 Recursively scanning the `/var/www` directory for malware:
 
 	wordfence malware-scan /var/www
 
-A [full list of examples for the malware scan](https://github.com/wordfence/wordfence-cli/blob/v3.0.2/docs/malware-scan/Examples.md) is included in our documentation.
+A [full list of examples for the malware scan](https://github.com/wordfence/wordfence-cli/blob/v4.0.1/docs/malware-scan/Examples.md) is included in our documentation.
 
 #### Scanning a WordPress installation for vulnerabilities
 
 Scanning the `/var/www/wordpress` directory for vulnerabilities. 
 
 	wordfence vuln-scan /var/www/wordpress
 
-A [full list of examples for the vulnerability scan](https://github.com/wordfence/wordfence-cli/blob/v3.0.2/docs/vuln-scan/Examples.md) is included in our documentation.
+A [full list of examples for the vulnerability scan](https://github.com/wordfence/wordfence-cli/blob/v4.0.1/docs/vuln-scan/Examples.md) is included in our documentation.
 
 ## Documentation
 
-The full documentation for Wordfence CLI can be found [here](https://github.com/wordfence/wordfence-cli/blob/v3.0.2/docs/) which includes installation instructions, configuration options, detailed examples, and frequently asked questions.
+The full documentation for Wordfence CLI can be found [here](https://github.com/wordfence/wordfence-cli/blob/v4.0.1/docs/) which includes installation instructions, configuration options, detailed examples, and frequently asked questions.
 
 ## License
 
-Wordfence CLI is open source, licensed under GPLv3. The license can be found [here](https://github.com/wordfence/wordfence-cli/blob/v3.0.2/LICENSE).
+Wordfence CLI is open source, licensed under GPLv3. The license can be found [here](https://github.com/wordfence/wordfence-cli/blob/v4.0.1/LICENSE).
```

### Comparing `wordfence-3.0.2/wordfence.egg-info/SOURCES.txt` & `wordfence-4.0.1/wordfence.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -69,32 +69,46 @@
 wordfence/logging/formatting.py
 wordfence/php/__init__.py
 wordfence/php/lexing.py
 wordfence/php/parsing.py
 wordfence/scanning/__init__.py
 wordfence/scanning/exceptions.py
 wordfence/scanning/filtering.py
-wordfence/scanning/matching.py
 wordfence/scanning/scanner.py
+wordfence/scanning/matching/__init__.py
+wordfence/scanning/matching/matching.py
+wordfence/scanning/matching/pcre.py
+wordfence/scanning/matching/vectorscan.py
 wordfence/util/__init__.py
 wordfence/util/caching.py
+wordfence/util/direct_io.py
 wordfence/util/html.py
 wordfence/util/input.py
 wordfence/util/io.py
-wordfence/util/pcre.py
+wordfence/util/library.py
+wordfence/util/platform.py
+wordfence/util/profiling.py
 wordfence/util/serialization.py
+wordfence/util/signals.py
 wordfence/util/terminal.py
 wordfence/util/test_versioning.py
+wordfence/util/text.py
 wordfence/util/timing.py
 wordfence/util/unicode.py
 wordfence/util/units.py
 wordfence/util/updater.py
 wordfence/util/url.py
 wordfence/util/validation.py
 wordfence/util/versioning.py
+wordfence/util/pcre/__init__.py
+wordfence/util/pcre/bindings.py
+wordfence/util/pcre/pcre.py
+wordfence/util/vectorscan/__init__.py
+wordfence/util/vectorscan/bindings.py
+wordfence/util/vectorscan/vectorscan.py
 wordfence/wordpress/__init__.py
 wordfence/wordpress/exceptions.py
 wordfence/wordpress/extension.py
 wordfence/wordpress/identifier.py
 wordfence/wordpress/plugin.py
 wordfence/wordpress/remediator.py
 wordfence/wordpress/site.py
```


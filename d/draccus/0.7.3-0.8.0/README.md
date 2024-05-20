# Comparing `tmp/draccus-0.7.3.tar.gz` & `tmp/draccus-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draccus-0.7.3.tar", last modified: Wed Apr 17 16:59:48 2024, max compression
+gzip compressed data, was "draccus-0.8.0.tar", last modified: Mon May 20 05:32:58 2024, max compression
```

## Comparing `draccus-0.7.3.tar` & `draccus-0.8.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-04-17 16:59:48.838624 draccus-0.7.3/
--rw-r--r--   0 dlwh       (501) staff       (20)     1179 2023-11-09 05:37:34.000000 draccus-0.7.3/LICENSE
--rw-r--r--   0 dlwh       (501) staff       (20)    23796 2024-04-17 16:59:48.838341 draccus-0.7.3/PKG-INFO
--rw-r--r--   0 dlwh       (501) staff       (20)    21142 2023-11-09 05:37:34.000000 draccus-0.7.3/README.md
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-04-17 16:59:48.826550 draccus-0.7.3/draccus/
--rw-r--r--   0 dlwh       (501) staff       (20)      481 2023-11-09 05:37:34.000000 draccus-0.7.3/draccus/__init__.py
--rw-r--r--   0 dlwh       (501) staff       (20)     7762 2023-12-22 21:08:59.000000 draccus-0.7.3/draccus/argparsing.py
--rw-r--r--   0 dlwh       (501) staff       (20)     1115 2023-12-22 20:35:01.000000 draccus-0.7.3/draccus/cfgparsing.py
--rw-r--r--   0 dlwh       (501) staff       (20)     6592 2023-12-22 21:00:27.000000 draccus-0.7.3/draccus/choice_types.py
--rw-r--r--   0 dlwh       (501) staff       (20)      846 2023-11-09 05:37:34.000000 draccus-0.7.3/draccus/fields.py
--rw-r--r--   0 dlwh       (501) staff       (20)     3262 2023-11-09 05:37:34.000000 draccus-0.7.3/draccus/help_formatter.py
--rw-r--r--   0 dlwh       (501) staff       (20)      849 2023-06-22 17:52:39.000000 draccus-0.7.3/draccus/options.py
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-04-17 16:59:48.829199 draccus-0.7.3/draccus/parsers/
--rw-r--r--   0 dlwh       (501) staff       (20)        0 2023-06-22 00:25:09.000000 draccus-0.7.3/draccus/parsers/__init__.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2244 2023-11-09 05:37:34.000000 draccus-0.7.3/draccus/parsers/config_parsers.py
--rw-r--r--   0 dlwh       (501) staff       (20)    16165 2023-12-24 07:17:29.000000 draccus-0.7.3/draccus/parsers/decoding.py
--rw-r--r--   0 dlwh       (501) staff       (20)     3771 2023-11-09 05:37:34.000000 draccus-0.7.3/draccus/parsers/encoding.py
--rw-r--r--   0 dlwh       (501) staff       (20)     3024 2023-12-24 20:24:14.000000 draccus-0.7.3/draccus/parsers/registry_utils.py
--rw-r--r--   0 dlwh       (501) staff       (20)     3725 2023-11-09 05:37:34.000000 draccus-0.7.3/draccus/parsers/yaml_loader.py
--rw-r--r--   0 dlwh       (501) staff       (20)        0 2023-06-22 00:25:09.000000 draccus-0.7.3/draccus/py.typed
--rw-r--r--   0 dlwh       (501) staff       (20)    12254 2023-12-24 20:24:29.000000 draccus-0.7.3/draccus/utils.py
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-04-17 16:59:48.831241 draccus-0.7.3/draccus/wrappers/
--rw-r--r--   0 dlwh       (501) staff       (20)       88 2023-06-22 00:25:09.000000 draccus-0.7.3/draccus/wrappers/__init__.py
--rw-r--r--   0 dlwh       (501) staff       (20)     4176 2023-11-09 05:37:34.000000 draccus-0.7.3/draccus/wrappers/choice_wrapper.py
--rw-r--r--   0 dlwh       (501) staff       (20)     7356 2023-12-24 07:14:39.000000 draccus-0.7.3/draccus/wrappers/dataclass_wrapper.py
--rw-r--r--   0 dlwh       (501) staff       (20)    10207 2023-11-09 05:37:34.000000 draccus-0.7.3/draccus/wrappers/docstring.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2199 2023-11-09 05:37:34.000000 draccus-0.7.3/draccus/wrappers/field_metavar.py
--rw-r--r--   0 dlwh       (501) staff       (20)    13149 2023-11-28 00:05:42.000000 draccus-0.7.3/draccus/wrappers/field_wrapper.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2113 2023-11-09 05:37:34.000000 draccus-0.7.3/draccus/wrappers/suppressing_argparse.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2123 2023-11-09 05:37:34.000000 draccus-0.7.3/draccus/wrappers/wrapper.py
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-04-17 16:59:48.837658 draccus-0.7.3/draccus.egg-info/
--rw-r--r--   0 dlwh       (501) staff       (20)    23796 2024-04-17 16:59:48.000000 draccus-0.7.3/draccus.egg-info/PKG-INFO
--rw-r--r--   0 dlwh       (501) staff       (20)     1463 2024-04-17 16:59:48.000000 draccus-0.7.3/draccus.egg-info/SOURCES.txt
--rw-r--r--   0 dlwh       (501) staff       (20)        1 2024-04-17 16:59:48.000000 draccus-0.7.3/draccus.egg-info/dependency_links.txt
--rw-r--r--   0 dlwh       (501) staff       (20)      121 2024-04-17 16:59:48.000000 draccus-0.7.3/draccus.egg-info/requires.txt
--rw-r--r--   0 dlwh       (501) staff       (20)       41 2024-04-17 16:59:48.000000 draccus-0.7.3/draccus.egg-info/top_level.txt
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-04-17 16:59:48.831605 draccus-0.7.3/examples/
--rw-r--r--   0 dlwh       (501) staff       (20)     2007 2023-11-09 05:37:34.000000 draccus-0.7.3/examples/choice_class_demo.py
--rw-r--r--   0 dlwh       (501) staff       (20)     1609 2023-11-09 05:37:34.000000 draccus-0.7.3/examples/demo.py
--rw-r--r--   0 dlwh       (501) staff       (20)     1880 2024-04-17 16:58:51.000000 draccus-0.7.3/pyproject.toml
--rw-r--r--   0 dlwh       (501) staff       (20)       38 2024-04-17 16:59:48.838675 draccus-0.7.3/setup.cfg
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-04-17 16:59:48.836508 draccus-0.7.3/tests/
--rw-r--r--   0 dlwh       (501) staff       (20)        0 2023-12-23 07:37:50.000000 draccus-0.7.3/tests/__init__.py
--rw-r--r--   0 dlwh       (501) staff       (20)     6231 2023-11-09 05:37:34.000000 draccus-0.7.3/tests/conftest.py
-drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-04-17 16:59:48.836962 draccus-0.7.3/tests/draccus_choice_plugins/
--rw-r--r--   0 dlwh       (501) staff       (20)      207 2023-06-26 06:28:19.000000 draccus-0.7.3/tests/draccus_choice_plugins/gpt.py
--rw-r--r--   0 dlwh       (501) staff       (20)      437 2023-11-28 00:05:42.000000 draccus-0.7.3/tests/draccus_choice_plugins/model_config.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2153 2023-11-09 05:37:34.000000 draccus-0.7.3/tests/test_argparse_choice_types.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2245 2023-11-28 00:05:42.000000 draccus-0.7.3/tests/test_argparse_choice_types_plugin.py
--rw-r--r--   0 dlwh       (501) staff       (20)     4815 2023-12-24 07:14:39.000000 draccus-0.7.3/tests/test_base.py
--rw-r--r--   0 dlwh       (501) staff       (20)      821 2023-12-23 07:25:55.000000 draccus-0.7.3/tests/test_bools.py
--rw-r--r--   0 dlwh       (501) staff       (20)     1539 2023-12-23 08:39:41.000000 draccus-0.7.3/tests/test_choice_types.py
--rw-r--r--   0 dlwh       (501) staff       (20)     3724 2023-12-24 07:14:36.000000 draccus-0.7.3/tests/test_decoding.py
--rw-r--r--   0 dlwh       (501) staff       (20)      803 2023-12-23 08:41:16.000000 draccus-0.7.3/tests/test_default_args.py
--rw-r--r--   0 dlwh       (501) staff       (20)     3105 2023-06-22 17:52:37.000000 draccus-0.7.3/tests/test_docstrings.py
--rw-r--r--   0 dlwh       (501) staff       (20)     1681 2023-11-09 05:37:34.000000 draccus-0.7.3/tests/test_enums.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2433 2023-11-09 05:37:34.000000 draccus-0.7.3/tests/test_inheritance.py
--rw-r--r--   0 dlwh       (501) staff       (20)     4112 2023-11-28 00:05:42.000000 draccus-0.7.3/tests/test_lists.py
--rw-r--r--   0 dlwh       (501) staff       (20)     3136 2023-06-22 17:34:00.000000 draccus-0.7.3/tests/test_optional.py
--rw-r--r--   0 dlwh       (501) staff       (20)      463 2023-06-22 00:25:09.000000 draccus-0.7.3/tests/test_optional_union.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2516 2023-11-09 05:37:34.000000 draccus-0.7.3/tests/test_preferred_help.py
--rw-r--r--   0 dlwh       (501) staff       (20)     1313 2023-12-23 08:11:15.000000 draccus-0.7.3/tests/test_tuples.py
--rw-r--r--   0 dlwh       (501) staff       (20)     3027 2023-12-23 08:41:06.000000 draccus-0.7.3/tests/test_union.py
--rw-r--r--   0 dlwh       (501) staff       (20)     2348 2023-06-22 17:38:04.000000 draccus-0.7.3/tests/test_utils.py
--rw-r--r--   0 dlwh       (501) staff       (20)     1797 2023-11-09 05:37:34.000000 draccus-0.7.3/tests/test_yaml_inclusion.py
--rw-r--r--   0 dlwh       (501) staff       (20)     4656 2023-11-09 05:37:34.000000 draccus-0.7.3/tests/testutils.py
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-05-20 05:32:58.358389 draccus-0.8.0/
+-rw-r--r--   0 dlwh       (501) staff       (20)     1179 2023-11-09 05:37:34.000000 draccus-0.8.0/LICENSE
+-rw-r--r--   0 dlwh       (501) staff       (20)    23796 2024-05-20 05:32:58.358091 draccus-0.8.0/PKG-INFO
+-rw-r--r--   0 dlwh       (501) staff       (20)    21142 2023-11-09 05:37:34.000000 draccus-0.8.0/README.md
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-05-20 05:32:58.346510 draccus-0.8.0/draccus/
+-rw-r--r--   0 dlwh       (501) staff       (20)      481 2023-11-09 05:37:34.000000 draccus-0.8.0/draccus/__init__.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     7762 2023-12-22 21:08:59.000000 draccus-0.8.0/draccus/argparsing.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     1115 2023-12-22 20:35:01.000000 draccus-0.8.0/draccus/cfgparsing.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     6592 2023-12-22 21:00:27.000000 draccus-0.8.0/draccus/choice_types.py
+-rw-r--r--   0 dlwh       (501) staff       (20)      846 2023-11-09 05:37:34.000000 draccus-0.8.0/draccus/fields.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     3262 2023-11-09 05:37:34.000000 draccus-0.8.0/draccus/help_formatter.py
+-rw-r--r--   0 dlwh       (501) staff       (20)      849 2023-06-22 17:52:39.000000 draccus-0.8.0/draccus/options.py
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-05-20 05:32:58.348778 draccus-0.8.0/draccus/parsers/
+-rw-r--r--   0 dlwh       (501) staff       (20)        0 2023-06-22 00:25:09.000000 draccus-0.8.0/draccus/parsers/__init__.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     2244 2023-11-09 05:37:34.000000 draccus-0.8.0/draccus/parsers/config_parsers.py
+-rw-r--r--   0 dlwh       (501) staff       (20)    16571 2024-05-20 05:27:26.000000 draccus-0.8.0/draccus/parsers/decoding.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     3771 2023-11-09 05:37:34.000000 draccus-0.8.0/draccus/parsers/encoding.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     3024 2023-12-24 20:24:14.000000 draccus-0.8.0/draccus/parsers/registry_utils.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     3725 2023-11-09 05:37:34.000000 draccus-0.8.0/draccus/parsers/yaml_loader.py
+-rw-r--r--   0 dlwh       (501) staff       (20)        0 2023-06-22 00:25:09.000000 draccus-0.8.0/draccus/py.typed
+-rw-r--r--   0 dlwh       (501) staff       (20)    12254 2023-12-24 20:24:29.000000 draccus-0.8.0/draccus/utils.py
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-05-20 05:32:58.350976 draccus-0.8.0/draccus/wrappers/
+-rw-r--r--   0 dlwh       (501) staff       (20)       88 2023-06-22 00:25:09.000000 draccus-0.8.0/draccus/wrappers/__init__.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     4176 2023-11-09 05:37:34.000000 draccus-0.8.0/draccus/wrappers/choice_wrapper.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     7356 2023-12-24 07:14:39.000000 draccus-0.8.0/draccus/wrappers/dataclass_wrapper.py
+-rw-r--r--   0 dlwh       (501) staff       (20)    10207 2023-11-09 05:37:34.000000 draccus-0.8.0/draccus/wrappers/docstring.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     2199 2023-11-09 05:37:34.000000 draccus-0.8.0/draccus/wrappers/field_metavar.py
+-rw-r--r--   0 dlwh       (501) staff       (20)    13149 2023-11-28 00:05:42.000000 draccus-0.8.0/draccus/wrappers/field_wrapper.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     2113 2023-11-09 05:37:34.000000 draccus-0.8.0/draccus/wrappers/suppressing_argparse.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     2123 2023-11-09 05:37:34.000000 draccus-0.8.0/draccus/wrappers/wrapper.py
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-05-20 05:32:58.357406 draccus-0.8.0/draccus.egg-info/
+-rw-r--r--   0 dlwh       (501) staff       (20)    23796 2024-05-20 05:32:58.000000 draccus-0.8.0/draccus.egg-info/PKG-INFO
+-rw-r--r--   0 dlwh       (501) staff       (20)     1463 2024-05-20 05:32:58.000000 draccus-0.8.0/draccus.egg-info/SOURCES.txt
+-rw-r--r--   0 dlwh       (501) staff       (20)        1 2024-05-20 05:32:58.000000 draccus-0.8.0/draccus.egg-info/dependency_links.txt
+-rw-r--r--   0 dlwh       (501) staff       (20)      121 2024-05-20 05:32:58.000000 draccus-0.8.0/draccus.egg-info/requires.txt
+-rw-r--r--   0 dlwh       (501) staff       (20)       41 2024-05-20 05:32:58.000000 draccus-0.8.0/draccus.egg-info/top_level.txt
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-05-20 05:32:58.351362 draccus-0.8.0/examples/
+-rw-r--r--   0 dlwh       (501) staff       (20)     2007 2023-11-09 05:37:34.000000 draccus-0.8.0/examples/choice_class_demo.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     1609 2023-11-09 05:37:34.000000 draccus-0.8.0/examples/demo.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     1880 2024-05-20 05:27:09.000000 draccus-0.8.0/pyproject.toml
+-rw-r--r--   0 dlwh       (501) staff       (20)       38 2024-05-20 05:32:58.358447 draccus-0.8.0/setup.cfg
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-05-20 05:32:58.356412 draccus-0.8.0/tests/
+-rw-r--r--   0 dlwh       (501) staff       (20)        0 2023-12-23 07:37:50.000000 draccus-0.8.0/tests/__init__.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     6231 2023-11-09 05:37:34.000000 draccus-0.8.0/tests/conftest.py
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2024-05-20 05:32:58.356871 draccus-0.8.0/tests/draccus_choice_plugins/
+-rw-r--r--   0 dlwh       (501) staff       (20)      207 2023-06-26 06:28:19.000000 draccus-0.8.0/tests/draccus_choice_plugins/gpt.py
+-rw-r--r--   0 dlwh       (501) staff       (20)      437 2023-11-28 00:05:42.000000 draccus-0.8.0/tests/draccus_choice_plugins/model_config.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     2153 2023-11-09 05:37:34.000000 draccus-0.8.0/tests/test_argparse_choice_types.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     2245 2023-11-28 00:05:42.000000 draccus-0.8.0/tests/test_argparse_choice_types_plugin.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     4815 2023-12-24 07:14:39.000000 draccus-0.8.0/tests/test_base.py
+-rw-r--r--   0 dlwh       (501) staff       (20)      821 2023-12-23 07:25:55.000000 draccus-0.8.0/tests/test_bools.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     1539 2023-12-23 08:39:41.000000 draccus-0.8.0/tests/test_choice_types.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     3724 2023-12-24 07:14:36.000000 draccus-0.8.0/tests/test_decoding.py
+-rw-r--r--   0 dlwh       (501) staff       (20)      803 2023-12-23 08:41:16.000000 draccus-0.8.0/tests/test_default_args.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     3105 2023-06-22 17:52:37.000000 draccus-0.8.0/tests/test_docstrings.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     2384 2024-05-20 05:26:44.000000 draccus-0.8.0/tests/test_enums.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     2433 2023-11-09 05:37:34.000000 draccus-0.8.0/tests/test_inheritance.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     4112 2023-11-28 00:05:42.000000 draccus-0.8.0/tests/test_lists.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     3136 2023-06-22 17:34:00.000000 draccus-0.8.0/tests/test_optional.py
+-rw-r--r--   0 dlwh       (501) staff       (20)      463 2023-06-22 00:25:09.000000 draccus-0.8.0/tests/test_optional_union.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     2516 2023-11-09 05:37:34.000000 draccus-0.8.0/tests/test_preferred_help.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     1313 2023-12-23 08:11:15.000000 draccus-0.8.0/tests/test_tuples.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     3027 2023-12-23 08:41:06.000000 draccus-0.8.0/tests/test_union.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     2348 2023-06-22 17:38:04.000000 draccus-0.8.0/tests/test_utils.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     1797 2023-11-09 05:37:34.000000 draccus-0.8.0/tests/test_yaml_inclusion.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     4656 2023-11-09 05:37:34.000000 draccus-0.8.0/tests/testutils.py
```

### Comparing `draccus-0.7.3/LICENSE` & `draccus-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/PKG-INFO` & `draccus-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draccus
-Version: 0.7.3
+Version: 0.8.0
 Summary: A slightly opinionated framework for simple dataclass-based configurations based on Pyrallis.
 Author-email: David Hall <dlwh@cs.stanford.edu>, Siddharth Karamcheti <skaramcheti@cs.stanford.edu>
 License: MIT License
         
         Copyright (c) 2019 Fabrice Normandin
         Copyright (c) 2021 Elad Richardson
         Copyright (c) 2023 David Hall
```

### Comparing `draccus-0.7.3/README.md` & `draccus-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/draccus/argparsing.py` & `draccus-0.8.0/draccus/argparsing.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/draccus/cfgparsing.py` & `draccus-0.8.0/draccus/cfgparsing.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/draccus/choice_types.py` & `draccus-0.8.0/draccus/choice_types.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/draccus/fields.py` & `draccus-0.8.0/draccus/fields.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/draccus/help_formatter.py` & `draccus-0.8.0/draccus/help_formatter.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/draccus/options.py` & `draccus-0.8.0/draccus/options.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/draccus/parsers/config_parsers.py` & `draccus-0.8.0/draccus/parsers/config_parsers.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/draccus/parsers/decoding.py` & `draccus-0.8.0/draccus/parsers/decoding.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,17 +292,20 @@
 
 def decode_enum(cls: Type[T], raw_value: Any, path) -> T:
     """Decodes a value into an enum."""
     if not is_enum(cls):
         raise Exception(f"Expected an enum type, got {cls}")
 
     try:
-        return cls[raw_value]  # type: ignore
-    except ValueError as e:
-        raise DecodingError(path, f"Couldn't parse '{raw_value}' into an enum of type {cls}") from e
+        return cls(raw_value)  # type: ignore
+    except ValueError:
+        try:
+            return cls[raw_value]  # type: ignore
+        except ValueError as e:
+            raise DecodingError(path, f"Couldn't parse '{raw_value}' into an enum of type {cls}") from e
 
 
 def decode_optional(t: Type[T]) -> DecodingFunction[Optional[T]]:
     decode = get_decoding_fn(t)  # type: ignore
 
     def _decode_optional(raw_value: Any, path: Sequence[str] = ()) -> Optional[T]:
         return raw_value if raw_value is None else decode(raw_value, path)
@@ -349,15 +352,22 @@
                 if first_line:
                     first_line = False
                     message += f"    {descriptor}: {line.strip()}"
                     message += "\n"
                 else:
                     message += f"{' ' * (5 + len(str(descriptor)))}{line}\n"
 
-        raise DecodingError(path, message) from exceptions[next(iter(exceptions))]
+        exception_to_raise_from = next(iter(exceptions.values()))
+        # we'd prefer to find the first exception with an interesting message (not a DecodingError)
+        for ex in exceptions.values():
+            if not isinstance(ex, DecodingError):
+                exception_to_raise_from = ex
+                break
+
+        raise DecodingError(path, message) from exception_to_raise_from
 
     return _try_functions
 
 
 def decode_list(t: Type[T]) -> DecodingFunction[List[T]]:
     decode_item = get_decoding_fn(t)  # type: ignore
```

### Comparing `draccus-0.7.3/draccus/parsers/encoding.py` & `draccus-0.8.0/draccus/parsers/encoding.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/draccus/parsers/registry_utils.py` & `draccus-0.8.0/draccus/parsers/registry_utils.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/draccus/parsers/yaml_loader.py` & `draccus-0.8.0/draccus/parsers/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/draccus/utils.py` & `draccus-0.8.0/draccus/utils.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/draccus/wrappers/choice_wrapper.py` & `draccus-0.8.0/draccus/wrappers/choice_wrapper.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/draccus/wrappers/dataclass_wrapper.py` & `draccus-0.8.0/draccus/wrappers/dataclass_wrapper.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/draccus/wrappers/docstring.py` & `draccus-0.8.0/draccus/wrappers/docstring.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/draccus/wrappers/field_metavar.py` & `draccus-0.8.0/draccus/wrappers/field_metavar.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/draccus/wrappers/field_wrapper.py` & `draccus-0.8.0/draccus/wrappers/field_wrapper.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/draccus/wrappers/suppressing_argparse.py` & `draccus-0.8.0/draccus/wrappers/suppressing_argparse.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/draccus/wrappers/wrapper.py` & `draccus-0.8.0/draccus/wrappers/wrapper.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/draccus.egg-info/PKG-INFO` & `draccus-0.8.0/draccus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draccus
-Version: 0.7.3
+Version: 0.8.0
 Summary: A slightly opinionated framework for simple dataclass-based configurations based on Pyrallis.
 Author-email: David Hall <dlwh@cs.stanford.edu>, Siddharth Karamcheti <skaramcheti@cs.stanford.edu>
 License: MIT License
         
         Copyright (c) 2019 Fabrice Normandin
         Copyright (c) 2021 Elad Richardson
         Copyright (c) 2023 David Hall
```

### Comparing `draccus-0.7.3/draccus.egg-info/SOURCES.txt` & `draccus-0.8.0/draccus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/examples/choice_class_demo.py` & `draccus-0.8.0/examples/choice_class_demo.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/examples/demo.py` & `draccus-0.8.0/examples/demo.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/pyproject.toml` & `draccus-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "draccus"
-version = "0.7.3"
+version = "0.8.0"
 authors = [
   {name = "David Hall", email = "dlwh@cs.stanford.edu"},
   {name = "Siddharth Karamcheti", email = "skaramcheti@cs.stanford.edu"},
 ]
 description = "A slightly opinionated framework for simple dataclass-based configurations based on Pyrallis."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `draccus-0.7.3/tests/conftest.py` & `draccus-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/tests/test_argparse_choice_types.py` & `draccus-0.8.0/tests/test_argparse_choice_types.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/tests/test_argparse_choice_types_plugin.py` & `draccus-0.8.0/tests/test_argparse_choice_types_plugin.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/tests/test_base.py` & `draccus-0.8.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/tests/test_bools.py` & `draccus-0.8.0/tests/test_bools.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/tests/test_choice_types.py` & `draccus-0.8.0/tests/test_choice_types.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/tests/test_decoding.py` & `draccus-0.8.0/tests/test_decoding.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/tests/test_default_args.py` & `draccus-0.8.0/tests/test_default_args.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/tests/test_docstrings.py` & `draccus-0.8.0/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/tests/test_enums.py` & `draccus-0.8.0/tests/test_enums.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,28 +10,53 @@
 class Color(Enum):
     blue: str = auto()  # type: ignore
     red: str = auto()  # type: ignore
     green: str = auto()  # type: ignore
     orange: str = auto()  # type: ignore
 
 
+class BigColor(Enum):
+    BLUE: str = "blue"
+    RED: str = "red"
+    GREEN: str = "green"
+    TRICKY: str = "orange"
+
+
 def test_passing_enum_to_choice():
     @dataclass
     class Something(TestSetup):
         favorite_color: Color = field(default=Color.green)
         colors: List[Color] = field(default_factory=[Color.green].copy)
 
     s = Something.setup("")
     assert s.favorite_color == Color.green
     assert s.colors == [Color.green]
 
     s = Something.setup("--colors [blue,red]")
     assert s.colors == [Color.blue, Color.red]
 
 
+def test_passing_enum_to_choice_from_value():
+    @dataclass
+    class Something(TestSetup):
+        favorite_color: BigColor = field(default=BigColor.GREEN)
+        colors: List[BigColor] = field(default_factory=[BigColor.GREEN].copy)
+
+    s = Something.setup("")
+    assert s.favorite_color == BigColor.GREEN
+    assert s.colors == [BigColor.GREEN]
+
+    s = Something.setup("--colors '[blue, red]'")
+    assert s.colors == [BigColor.BLUE, BigColor.RED]
+
+    # try tricky
+    s = Something.setup("--colors '[blue,orange]'")
+    assert s.colors == [BigColor.BLUE, BigColor.TRICKY]
+
+
 #
 #
 def test_passing_enum_to_choice_no_default_makes_required_arg():
     @dataclass
     class Something(TestSetup):
         favorite_color: Color = field()
```

### Comparing `draccus-0.7.3/tests/test_inheritance.py` & `draccus-0.8.0/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/tests/test_lists.py` & `draccus-0.8.0/tests/test_lists.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/tests/test_optional.py` & `draccus-0.8.0/tests/test_optional.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/tests/test_preferred_help.py` & `draccus-0.8.0/tests/test_preferred_help.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/tests/test_tuples.py` & `draccus-0.8.0/tests/test_tuples.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/tests/test_union.py` & `draccus-0.8.0/tests/test_union.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/tests/test_utils.py` & `draccus-0.8.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/tests/test_yaml_inclusion.py` & `draccus-0.8.0/tests/test_yaml_inclusion.py`

 * *Files identical despite different names*

### Comparing `draccus-0.7.3/tests/testutils.py` & `draccus-0.8.0/tests/testutils.py`

 * *Files identical despite different names*


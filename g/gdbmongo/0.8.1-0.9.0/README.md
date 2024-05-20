# Comparing `tmp/gdbmongo-0.8.1.tar.gz` & `tmp/gdbmongo-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdbmongo-0.8.1.tar", last modified: Sat Mar  4 15:43:57 2023, max compression
+gzip compressed data, was "gdbmongo-0.9.0.tar", last modified: Sat Aug 26 14:18:37 2023, max compression
```

## Comparing `gdbmongo-0.8.1.tar` & `gdbmongo-0.9.0.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 15:43:57.070182 gdbmongo-0.8.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2762 2022-02-19 19:02:45.000000 gdbmongo-0.8.1/.gitignore
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1561 2023-03-04 15:31:52.000000 gdbmongo-0.8.1/CHANGELOG.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      259 2022-02-26 03:31:36.000000 gdbmongo-0.8.1/CONTRIBUTING.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2022-02-19 18:35:21.000000 gdbmongo-0.8.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6341 2023-03-04 15:43:57.070182 gdbmongo-0.8.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3809 2023-02-04 16:43:40.000000 gdbmongo-0.8.1/README.rst
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 15:43:57.066182 gdbmongo-0.8.1/gdbmongo/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2022-02-26 20:57:41.000000 gdbmongo-0.8.1/gdbmongo/.gitignore
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1361 2022-03-13 00:09:21.000000 gdbmongo-0.8.1/gdbmongo/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      160 2023-03-04 15:43:57.000000 gdbmongo-0.8.1/gdbmongo/_version.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8180 2022-12-24 16:01:18.000000 gdbmongo-0.8.1/gdbmongo/abseil_printers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2988 2023-03-04 15:31:52.000000 gdbmongo-0.8.1/gdbmongo/boost_printers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10112 2022-04-02 17:37:00.000000 gdbmongo-0.8.1/gdbmongo/bsonmisc_printer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19133 2022-07-23 12:02:30.000000 gdbmongo-0.8.1/gdbmongo/bsonobj_printer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3312 2022-04-02 17:37:00.000000 gdbmongo-0.8.1/gdbmongo/date_printer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8525 2022-12-24 16:01:18.000000 gdbmongo-0.8.1/gdbmongo/decorable_printer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6348 2022-12-23 15:04:20.000000 gdbmongo-0.8.1/gdbmongo/detect_toolchain.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8885 2023-03-04 15:20:48.000000 gdbmongo-0.8.1/gdbmongo/interaction.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22317 2022-12-24 16:01:18.000000 gdbmongo-0.8.1/gdbmongo/lock_manager_printer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2720 2022-04-02 17:37:00.000000 gdbmongo-0.8.1/gdbmongo/objectid_printer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1844 2022-03-26 02:52:20.000000 gdbmongo-0.8.1/gdbmongo/printer_protocol.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4766 2022-07-31 12:36:14.000000 gdbmongo-0.8.1/gdbmongo/status_printer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2176 2022-12-24 16:01:18.000000 gdbmongo-0.8.1/gdbmongo/stdlib_printers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7230 2022-12-24 16:01:18.000000 gdbmongo-0.8.1/gdbmongo/stdlib_printers.pyi
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2641 2023-01-15 23:33:46.000000 gdbmongo-0.8.1/gdbmongo/stdlib_printers_loader.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2096 2022-03-30 02:03:29.000000 gdbmongo-0.8.1/gdbmongo/stdlib_xmethods.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13677 2022-03-29 02:44:28.000000 gdbmongo-0.8.1/gdbmongo/stdlib_xmethods.pyi
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6021 2022-04-02 17:37:00.000000 gdbmongo-0.8.1/gdbmongo/string_data_printer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3736 2023-02-04 16:43:40.000000 gdbmongo-0.8.1/gdbmongo/thread_name_printer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2022-04-02 17:37:00.000000 gdbmongo-0.8.1/gdbmongo/timestamp_printer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2846 2022-07-23 12:02:30.000000 gdbmongo-0.8.1/gdbmongo/uuid_printer.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 15:43:57.066182 gdbmongo-0.8.1/gdbmongo.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6341 2023-03-04 15:43:57.000000 gdbmongo-0.8.1/gdbmongo.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1554 2023-03-04 15:43:57.000000 gdbmongo-0.8.1/gdbmongo.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-04 15:43:57.000000 gdbmongo-0.8.1/gdbmongo.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-02-19 19:47:10.000000 gdbmongo-0.8.1/gdbmongo.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-03-04 15:43:57.000000 gdbmongo-0.8.1/gdbmongo.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1076 2023-01-22 02:12:14.000000 gdbmongo-0.8.1/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      998 2023-03-04 15:43:57.070182 gdbmongo-0.8.1/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 15:43:57.062183 gdbmongo-0.8.1/stubs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 15:43:57.070182 gdbmongo-0.8.1/stubs/gdb/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3077 2023-02-04 16:43:40.000000 gdbmongo-0.8.1/stubs/gdb/__init__.pyi
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      732 2023-02-04 16:43:40.000000 gdbmongo-0.8.1/stubs/gdb/_architecture.pyi
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1033 2022-03-12 19:45:56.000000 gdbmongo-0.8.1/stubs/gdb/_basic.pyi
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      774 2022-03-12 19:45:56.000000 gdbmongo-0.8.1/stubs/gdb/_errors.pyi
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1213 2023-02-04 16:43:40.000000 gdbmongo-0.8.1/stubs/gdb/_frame.pyi
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1395 2023-02-04 16:43:40.000000 gdbmongo-0.8.1/stubs/gdb/_inferior.pyi
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1331 2023-02-04 16:43:40.000000 gdbmongo-0.8.1/stubs/gdb/_inferiorthread.pyi
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1047 2022-03-26 02:52:20.000000 gdbmongo-0.8.1/stubs/gdb/_lazy_string.pyi
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      735 2022-03-12 19:45:56.000000 gdbmongo-0.8.1/stubs/gdb/_objfile.pyi
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      776 2023-02-04 16:43:40.000000 gdbmongo-0.8.1/stubs/gdb/_progspace.pyi
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      946 2022-03-12 19:45:56.000000 gdbmongo-0.8.1/stubs/gdb/_symbol.pyi
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2096 2022-03-30 03:41:46.000000 gdbmongo-0.8.1/stubs/gdb/_type.pyi
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2759 2022-04-02 17:37:00.000000 gdbmongo-0.8.1/stubs/gdb/_value.pyi
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-02-04 16:43:40.000000 gdbmongo-0.8.1/stubs/gdb/events.pyi
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2839 2022-03-30 02:03:29.000000 gdbmongo-0.8.1/stubs/gdb/printing.pyi
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      791 2022-03-13 03:14:23.000000 gdbmongo-0.8.1/stubs/gdb/xmethod.pyi
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 15:43:57.070182 gdbmongo-0.8.1/stubs/pydocstyle/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      635 2022-03-13 00:09:21.000000 gdbmongo-0.8.1/stubs/pydocstyle/__init__.pyi
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      674 2022-03-13 00:09:21.000000 gdbmongo-0.8.1/stubs/pydocstyle/cli.pyi
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 15:43:57.070182 gdbmongo-0.8.1/stubs/pylint/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      631 2022-03-12 23:49:49.000000 gdbmongo-0.8.1/stubs/pylint/__init__.pyi
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      905 2022-03-12 19:45:56.000000 gdbmongo-0.8.1/stubs/pylint/lint.pyi
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 15:43:57.070182 gdbmongo-0.8.1/stubs/yapf/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      699 2022-03-12 19:45:56.000000 gdbmongo-0.8.1/stubs/yapf/__init__.pyi
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-04 15:43:57.070182 gdbmongo-0.8.1/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6847 2023-02-26 15:05:07.000000 gdbmongo-0.8.1/tests/test_detect_toolchain.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2609 2022-12-23 15:04:20.000000 gdbmongo-0.8.1/tests/test_formatting.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3369 2023-03-04 13:14:28.000000 gdbmongo-0.8.1/tests/test_interaction.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2671 2022-07-23 02:19:06.000000 gdbmongo-0.8.1/tests/test_linting.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4388 2022-12-23 15:04:20.000000 gdbmongo-0.8.1/tests/test_stdlib_printers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      622 2023-01-22 02:12:19.000000 gdbmongo-0.8.1/tox.ini
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-26 14:18:37.684023 gdbmongo-0.9.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2762 2022-02-19 19:02:45.000000 gdbmongo-0.9.0/.gitignore
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1662 2023-08-26 14:17:38.000000 gdbmongo-0.9.0/CHANGELOG.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      259 2022-02-26 03:31:36.000000 gdbmongo-0.9.0/CONTRIBUTING.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2022-02-19 18:35:21.000000 gdbmongo-0.9.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6479 2023-08-26 14:18:37.684023 gdbmongo-0.9.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3809 2023-02-04 16:43:40.000000 gdbmongo-0.9.0/README.rst
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-26 14:18:37.684023 gdbmongo-0.9.0/gdbmongo/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2022-02-26 20:57:41.000000 gdbmongo-0.9.0/gdbmongo/.gitignore
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1361 2022-03-13 00:09:21.000000 gdbmongo-0.9.0/gdbmongo/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      160 2023-08-26 14:18:37.000000 gdbmongo-0.9.0/gdbmongo/_version.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8218 2023-08-12 16:03:32.000000 gdbmongo-0.9.0/gdbmongo/abseil_printers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3656 2023-08-26 14:17:38.000000 gdbmongo-0.9.0/gdbmongo/boost_printers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10112 2022-04-02 17:37:00.000000 gdbmongo-0.9.0/gdbmongo/bsonmisc_printer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19133 2022-07-23 12:02:30.000000 gdbmongo-0.9.0/gdbmongo/bsonobj_printer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3312 2022-04-02 17:37:00.000000 gdbmongo-0.9.0/gdbmongo/date_printer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8525 2022-12-24 16:01:18.000000 gdbmongo-0.9.0/gdbmongo/decorable_printer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6348 2022-12-23 15:04:20.000000 gdbmongo-0.9.0/gdbmongo/detect_toolchain.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8980 2023-08-26 14:17:38.000000 gdbmongo-0.9.0/gdbmongo/interaction.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24089 2023-08-26 14:17:38.000000 gdbmongo-0.9.0/gdbmongo/lock_manager_printer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2720 2022-04-02 17:37:00.000000 gdbmongo-0.9.0/gdbmongo/objectid_printer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1844 2022-03-26 02:52:20.000000 gdbmongo-0.9.0/gdbmongo/printer_protocol.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1798 2023-08-26 14:17:38.000000 gdbmongo-0.9.0/gdbmongo/static_immortal_printer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4766 2022-07-31 12:36:14.000000 gdbmongo-0.9.0/gdbmongo/status_printer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2176 2022-12-24 16:01:18.000000 gdbmongo-0.9.0/gdbmongo/stdlib_printers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7230 2022-12-24 16:01:18.000000 gdbmongo-0.9.0/gdbmongo/stdlib_printers.pyi
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2641 2023-01-15 23:33:46.000000 gdbmongo-0.9.0/gdbmongo/stdlib_printers_loader.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2096 2022-03-30 02:03:29.000000 gdbmongo-0.9.0/gdbmongo/stdlib_xmethods.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13677 2022-03-29 02:44:28.000000 gdbmongo-0.9.0/gdbmongo/stdlib_xmethods.pyi
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6021 2022-04-02 17:37:00.000000 gdbmongo-0.9.0/gdbmongo/string_data_printer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3736 2023-02-04 16:43:40.000000 gdbmongo-0.9.0/gdbmongo/thread_name_printer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2022-04-02 17:37:00.000000 gdbmongo-0.9.0/gdbmongo/timestamp_printer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2846 2022-07-23 12:02:30.000000 gdbmongo-0.9.0/gdbmongo/uuid_printer.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-26 14:18:37.684023 gdbmongo-0.9.0/gdbmongo.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6479 2023-08-26 14:18:37.000000 gdbmongo-0.9.0/gdbmongo.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1590 2023-08-26 14:18:37.000000 gdbmongo-0.9.0/gdbmongo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-08-26 14:18:37.000000 gdbmongo-0.9.0/gdbmongo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-02-19 19:47:10.000000 gdbmongo-0.9.0/gdbmongo.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-08-26 14:18:37.000000 gdbmongo-0.9.0/gdbmongo.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1076 2023-01-22 02:12:14.000000 gdbmongo-0.9.0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1041 2023-08-26 14:18:37.684023 gdbmongo-0.9.0/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-26 14:18:37.680024 gdbmongo-0.9.0/stubs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-26 14:18:37.684023 gdbmongo-0.9.0/stubs/gdb/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3077 2023-02-04 16:43:40.000000 gdbmongo-0.9.0/stubs/gdb/__init__.pyi
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      732 2023-02-04 16:43:40.000000 gdbmongo-0.9.0/stubs/gdb/_architecture.pyi
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1033 2022-03-12 19:45:56.000000 gdbmongo-0.9.0/stubs/gdb/_basic.pyi
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      774 2022-03-12 19:45:56.000000 gdbmongo-0.9.0/stubs/gdb/_errors.pyi
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1213 2023-02-04 16:43:40.000000 gdbmongo-0.9.0/stubs/gdb/_frame.pyi
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1395 2023-02-04 16:43:40.000000 gdbmongo-0.9.0/stubs/gdb/_inferior.pyi
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1331 2023-02-04 16:43:40.000000 gdbmongo-0.9.0/stubs/gdb/_inferiorthread.pyi
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1047 2022-03-26 02:52:20.000000 gdbmongo-0.9.0/stubs/gdb/_lazy_string.pyi
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      735 2022-03-12 19:45:56.000000 gdbmongo-0.9.0/stubs/gdb/_objfile.pyi
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      776 2023-02-04 16:43:40.000000 gdbmongo-0.9.0/stubs/gdb/_progspace.pyi
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      946 2022-03-12 19:45:56.000000 gdbmongo-0.9.0/stubs/gdb/_symbol.pyi
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2096 2022-03-30 03:41:46.000000 gdbmongo-0.9.0/stubs/gdb/_type.pyi
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2759 2022-04-02 17:37:00.000000 gdbmongo-0.9.0/stubs/gdb/_value.pyi
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-02-04 16:43:40.000000 gdbmongo-0.9.0/stubs/gdb/events.pyi
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2839 2022-03-30 02:03:29.000000 gdbmongo-0.9.0/stubs/gdb/printing.pyi
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      791 2022-03-13 03:14:23.000000 gdbmongo-0.9.0/stubs/gdb/xmethod.pyi
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-26 14:18:37.684023 gdbmongo-0.9.0/stubs/pydocstyle/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      635 2022-03-13 00:09:21.000000 gdbmongo-0.9.0/stubs/pydocstyle/__init__.pyi
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      674 2022-03-13 00:09:21.000000 gdbmongo-0.9.0/stubs/pydocstyle/cli.pyi
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-26 14:18:37.684023 gdbmongo-0.9.0/stubs/pylint/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      631 2022-03-12 23:49:49.000000 gdbmongo-0.9.0/stubs/pylint/__init__.pyi
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      905 2022-03-12 19:45:56.000000 gdbmongo-0.9.0/stubs/pylint/lint.pyi
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-26 14:18:37.684023 gdbmongo-0.9.0/stubs/yapf/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      699 2022-03-12 19:45:56.000000 gdbmongo-0.9.0/stubs/yapf/__init__.pyi
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-26 14:18:37.684023 gdbmongo-0.9.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6847 2023-03-04 15:58:53.000000 gdbmongo-0.9.0/tests/test_detect_toolchain.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2609 2022-12-23 15:04:20.000000 gdbmongo-0.9.0/tests/test_formatting.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3369 2023-03-04 15:58:53.000000 gdbmongo-0.9.0/tests/test_interaction.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2671 2022-07-23 02:19:06.000000 gdbmongo-0.9.0/tests/test_linting.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4388 2022-12-23 15:04:20.000000 gdbmongo-0.9.0/tests/test_stdlib_printers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      622 2023-01-22 02:12:19.000000 gdbmongo-0.9.0/tox.ini
```

### Comparing `gdbmongo-0.8.1/.gitignore` & `gdbmongo-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/CHANGELOG.rst` & `gdbmongo-0.9.0/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+0.9.0 (2023-08-26)
+------------------
+
+* Support dumping LockManager from core dump of MongoDB 7.0.
+
 0.8.1 (2023-03-04)
 ------------------
 
 * Fix two Python exceptions from thread names logic when no program or core dump was loaded.
 * Fix boost::optional pretty printer for scalar types.
 
 0.8.0 (2023-02-04)
```

### Comparing `gdbmongo-0.8.1/LICENSE` & `gdbmongo-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/PKG-INFO` & `gdbmongo-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdbmongo
-Version: 0.8.1
+Version: 0.9.0
 Summary: GDB pretty printers and commands for debugging the MongoDB Server
 Home-page: https://github.com/visemet/gdb-mongodb-server
 Maintainer: Max Hirschhorn
 Maintainer-email: max.hirschhorn@mongodb.com
 License: Apache License, Version 2.0
 Keywords: mongo,mongodb,gdb
 Platform: linux
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Debuggers
 Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ==================
 gdb-mongodb-server
 ==================
 
 About
@@ -119,14 +120,19 @@
 
     (gdb) python lock_mgr = gdbmongo.LockManagerPrinter.from_global()
     (gdb) python print(lock_mgr.val)
 
 Changelog
 =========
 
+0.9.0 (2023-08-26)
+------------------
+
+* Support dumping LockManager from core dump of MongoDB 7.0.
+
 0.8.1 (2023-03-04)
 ------------------
 
 * Fix two Python exceptions from thread names logic when no program or core dump was loaded.
 * Fix boost::optional pretty printer for scalar types.
 
 0.8.0 (2023-02-04)
```

### Comparing `gdbmongo-0.8.1/README.rst` & `gdbmongo-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/gdbmongo/__init__.py` & `gdbmongo-0.9.0/gdbmongo/__init__.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/gdbmongo/abseil_printers.py` & `gdbmongo-0.9.0/gdbmongo/abseil_printers.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ###
-"""Pretty printers for absl:: container types."""
+"""Pretty-printers for absl:: container types."""
 
 import typing
 
 import gdb
 
 from gdbmongo import stdlib_printers
 from gdbmongo.printer_protocol import PrettyPrinterProtocol, SupportsDisplayHint
@@ -48,16 +48,16 @@
     derived class.
     """
     capacity = int(container["capacity_"])
     ctrl = container["ctrl_"]
     slots = container["slots_"]
 
     # We search for any in-use `slots_` among the `ctrl_` bytes and return them.
-    # https://github.com/mongodb/mongo/blob/r5.3.0-rc1/src/third_party/abseil-cpp-master/abseil-cpp/absl/container/internal/raw_hash_set.h#L1817-L1820
-    # https://github.com/mongodb/mongo/blob/r5.3.0-rc1/src/third_party/abseil-cpp-master/abseil-cpp/absl/container/internal/raw_hash_set.h#L315
+    # https://github.com/mongodb/mongo/blob/r7.0.0/src/third_party/abseil-cpp/dist/absl/container/internal/raw_hash_set.h#L1948-L1951
+    # https://github.com/mongodb/mongo/blob/r7.0.0/src/third_party/abseil-cpp/dist/absl/container/internal/raw_hash_set.h#L330
     for i in range(capacity):
         is_full = int(ctrl[i]) >= 0
         if is_full:
             yield slots[i]
 
 
 # pylint: disable-next=missing-class-docstring
@@ -100,29 +100,29 @@
         raise NotImplementedError("AbslHashSetPrinterBase._extract_element")
 
 
 class AbslNodeHashSetPrinter(AbslHashSetPrinterBase):
     """Pretty-printer for absl::node_hash_set<T>."""
 
     template_name = "absl::node_hash_set"
-    type_aliases = ("absl::lts_20210324::node_hash_set", )
+    type_aliases = ("absl::lts_20210324::node_hash_set", "absl::lts_20211102::node_hash_set")
 
     def _extract_element(self, elem_val: gdb.Value, /) -> gdb.Value:
-        # https://github.com/mongodb/mongo/blob/r5.3.0-rc1/src/third_party/abseil-cpp-master/abseil-cpp/absl/container/internal/node_hash_policy.h#L75
+        # https://github.com/mongodb/mongo/blob/r7.0.0/src/third_party/abseil-cpp/dist/absl/container/internal/node_hash_policy.h#L75
         return elem_val.dereference()
 
 
 class AbslFlatHashSetPrinter(AbslHashSetPrinterBase):
     """Pretty-printer for absl::flat_hash_set<T>."""
 
     template_name = "absl::flat_hash_set"
-    type_aliases = ("absl::lts_20210324::flat_hash_set", )
+    type_aliases = ("absl::lts_20210324::flat_hash_set", "absl::lts_20211102::flat_hash_set")
 
     def _extract_element(self, elem_val: gdb.Value, /) -> gdb.Value:
-        # https://github.com/mongodb/mongo/blob/r5.3.0-rc1/src/third_party/abseil-cpp-master/abseil-cpp/absl/container/flat_hash_set.h#L478
+        # https://github.com/mongodb/mongo/blob/r7.0.0/src/third_party/abseil-cpp/dist/absl/container/flat_hash_set.h#L478
         return elem_val
 
 
 class AbslHashMapPrinterBase(AbslPrinterProtocol):
     # pylint: disable=missing-function-docstring
     """Pretty-printer base class for absl::node_hash_map<K, V> and absl::flat_hash_map<K, V>."""
 
@@ -162,31 +162,31 @@
         raise NotImplementedError("AbslHashMapPrinterBase._extract_key_value_pair")
 
 
 class AbslNodeHashMapPrinter(AbslHashMapPrinterBase):
     """Pretty-printer for absl::node_hash_map<K, V>."""
 
     template_name = "absl::node_hash_map"
-    type_aliases = ("absl::lts_20210324::node_hash_map", )
+    type_aliases = ("absl::lts_20210324::node_hash_map", "absl::lts_20211102::node_hash_map")
 
     def _extract_key_value_pair(self, kvp_value: gdb.Value,
                                 /) -> typing.Tuple[gdb.Value, gdb.Value]:
-        # https://github.com/mongodb/mongo/blob/r5.3.0-rc1/src/third_party/abseil-cpp-master/abseil-cpp/absl/container/node_hash_map.h#L580
+        # https://github.com/mongodb/mongo/blob/r7.0.0/src/third_party/abseil-cpp/dist/absl/container/node_hash_map.h#L580
         return (kvp_value["first"], kvp_value["second"])
 
 
 class AbslFlatHashMapPrinter(AbslHashMapPrinterBase):
     """Pretty-printer for absl::flat_hash_map<K, V>."""
 
     template_name = "absl::flat_hash_map"
-    type_aliases = ("absl::lts_20210324::flat_hash_map", )
+    type_aliases = ("absl::lts_20210324::flat_hash_map", "absl::lts_20211102::flat_hash_map")
 
     def _extract_key_value_pair(self, kvp_value: gdb.Value,
                                 /) -> typing.Tuple[gdb.Value, gdb.Value]:
-        # https://github.com/mongodb/mongo/blob/r5.3.0-rc1/src/third_party/abseil-cpp-master/abseil-cpp/absl/container/flat_hash_map.h#L586-L588
+        # https://github.com/mongodb/mongo/blob/r7.0.0/src/third_party/abseil-cpp/dist/absl/container/flat_hash_map.h#L586-L588
         return (kvp_value["key"], kvp_value["value"]["second"])
 
 
 def add_printers(pretty_printer: gdb.printing.RegexpCollectionPrettyPrinter, /) -> None:
     """Add the Abseil printers to the pretty printer collection given."""
     for printer in (AbslNodeHashSetPrinter, AbslFlatHashSetPrinter, AbslNodeHashMapPrinter,
                     AbslFlatHashMapPrinter):
```

### Comparing `gdbmongo-0.8.1/gdbmongo/boost_printers.py` & `gdbmongo-0.9.0/gdbmongo/boost_printers.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,61 +11,81 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ###
 """Pretty-printers for boost:: types."""
 
+import abc
 import typing
 
 import gdb
 
 from gdbmongo.abseil_printers import gdb_resolve_type
-from gdbmongo.printer_protocol import PrettyPrinterProtocol
+from gdbmongo.printer_protocol import PrettyPrinterProtocol, SupportsChildren, SupportsDisplayHint
 
 
-class BoostOptionalPrinter(PrettyPrinterProtocol):
+class SingletonPrinterBase(SupportsChildren, SupportsDisplayHint):
+    # pylint: disable=missing-function-docstring
+    """Class to define conventions for displaying a container of a single value."""
+
+    @staticmethod
+    def display_hint() -> typing.Literal["array"]:
+        return "array"
+
+    def children(self) -> typing.Iterator[typing.Tuple[str, gdb.Value]]:
+        # Ideally we would have returned `contained_value` in the to_string() method and skipped
+        # defining a children() method at all. But that approach causes GDB to not display the
+        # addresses for Xmethods like get() on std::unique_ptr and std::shared_ptr types for any
+        # members within `contained_value`. We display the contained value as if it was an array of
+        # size 1 to keep the GDB output more compact as a compromise.
+        contained_value = self.value()
+        yield ("", contained_value)
+
+    @abc.abstractmethod
+    def value(self) -> gdb.Value:
+        """Return the contained value."""
+        raise NotImplementedError
+
+
+class BoostOptionalPrinter(PrettyPrinterProtocol, SingletonPrinterBase):
     # pylint: disable=missing-function-docstring
     """Pretty-printer for boost::optional<T>."""
 
     def __init__(self, val: gdb.Value, /) -> None:
         self.element_type = val.type.template_argument(0)
         self.is_initialized = bool(val["m_initialized"])
         self.val = val
 
         gdb_resolve_type(self.element_type)
 
-    @staticmethod
-    def display_hint() -> typing.Literal["array"]:
-        return "array"
-
     def to_string(self) -> str:
         if self.is_initialized:
             return f"boost::optional<{self.element_type}>"
 
         return "boost::none"
 
     def children(self) -> typing.Iterator[typing.Tuple[str, gdb.Value]]:
         if self.is_initialized:
-            storage = self.val["m_storage"]
-            # boost::optional<T> is either stored using boost::optional_detail::aligned_storage<T>
-            # or using direct storage of `T`. Scalar types are able to take advantage of direct
-            # storage.
-            #
-            # https://www.boost.org/doc/libs/1_79_0/libs/optional/doc/html/boost_optional/tutorial/performance_considerations.html
-            if storage.type.strip_typedefs().code == gdb.TYPE_CODE_STRUCT:
-                storage = storage["dummy_"]["data"]
-                contained_value = storage.cast(self.element_type.pointer()).dereference()
-            else:
-                contained_value = storage
-
-            # Ideally we would have returned `contained_value` in the to_string() method and skipped
-            # defining a children() method at all. But that approach causes GDB to not display the
-            # addresses for Xmethods like get() on std::unique_ptr and std::shared_ptr types for any
-            # members within `contained_value`. We display the engaged boost::optional as if it was
-            # an array of size 1 to keep the GDB output more compact as a compromise.
-            yield ("", contained_value)
+            yield from SingletonPrinterBase.children(self)
+
+    def value(self) -> gdb.Value:
+        if not self.is_initialized:
+            raise ValueError("Cannot extract value from boost::none")
+
+        storage = self.val["m_storage"]
+        # boost::optional<T> is either stored using boost::optional_detail::aligned_storage<T> or
+        # using direct storage of `T`. Scalar types are able to take advantage of direct storage.
+        #
+        # https://www.boost.org/doc/libs/1_79_0/libs/optional/doc/html/boost_optional/tutorial/performance_considerations.html
+        if storage.type.strip_typedefs().code == gdb.TYPE_CODE_STRUCT:
+            storage = storage["dummy_"]["data"]
+            contained_value = storage.cast(self.element_type.pointer()).dereference()
+        else:
+            contained_value = storage
+
+        return contained_value
 
 
 def add_printers(pretty_printer: gdb.printing.RegexpCollectionPrettyPrinter, /) -> None:
     """Add the Boost printers to the pretty printer collection given."""
     pretty_printer.add_printer("boost::optional", "^boost::optional<.*>$", BoostOptionalPrinter)
```

### Comparing `gdbmongo-0.8.1/gdbmongo/bsonmisc_printer.py` & `gdbmongo-0.9.0/gdbmongo/bsonmisc_printer.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/gdbmongo/bsonobj_printer.py` & `gdbmongo-0.9.0/gdbmongo/bsonobj_printer.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/gdbmongo/date_printer.py` & `gdbmongo-0.9.0/gdbmongo/date_printer.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/gdbmongo/decorable_printer.py` & `gdbmongo-0.9.0/gdbmongo/decorable_printer.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/gdbmongo/detect_toolchain.py` & `gdbmongo-0.9.0/gdbmongo/detect_toolchain.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/gdbmongo/interaction.py` & `gdbmongo-0.9.0/gdbmongo/interaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 import warnings
 
 import gdb
 import gdb.printing
 
 from gdbmongo import (abseil_printers, boost_printers, bsonmisc_printer, bsonobj_printer,
                       date_printer, decorable_printer, lock_manager_printer, objectid_printer,
-                      status_printer, string_data_printer, thread_name_printer, timestamp_printer,
-                      uuid_printer)
+                      static_immortal_printer, status_printer, string_data_printer,
+                      thread_name_printer, timestamp_printer, uuid_printer)
 from gdbmongo.detect_toolchain import ToolchainVersionDetector
 from gdbmongo.printer_protocol import SupportsChildren, SupportsToString
 from gdbmongo.stdlib_printers_loader import resolve_import
 
 
 def _import_libstdcxx_printers(executable: str, /, *, register_libstdcxx_printers: bool) -> None:
     """Import the version of the libstdc++ GDB pretty printers corresponding to the version of the
@@ -110,14 +110,15 @@
     pretty_printer_mongo_extras = RegexpCollectionPrettyPrinter("gdbmongo-mongo-extras")
     pretty_printer_mongo_extras.enabled = mongo_extras
     bsonmisc_printer.add_printers(pretty_printer_mongo_extras)
     bsonobj_printer.add_printers(pretty_printer_mongo_extras)
     date_printer.add_printers(pretty_printer_mongo_extras)
     decorable_printer.add_printers(pretty_printer_mongo_extras)
     objectid_printer.add_printers(pretty_printer_mongo_extras)
+    static_immortal_printer.add_printers(pretty_printer_mongo_extras)
     status_printer.add_printers(pretty_printer_mongo_extras)
     string_data_printer.add_printers(pretty_printer_mongo_extras)
     timestamp_printer.add_printers(pretty_printer_mongo_extras)
     uuid_printer.add_printers(pretty_printer_mongo_extras)
     gdb.printing.register_pretty_printer(gdb.current_objfile(), pretty_printer_mongo_extras)
 
     def initialize_environment(executable: str, /) -> None:
```

### Comparing `gdbmongo-0.8.1/gdbmongo/lock_manager_printer.py` & `gdbmongo-0.9.0/gdbmongo/lock_manager_printer.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 import gdb
 
 from gdbmongo import stdlib_printers, stdlib_xmethods
 from gdbmongo.abseil_printers import (AbslFlatHashMapPrinter, AbslNodeHashMapPrinter,
                                       AbslFlatHashSetPrinter)
 from gdbmongo.decorable_printer import DecorationContainerPrinter
 from gdbmongo.printer_protocol import PrettyPrinterProtocol, SupportsDisplayHint, SupportsToString
+from gdbmongo.static_immortal_printer import StaticImmortalPrinter
 from gdbmongo.string_data_printer import StdStringPrinter
 
 
 def gdb_lookup_value(symbol_name: str, /) -> typing.Optional[gdb.Value]:
     """Return the gdb.Value corresponding to the symbol name given."""
     if (symbol := gdb.lookup_symbol(symbol_name)[0]) is not None:
         return symbol.value()
@@ -349,14 +350,53 @@
             lock_request = lock_request["next"]
 
     def __bool__(self) -> bool:
         """Return True if the linked list isn't empty, and return False otherwise."""
         return self.val["_front"] != 0
 
 
+# We don't have to_string() or children() defined on _ResourceIdFactoryPrinter right now. Until we
+# have a sense of how else we might want to use the ResourceIdFactory in GDB pretty printers, it is
+# probably best to mark the type as being internal to this module.
+class _ResourceIdFactoryPrinter:
+    """Pretty-printer for mongo::Lock::ResourceMutex::ResourceIdFactory."""
+
+    def __init__(self, val: gdb.Value, /) -> None:
+        self.resource_labels = val["labels"]
+        self.val = val
+
+    def lookup_resource_mutex_label(self, res_id: gdb.Value, /) -> str:
+        """Return the name of the mutex."""
+        xmethod_worker = stdlib_xmethods.VectorMethodsMatcher().match(self.resource_labels.type,
+                                                                      "at")
+
+        label = StdStringPrinter(xmethod_worker(self.resource_labels, res_id)).string()
+        return label
+
+    @classmethod
+    def from_global(cls) -> "_ResourceIdFactoryPrinter":
+        """Return a _ResourceIdFactoryPrinter from its global definition."""
+        # The ResourceIdFactory type was moved to be a nested type within mongo::Lock::ResourceMutex
+        # as part of SERVER-70467 in MongoDB 6.3. Previously in MongoDB 6.0, the ResourceIdFactory
+        # type was defined as its own top-level type.
+        # https://github.com/mongodb/mongo/blob/r7.0.0/src/mongo/db/concurrency/d_concurrency.cpp#L77
+        # https://github.com/mongodb/mongo/blob/r6.0.9/src/mongo/db/concurrency/d_concurrency.cpp#L91
+        if (res_id_factory := gdb_lookup_value(
+                # pylint: disable-next=line-too-long
+                "mongo::Lock::ResourceMutex::ResourceIdFactory::_resourceIdFactory()::resourceIdFactory"
+        )) is not None:
+            return cls(StaticImmortalPrinter(res_id_factory).value())
+
+        if (res_id_factory := gdb_lookup_value(
+                "mongo::(anonymous namespace)::ResourceIdFactory::resourceIdFactory")) is not None:
+            return cls(res_id_factory)
+
+        raise ValueError("Failed to locate ResourceIdFactory")
+
+
 # pylint: disable-next=too-few-public-methods
 class ResourceIdPrinter(SupportsToString):
     # pylint: disable=missing-function-docstring
     """Pretty-printer for mongo::ResourceId."""
 
     def __init__(self, val: gdb.Value, /) -> None:
         self.val = val
@@ -368,24 +408,16 @@
             gdb.lookup_type("mongo::ResourceType"))
         self.hash_id = self.full_hash & ((2**64 - 1) >> int(resource_type_bits))
 
     def to_string(self) -> str:
         ret = f"{{{self.full_hash}: {self.resource_type}, {self.hash_id}}}"
 
         if self.resource_type == gdb_lookup_value("mongo::RESOURCE_MUTEX"):
-            res_id_factory = gdb_lookup_value(
-                "mongo::(anonymous namespace)::ResourceIdFactory::resourceIdFactory")
-            assert res_id_factory is not None
-
-            resource_labels = res_id_factory["labels"]
-            xmethod_worker = stdlib_xmethods.VectorMethodsMatcher().match(
-                resource_labels.type, "at")
-
-            label = StdStringPrinter(xmethod_worker(resource_labels,
-                                                    gdb.Value(self.hash_id))).string()
+            res_id_factory = _ResourceIdFactoryPrinter.from_global()
+            label = res_id_factory.lookup_resource_mutex_label(gdb.Value(self.hash_id))
             ret += f", {label}"
 
             if "DatabaseShardingState" == label:
                 # The label for the DatabaseShardingState's ResourceMutex was changed as part of
                 # SERVER-70610 in MongoDB 6.2 where it now embeds the database name in the label.
                 # Previously in MongoDB 6.0, the labels for all DatabaseShardingStates'
                 # ResourceMutexes were the same generic "DatabaseShardingState" string and meant
```

### Comparing `gdbmongo-0.8.1/gdbmongo/objectid_printer.py` & `gdbmongo-0.9.0/gdbmongo/objectid_printer.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/gdbmongo/printer_protocol.py` & `gdbmongo-0.9.0/gdbmongo/printer_protocol.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/gdbmongo/status_printer.py` & `gdbmongo-0.9.0/gdbmongo/status_printer.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/gdbmongo/stdlib_printers.py` & `gdbmongo-0.9.0/gdbmongo/stdlib_printers.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/gdbmongo/stdlib_printers.pyi` & `gdbmongo-0.9.0/gdbmongo/stdlib_printers.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/gdbmongo/stdlib_printers_loader.py` & `gdbmongo-0.9.0/gdbmongo/stdlib_printers_loader.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/gdbmongo/stdlib_xmethods.py` & `gdbmongo-0.9.0/gdbmongo/stdlib_xmethods.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/gdbmongo/stdlib_xmethods.pyi` & `gdbmongo-0.9.0/gdbmongo/stdlib_xmethods.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/gdbmongo/string_data_printer.py` & `gdbmongo-0.9.0/gdbmongo/string_data_printer.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/gdbmongo/thread_name_printer.py` & `gdbmongo-0.9.0/gdbmongo/thread_name_printer.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/gdbmongo/timestamp_printer.py` & `gdbmongo-0.9.0/gdbmongo/timestamp_printer.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/gdbmongo/uuid_printer.py` & `gdbmongo-0.9.0/gdbmongo/uuid_printer.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/gdbmongo.egg-info/PKG-INFO` & `gdbmongo-0.9.0/gdbmongo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdbmongo
-Version: 0.8.1
+Version: 0.9.0
 Summary: GDB pretty printers and commands for debugging the MongoDB Server
 Home-page: https://github.com/visemet/gdb-mongodb-server
 Maintainer: Max Hirschhorn
 Maintainer-email: max.hirschhorn@mongodb.com
 License: Apache License, Version 2.0
 Keywords: mongo,mongodb,gdb
 Platform: linux
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Debuggers
 Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ==================
 gdb-mongodb-server
 ==================
 
 About
@@ -119,14 +120,19 @@
 
     (gdb) python lock_mgr = gdbmongo.LockManagerPrinter.from_global()
     (gdb) python print(lock_mgr.val)
 
 Changelog
 =========
 
+0.9.0 (2023-08-26)
+------------------
+
+* Support dumping LockManager from core dump of MongoDB 7.0.
+
 0.8.1 (2023-03-04)
 ------------------
 
 * Fix two Python exceptions from thread names logic when no program or core dump was loaded.
 * Fix boost::optional pretty printer for scalar types.
 
 0.8.0 (2023-02-04)
```

### Comparing `gdbmongo-0.8.1/gdbmongo.egg-info/SOURCES.txt` & `gdbmongo-0.9.0/gdbmongo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 gdbmongo/date_printer.py
 gdbmongo/decorable_printer.py
 gdbmongo/detect_toolchain.py
 gdbmongo/interaction.py
 gdbmongo/lock_manager_printer.py
 gdbmongo/objectid_printer.py
 gdbmongo/printer_protocol.py
+gdbmongo/static_immortal_printer.py
 gdbmongo/status_printer.py
 gdbmongo/stdlib_printers.py
 gdbmongo/stdlib_printers.pyi
 gdbmongo/stdlib_printers_loader.py
 gdbmongo/stdlib_xmethods.py
 gdbmongo/stdlib_xmethods.pyi
 gdbmongo/string_data_printer.py
```

### Comparing `gdbmongo-0.8.1/pyproject.toml` & `gdbmongo-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/setup.cfg` & `gdbmongo-0.9.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [metadata]
 name = gdbmongo
 description = GDB pretty printers and commands for debugging the MongoDB Server
 long_description = file: README.rst, CHANGELOG.rst
+long_description_content_type = text/x-rst
 url = https://github.com/visemet/gdb-mongodb-server
 maintainer = Max Hirschhorn
 maintainer_email = max.hirschhorn@mongodb.com
 license = Apache License, Version 2.0
 license_files = 
 	LICENSE
 classifiers =
```

### Comparing `gdbmongo-0.8.1/stubs/gdb/__init__.pyi` & `gdbmongo-0.9.0/stubs/gdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/stubs/gdb/_architecture.pyi` & `gdbmongo-0.9.0/stubs/gdb/_architecture.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/stubs/gdb/_basic.pyi` & `gdbmongo-0.9.0/stubs/gdb/_basic.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/stubs/gdb/_errors.pyi` & `gdbmongo-0.9.0/stubs/gdb/_errors.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/stubs/gdb/_frame.pyi` & `gdbmongo-0.9.0/stubs/gdb/_frame.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/stubs/gdb/_inferior.pyi` & `gdbmongo-0.9.0/stubs/gdb/_inferior.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/stubs/gdb/_inferiorthread.pyi` & `gdbmongo-0.9.0/stubs/gdb/_inferiorthread.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/stubs/gdb/_lazy_string.pyi` & `gdbmongo-0.9.0/stubs/gdb/_lazy_string.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/stubs/gdb/_objfile.pyi` & `gdbmongo-0.9.0/stubs/gdb/_objfile.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/stubs/gdb/_progspace.pyi` & `gdbmongo-0.9.0/stubs/gdb/_progspace.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/stubs/gdb/_symbol.pyi` & `gdbmongo-0.9.0/stubs/gdb/_symbol.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/stubs/gdb/_type.pyi` & `gdbmongo-0.9.0/stubs/gdb/_type.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/stubs/gdb/_value.pyi` & `gdbmongo-0.9.0/stubs/gdb/_value.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/stubs/gdb/events.pyi` & `gdbmongo-0.9.0/stubs/gdb/events.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/stubs/gdb/printing.pyi` & `gdbmongo-0.9.0/stubs/gdb/printing.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/stubs/gdb/xmethod.pyi` & `gdbmongo-0.9.0/stubs/gdb/xmethod.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/stubs/pydocstyle/__init__.pyi` & `gdbmongo-0.9.0/stubs/pydocstyle/__init__.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/stubs/pydocstyle/cli.pyi` & `gdbmongo-0.9.0/stubs/pydocstyle/cli.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/stubs/pylint/__init__.pyi` & `gdbmongo-0.9.0/stubs/pylint/__init__.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/stubs/pylint/lint.pyi` & `gdbmongo-0.9.0/stubs/pylint/lint.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/stubs/yapf/__init__.pyi` & `gdbmongo-0.9.0/stubs/yapf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/tests/test_detect_toolchain.py` & `gdbmongo-0.9.0/tests/test_detect_toolchain.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/tests/test_formatting.py` & `gdbmongo-0.9.0/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/tests/test_interaction.py` & `gdbmongo-0.9.0/tests/test_interaction.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/tests/test_linting.py` & `gdbmongo-0.9.0/tests/test_linting.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/tests/test_stdlib_printers.py` & `gdbmongo-0.9.0/tests/test_stdlib_printers.py`

 * *Files identical despite different names*

### Comparing `gdbmongo-0.8.1/tox.ini` & `gdbmongo-0.9.0/tox.ini`

 * *Files identical despite different names*


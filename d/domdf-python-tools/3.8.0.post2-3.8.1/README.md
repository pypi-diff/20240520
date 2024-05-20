# Comparing `tmp/domdf_python_tools-3.8.0.post2.tar.gz` & `tmp/domdf_python_tools-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domdf_python_tools-3.8.0.post2.tar", last modified: Mon Dec 11 16:17:15 2023, max compression
+gzip compressed data, was "domdf_python_tools-3.8.1.tar", last modified: Mon May 20 16:56:09 2024, max compression
```

## Comparing `domdf_python_tools-3.8.0.post2.tar` & `domdf_python_tools-3.8.1.tar`

### file list

```diff
@@ -1,73 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:17:15.118780 domdf_python_tools-3.8.0.post2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8885 2023-12-11 16:17:15.118780 domdf_python_tools-3.8.0.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5659 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/__pkginfo__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:17:15.110781 domdf_python_tools-3.8.0.post2/domdf_python_tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/_is_match.py
--rw-r--r--   0 runner    (1001) docker     (127)    17722 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/bases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:17:15.114781 domdf_python_tools-3.8.0.post2/domdf_python_tools/compat/
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/compat/importlib_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/compat/importlib_metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/compat/importlib_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/compat/importlib_resources.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10858 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/delegators.py
--rw-r--r--   0 runner    (1001) docker     (127)    12333 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/doctools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/getters.py
--rw-r--r--   0 runner    (1001) docker     (127)    75153 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/google-10000-english-no-swears.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/import_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11966 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/iterative.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:17:15.114781 domdf_python_tools-3.8.0.post2/domdf_python_tools/pagesizes/
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/pagesizes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/pagesizes/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8803 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/pagesizes/sizes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8914 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/pagesizes/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/pagesizes/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34600 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     8496 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/pretty_print.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    14454 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/stringlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7372 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17211 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/versions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21784 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools/words.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:17:15.118780 domdf_python_tools-3.8.0.post2/domdf_python_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8885 2023-12-11 16:17:15.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2023-12-11 16:17:15.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 16:17:15.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 16:17:15.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-12-11 16:17:15.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-11 16:17:15.000000 domdf_python_tools-3.8.0.post2/domdf_python_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2023-12-11 16:17:15.118780 domdf_python_tools-3.8.0.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:17:15.118780 domdf_python_tools-3.8.0.post2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_bases.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12800 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_delegators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8969 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_dir_comparator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    12945 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_doctools.py
--rw-r--r--   0 runner    (1001) docker     (127)    10904 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_getters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7169 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_import_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    15576 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_iterative.py
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_namedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    29785 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)    17671 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_paths_stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    26929 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_pretty_print.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    16328 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_stringlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_userlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    14335 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12192 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8447 2023-12-11 16:16:51.000000 domdf_python_tools-3.8.0.post2/tests/test_words.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:56:09.490877 domdf_python_tools-3.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-05-20 16:56:09.490877 domdf_python_tools-3.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/__pkginfo__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:56:09.486877 domdf_python_tools-3.8.1/domdf_python_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/_is_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17722 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/bases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:56:09.490877 domdf_python_tools-3.8.1/domdf_python_tools/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/compat/importlib_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/compat/importlib_metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/compat/importlib_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/compat/importlib_resources.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/delegators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12333 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/doctools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/getters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75153 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/google-10000-english-no-swears.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/import_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11966 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/iterative.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:56:09.490877 domdf_python_tools-3.8.1/domdf_python_tools/pagesizes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/pagesizes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/pagesizes/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8803 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/pagesizes/sizes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/pagesizes/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/pagesizes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8496 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/pretty_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14454 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/stringlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7372 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17211 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21784 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/domdf_python_tools/words.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:56:09.490877 domdf_python_tools-3.8.1/domdf_python_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-05-20 16:56:09.000000 domdf_python_tools-3.8.1/domdf_python_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-20 16:56:09.000000 domdf_python_tools-3.8.1/domdf_python_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:56:09.000000 domdf_python_tools-3.8.1/domdf_python_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:56:09.000000 domdf_python_tools-3.8.1/domdf_python_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-20 16:56:09.000000 domdf_python_tools-3.8.1/domdf_python_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-20 16:56:09.000000 domdf_python_tools-3.8.1/domdf_python_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-20 16:56:09.490877 domdf_python_tools-3.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-20 16:55:46.000000 domdf_python_tools-3.8.1/setup.py
```

### Comparing `domdf_python_tools-3.8.0.post2/LICENSE` & `domdf_python_tools-3.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/PKG-INFO` & `domdf_python_tools-3.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domdf_python_tools
-Version: 3.8.0.post2
+Version: 3.8.1
 Summary: Helpful functions for Python 🐍 🛠️
 Home-page: https://github.com/domdfcoding/domdf_python_tools
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2019-2022 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,24 +48,18 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: importlib-metadata>=3.6.0; python_version < "3.9"
-Requires-Dist: importlib-resources>=3.0.0; python_version < "3.7"
-Requires-Dist: natsort>=7.0.1
-Requires-Dist: typing-extensions>=3.7.4.1
 Provides-Extra: dates
-Requires-Dist: pytz>=2019.1; extra == "dates"
 Provides-Extra: testing
 Provides-Extra: all
-Requires-Dist: pytz>=2019.1; extra == "all"
+License-File: LICENSE
 
 =====================
 domdf_python_tools
 =====================
 
 .. start short_desc
 
@@ -161,23 +155,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/domdf_python_tools
 	:target: https://github.com/domdfcoding/domdf_python_tools/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/domdf_python_tools
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/domdf_python_tools/v3.8.0.post2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/domdf_python_tools/v3.8.1
 	:target: https://github.com/domdfcoding/domdf_python_tools/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/domdf_python_tools
 	:target: https://github.com/domdfcoding/domdf_python_tools/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/domdf_python_tools
 	:target: https://pypi.org/project/domdf_python_tools/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `domdf_python_tools-3.8.0.post2/README.rst` & `domdf_python_tools-3.8.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -96,23 +96,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/domdf_python_tools
 	:target: https://github.com/domdfcoding/domdf_python_tools/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/domdf_python_tools
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/domdf_python_tools/v3.8.0.post2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/domdf_python_tools/v3.8.1
 	:target: https://github.com/domdfcoding/domdf_python_tools/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/domdf_python_tools
 	:target: https://github.com/domdfcoding/domdf_python_tools/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/domdf_python_tools
 	:target: https://pypi.org/project/domdf_python_tools/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/__init__.py` & `domdf_python_tools-3.8.1/domdf_python_tools/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2014-2020 Dominic Davis-Foster"
 __license__: str = "MIT"
-__version__: str = "3.8.0.post2"
+__version__: str = "3.8.1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __docs = False
```

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/_is_match.py` & `domdf_python_tools-3.8.1/domdf_python_tools/_is_match.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/bases.py` & `domdf_python_tools-3.8.1/domdf_python_tools/bases.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/compat/__init__.py` & `domdf_python_tools-3.8.1/domdf_python_tools/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/compat/importlib_metadata.pyi` & `domdf_python_tools-3.8.1/domdf_python_tools/compat/importlib_metadata.pyi`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/compat/importlib_resources.py` & `domdf_python_tools-3.8.1/domdf_python_tools/compat/importlib_resources.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/compat/importlib_resources.pyi` & `domdf_python_tools-3.8.1/domdf_python_tools/compat/importlib_resources.pyi`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/dates.py` & `domdf_python_tools-3.8.1/domdf_python_tools/dates.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/delegators.py` & `domdf_python_tools-3.8.1/domdf_python_tools/delegators.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/doctools.py` & `domdf_python_tools-3.8.1/domdf_python_tools/doctools.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/getters.py` & `domdf_python_tools-3.8.1/domdf_python_tools/getters.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/google-10000-english-no-swears.txt` & `domdf_python_tools-3.8.1/domdf_python_tools/google-10000-english-no-swears.txt`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/import_tools.py` & `domdf_python_tools-3.8.1/domdf_python_tools/import_tools.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/iterative.py` & `domdf_python_tools-3.8.1/domdf_python_tools/iterative.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/pagesizes/__init__.py` & `domdf_python_tools-3.8.1/domdf_python_tools/pagesizes/__init__.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/pagesizes/classes.py` & `domdf_python_tools-3.8.1/domdf_python_tools/pagesizes/classes.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/pagesizes/sizes.py` & `domdf_python_tools-3.8.1/domdf_python_tools/pagesizes/sizes.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/pagesizes/units.py` & `domdf_python_tools-3.8.1/domdf_python_tools/pagesizes/units.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/pagesizes/utils.py` & `domdf_python_tools-3.8.1/domdf_python_tools/pagesizes/utils.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/paths.py` & `domdf_python_tools-3.8.1/domdf_python_tools/paths.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/pretty_print.py` & `domdf_python_tools-3.8.1/domdf_python_tools/pretty_print.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/secrets.py` & `domdf_python_tools-3.8.1/domdf_python_tools/secrets.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/stringlist.py` & `domdf_python_tools-3.8.1/domdf_python_tools/stringlist.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/terminal.py` & `domdf_python_tools-3.8.1/domdf_python_tools/terminal.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/typing.py` & `domdf_python_tools-3.8.1/domdf_python_tools/typing.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/utils.py` & `domdf_python_tools-3.8.1/domdf_python_tools/utils.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/versions.py` & `domdf_python_tools-3.8.1/domdf_python_tools/versions.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools/words.py` & `domdf_python_tools-3.8.1/domdf_python_tools/words.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.8.0.post2/domdf_python_tools.egg-info/PKG-INFO` & `domdf_python_tools-3.8.1/domdf_python_tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domdf-python-tools
-Version: 3.8.0.post2
+Version: 3.8.1
 Summary: Helpful functions for Python 🐍 🛠️
 Home-page: https://github.com/domdfcoding/domdf_python_tools
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2019-2022 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,24 +48,18 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: importlib-metadata>=3.6.0; python_version < "3.9"
-Requires-Dist: importlib-resources>=3.0.0; python_version < "3.7"
-Requires-Dist: natsort>=7.0.1
-Requires-Dist: typing-extensions>=3.7.4.1
 Provides-Extra: dates
-Requires-Dist: pytz>=2019.1; extra == "dates"
 Provides-Extra: testing
 Provides-Extra: all
-Requires-Dist: pytz>=2019.1; extra == "all"
+License-File: LICENSE
 
 =====================
 domdf_python_tools
 =====================
 
 .. start short_desc
 
@@ -161,23 +155,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/domdf_python_tools
 	:target: https://github.com/domdfcoding/domdf_python_tools/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/domdf_python_tools
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/domdf_python_tools/v3.8.0.post2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/domdf_python_tools/v3.8.1
 	:target: https://github.com/domdfcoding/domdf_python_tools/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/domdf_python_tools
 	:target: https://github.com/domdfcoding/domdf_python_tools/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2024
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/domdf_python_tools
 	:target: https://pypi.org/project/domdf_python_tools/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `domdf_python_tools-3.8.0.post2/pyproject.toml` & `domdf_python_tools-3.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = [ "setuptools!=61.*,>=40.6.0", "wheel>=0.34.2",]
+requires = [ "setuptools!=61.*,<=67.1.0,>=40.6.0", "wheel>=0.34.2",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "domdf_python_tools"
-version = "3.8.0.post2"
+version = "3.8.1"
 description = "Helpful functions for Python 🐍 🛠️"
 readme = "README.rst"
 requires-python = ">=3.6"
 keywords = [ "utilities",]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -26,22 +26,21 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 dynamic = [ "dependencies",]
 
+[project.license]
+file = "LICENSE"
+
 [[project.authors]]
 name = "Dominic Davis-Foster"
 email = "dominic@davis-foster.co.uk"
 
-
-[project.license]
-file = "LICENSE"
-
 [project.urls]
 Homepage = "https://github.com/domdfcoding/domdf_python_tools"
 "Issue Tracker" = "https://github.com/domdfcoding/domdf_python_tools/issues"
 "Source Code" = "https://github.com/domdfcoding/domdf_python_tools"
 Documentation = "https://domdf-python-tools.readthedocs.io/en/latest"
 
 [project.optional-dependencies]
@@ -71,29 +70,27 @@
     "sphinxcontrib.toctree_plus",
     "sphinx_toolbox.tweaks.latex_layout",
     "sphinx_toolbox.tweaks.latex_toc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinxcontrib.extras_require",
     "sphinx.ext.todo",
-    "sphinxemoji.sphinxemoji",
     "notfound.extension",
     "sphinx_copybutton",
     "sphinxcontrib.default_values",
     "sphinx_debuginfo",
     "sphinx_licenseinfo",
     "seed_intersphinx_mapping",
     "html_section",
     "sphinx_autofixture",
     "sphinx_highlights",
     "sphinx_toolbox.more_autosummary.column_widths",
     "sphinx_toolbox.latex.succinct_seealso",
     "latex_unicode",
 ]
-sphinxemoji_style = "twemoji"
 gitstamp_fmt = "%d %b %Y"
 templates_path = [ "_templates",]
 html_static_path = [ "_static",]
 source_suffix = ".rst"
 master_doc = "index"
 suppress_warnings = [ "image.nonlocal_uri",]
 pygments_style = "default"
@@ -158,14 +155,24 @@
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.snippet-fmt]
 directives = [ "code-block",]
 
+[tool.snippet-fmt.languages.python]
+reformat = true
+
+[tool.snippet-fmt.languages.TOML]
+reformat = true
+
+[tool.snippet-fmt.languages.ini]
+
+[tool.snippet-fmt.languages.json]
+
 [tool.setuptools]
 zip-safe = false
 include-package-data = true
 platforms = [ "Windows", "macOS", "Linux",]
 
 [tool.dependency-dash."requirements.txt"]
 order = 10
@@ -173,17 +180,7 @@
 [tool.dependency-dash."tests/requirements.txt"]
 order = 20
 include = false
 
 [tool.dependency-dash."doc-source/requirements.txt"]
 order = 30
 include = false
-
-[tool.snippet-fmt.languages.python]
-reformat = true
-
-[tool.snippet-fmt.languages.TOML]
-reformat = true
-
-[tool.snippet-fmt.languages.ini]
-
-[tool.snippet-fmt.languages.json]
```

### Comparing `domdf_python_tools-3.8.0.post2/setup.cfg` & `domdf_python_tools-3.8.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = domdf_python_tools
-version = 3.8.0.post2
+version = 3.8.1
 author = Dominic Davis-Foster
 author_email = dominic@davis-foster.co.uk
 license = MIT License
 keywords = utilities
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 platforms = Windows, macOS, Linux
```

### Comparing `domdf_python_tools-3.8.0.post2/setup.py` & `domdf_python_tools-3.8.1/setup.py`

 * *Files identical despite different names*


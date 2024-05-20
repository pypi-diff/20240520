# Comparing `tmp/enk-0.1.tar.gz` & `tmp/enk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enk-0.1.tar", last modified: Tue Oct 20 18:20:34 2020, max compression
+gzip compressed data, was "enk-0.2.0.tar", last modified: Mon May 20 13:43:30 2024, max compression
```

## Comparing `enk-0.1.tar` & `enk-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,18 @@
--rw-r--r--   0        0        0      294 2020-10-20 18:14:37.700550 enk-0.1/pyproject.toml
--rw-r--r--   0        0        0      169 2020-10-20 18:18:01.105426 enk-0.1/src/enk/__init__.py
--rw-r--r--   0        0        0      839 2020-10-20 18:16:40.381422 enk-0.1/src/enk/console.py
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 enk-0.1/setup.py
--rw-r--r--   0        0        0      183 1970-01-01 00:00:00.000000 enk-0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:43:30.128845 enk-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-20 13:43:26.000000 enk-0.2.0/DESCRIPTION.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-20 13:43:26.000000 enk-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-20 13:43:30.128845 enk-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-20 13:43:26.000000 enk-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:43:30.124845 enk-0.2.0/enk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:43:26.000000 enk-0.2.0/enk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-20 13:43:26.000000 enk-0.2.0/enk/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-20 13:43:26.000000 enk-0.2.0/enk/filegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-20 13:43:26.000000 enk-0.2.0/enk/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:43:30.128845 enk-0.2.0/enk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-20 13:43:30.000000 enk-0.2.0/enk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-20 13:43:30.000000 enk-0.2.0/enk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:43:30.000000 enk-0.2.0/enk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 13:43:30.000000 enk-0.2.0/enk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-20 13:43:30.000000 enk-0.2.0/enk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-20 13:43:30.128845 enk-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-05-20 13:43:26.000000 enk-0.2.0/setup.py
```


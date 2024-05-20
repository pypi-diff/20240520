# Comparing `tmp/italia-0.1.0.tar.gz` & `tmp/italia-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "italia-0.1.0.tar", last modified: Tue Apr 30 13:37:18 2024, max compression
+gzip compressed data, was "italia-0.2.0.tar", last modified: Mon May 20 18:37:47 2024, max compression
```

## Comparing `italia-0.1.0.tar` & `italia-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,9 @@
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-30 13:37:18.093743 italia-0.1.0/
--rw-r--r--   0 marco     (1000) marco     (1000)      199 2024-04-30 13:37:18.093743 italia-0.1.0/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)        9 2024-04-30 13:36:29.000000 italia-0.1.0/README.md
--rw-r--r--   0 marco     (1000) marco     (1000)      261 2024-04-30 13:37:07.000000 italia-0.1.0/pyproject.toml
--rw-r--r--   0 marco     (1000) marco     (1000)       38 2024-04-30 13:37:18.093743 italia-0.1.0/setup.cfg
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-30 13:37:18.093743 italia-0.1.0/src/
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-30 13:37:18.093743 italia-0.1.0/src/italia/
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-04-30 13:36:29.000000 italia-0.1.0/src/italia/__init__.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-30 13:37:18.093743 italia-0.1.0/src/italia.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)      199 2024-04-30 13:37:18.000000 italia-0.1.0/src/italia.egg-info/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)      183 2024-04-30 13:37:18.000000 italia-0.1.0/src/italia.egg-info/SOURCES.txt
--rw-r--r--   0 marco     (1000) marco     (1000)        1 2024-04-30 13:37:18.000000 italia-0.1.0/src/italia.egg-info/dependency_links.txt
--rw-r--r--   0 marco     (1000) marco     (1000)        7 2024-04-30 13:37:18.000000 italia-0.1.0/src/italia.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1070 2024-05-20 18:37:33.568165 italia-0.2.0/LICENCE
+-rw-r--r--   0        0        0     2663 2024-05-20 18:37:33.568165 italia-0.2.0/README.md
+-rw-r--r--   0        0        0       56 2024-05-20 18:37:33.568165 italia-0.2.0/italia/__init__.py
+-rw-r--r--   0        0        0     1883 2024-05-20 18:37:33.568165 italia-0.2.0/italia/story.py
+-rw-r--r--   0        0        0      607 2024-05-20 18:37:33.568165 italia-0.2.0/italia/team.py
+-rw-r--r--   0        0        0      532 2024-05-20 18:37:47.936270 italia-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-20 18:37:33.568165 italia-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      203 2024-05-20 18:37:33.568165 italia-0.2.0/tests/test_italia.py
+-rw-r--r--   0        0        0     2916 1970-01-01 00:00:00.000000 italia-0.2.0/PKG-INFO
```


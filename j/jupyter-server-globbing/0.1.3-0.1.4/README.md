# Comparing `tmp/jupyter_server_globbing-0.1.3.tar.gz` & `tmp/jupyter_server_globbing-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_server_globbing-0.1.3.tar", last modified: Mon May 20 14:20:29 2024, max compression
+gzip compressed data, was "jupyter_server_globbing-0.1.4.tar", last modified: Mon May 20 14:33:25 2024, max compression
```

## Comparing `jupyter_server_globbing-0.1.3.tar` & `jupyter_server_globbing-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-20 14:20:29.113826 jupyter_server_globbing-0.1.3/
--rw-r--r--   0 tparment (15010) diana    (200036)       67 2024-05-20 14:20:29.113229 jupyter_server_globbing-0.1.3/PKG-INFO
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-20 14:20:29.109885 jupyter_server_globbing-0.1.3/globbing/
--rw-r--r--   0 tparment (15010) diana    (200036)      380 2024-05-20 14:15:24.000000 jupyter_server_globbing-0.1.3/globbing/__init__.py
--rw-r--r--   0 tparment (15010) diana    (200036)      523 2024-05-20 13:55:21.000000 jupyter_server_globbing-0.1.3/globbing/handlers.py
--rw-r--r--   0 tparment (15010) diana    (200036)       22 2024-05-20 14:19:54.000000 jupyter_server_globbing-0.1.3/globbing/version.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-20 14:20:29.107917 jupyter_server_globbing-0.1.3/jupyter-config/
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-20 14:20:29.110353 jupyter_server_globbing-0.1.3/jupyter-config/jupyter_server_config.d/
--rw-r--r--   0 tparment (15010) diana    (200036)      101 2024-05-20 13:09:27.000000 jupyter_server_globbing-0.1.3/jupyter-config/jupyter_server_config.d/globbing.json
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-20 14:20:29.112671 jupyter_server_globbing-0.1.3/jupyter_server_globbing.egg-info/
--rw-r--r--   0 tparment (15010) diana    (200036)       67 2024-05-20 14:20:29.000000 jupyter_server_globbing-0.1.3/jupyter_server_globbing.egg-info/PKG-INFO
--rw-r--r--   0 tparment (15010) diana    (200036)      311 2024-05-20 14:20:29.000000 jupyter_server_globbing-0.1.3/jupyter_server_globbing.egg-info/SOURCES.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        1 2024-05-20 14:20:29.000000 jupyter_server_globbing-0.1.3/jupyter_server_globbing.egg-info/dependency_links.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        9 2024-05-20 14:20:29.000000 jupyter_server_globbing-0.1.3/jupyter_server_globbing.egg-info/top_level.txt
--rw-r--r--   0 tparment (15010) diana    (200036)       38 2024-05-20 14:20:29.113989 jupyter_server_globbing-0.1.3/setup.cfg
--rwxr-xr-x   0 tparment (15010) diana    (200036)      364 2024-05-20 14:19:34.000000 jupyter_server_globbing-0.1.3/setup.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-20 14:33:25.946880 jupyter_server_globbing-0.1.4/
+-rw-r--r--   0 tparment (15010) diana    (200036)      143 2024-05-20 14:33:25.946298 jupyter_server_globbing-0.1.4/PKG-INFO
+-rw-r--r--   0 tparment (15010) diana    (200036)      640 2024-05-20 14:30:23.000000 jupyter_server_globbing-0.1.4/README.md
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-20 14:33:25.942453 jupyter_server_globbing-0.1.4/globbing/
+-rw-r--r--   0 tparment (15010) diana    (200036)      380 2024-05-20 14:15:24.000000 jupyter_server_globbing-0.1.4/globbing/__init__.py
+-rw-r--r--   0 tparment (15010) diana    (200036)      852 2024-05-20 14:32:43.000000 jupyter_server_globbing-0.1.4/globbing/handlers.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       22 2024-05-20 14:31:14.000000 jupyter_server_globbing-0.1.4/globbing/version.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-20 14:33:25.939784 jupyter_server_globbing-0.1.4/jupyter-config/
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-20 14:33:25.942927 jupyter_server_globbing-0.1.4/jupyter-config/jupyter_server_config.d/
+-rw-r--r--   0 tparment (15010) diana    (200036)      101 2024-05-20 13:09:27.000000 jupyter_server_globbing-0.1.4/jupyter-config/jupyter_server_config.d/globbing.json
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-20 14:33:25.945708 jupyter_server_globbing-0.1.4/jupyter_server_globbing.egg-info/
+-rw-r--r--   0 tparment (15010) diana    (200036)      143 2024-05-20 14:33:25.000000 jupyter_server_globbing-0.1.4/jupyter_server_globbing.egg-info/PKG-INFO
+-rw-r--r--   0 tparment (15010) diana    (200036)      321 2024-05-20 14:33:25.000000 jupyter_server_globbing-0.1.4/jupyter_server_globbing.egg-info/SOURCES.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        1 2024-05-20 14:33:25.000000 jupyter_server_globbing-0.1.4/jupyter_server_globbing.egg-info/dependency_links.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        9 2024-05-20 14:33:25.000000 jupyter_server_globbing-0.1.4/jupyter_server_globbing.egg-info/top_level.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)       38 2024-05-20 14:33:25.947009 jupyter_server_globbing-0.1.4/setup.cfg
+-rwxr-xr-x   0 tparment (15010) diana    (200036)      442 2024-05-20 14:30:56.000000 jupyter_server_globbing-0.1.4/setup.py
```


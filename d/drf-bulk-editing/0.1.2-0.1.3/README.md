# Comparing `tmp/drf-bulk-editing-0.1.2.tar.gz` & `tmp/drf-bulk-editing-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-bulk-editing-0.1.2.tar", last modified: Mon May 20 12:05:11 2024, max compression
+gzip compressed data, was "drf-bulk-editing-0.1.3.tar", last modified: Mon May 20 12:10:16 2024, max compression
```

## Comparing `drf-bulk-editing-0.1.2.tar` & `drf-bulk-editing-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2024-05-20 12:05:11.929040 drf-bulk-editing-0.1.2/
--rw-r--r--   0 brian     (1000) brian     (1000)      437 2024-05-20 12:05:11.929040 drf-bulk-editing-0.1.2/PKG-INFO
--rw-r--r--   0 brian     (1000) brian     (1000)      263 2024-05-20 11:56:36.000000 drf-bulk-editing-0.1.2/README.md
-drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2024-05-20 12:05:11.919040 drf-bulk-editing-0.1.2/drf-bulk-editing/
--rw-r--r--   0 brian     (1000) brian     (1000)       57 2024-05-20 11:53:45.000000 drf-bulk-editing-0.1.2/drf-bulk-editing/main.py
-drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2024-05-20 12:05:11.929040 drf-bulk-editing-0.1.2/drf_bulk_editing.egg-info/
--rw-r--r--   0 brian     (1000) brian     (1000)      437 2024-05-20 12:05:11.000000 drf-bulk-editing-0.1.2/drf_bulk_editing.egg-info/PKG-INFO
--rw-r--r--   0 brian     (1000) brian     (1000)      246 2024-05-20 12:05:11.000000 drf-bulk-editing-0.1.2/drf_bulk_editing.egg-info/SOURCES.txt
--rw-r--r--   0 brian     (1000) brian     (1000)        1 2024-05-20 12:05:11.000000 drf-bulk-editing-0.1.2/drf_bulk_editing.egg-info/dependency_links.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       50 2024-05-20 12:05:11.000000 drf-bulk-editing-0.1.2/drf_bulk_editing.egg-info/entry_points.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       17 2024-05-20 12:05:11.000000 drf-bulk-editing-0.1.2/drf_bulk_editing.egg-info/top_level.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       38 2024-05-20 12:05:11.929040 drf-bulk-editing-0.1.2/setup.cfg
--rw-r--r--   0 brian     (1000) brian     (1000)      490 2024-05-20 12:04:59.000000 drf-bulk-editing-0.1.2/setup.py
+drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2024-05-20 12:10:16.278991 drf-bulk-editing-0.1.3/
+-rw-r--r--   0 brian     (1000) brian     (1000)      444 2024-05-20 12:10:16.278991 drf-bulk-editing-0.1.3/PKG-INFO
+-rw-r--r--   0 brian     (1000) brian     (1000)      270 2024-05-20 12:09:34.000000 drf-bulk-editing-0.1.3/README.md
+drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2024-05-20 12:10:16.278991 drf-bulk-editing-0.1.3/drf-bulk-editing/
+-rw-r--r--   0 brian     (1000) brian     (1000)       57 2024-05-20 11:53:45.000000 drf-bulk-editing-0.1.3/drf-bulk-editing/main.py
+drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2024-05-20 12:10:16.278991 drf-bulk-editing-0.1.3/drf_bulk_editing.egg-info/
+-rw-r--r--   0 brian     (1000) brian     (1000)      444 2024-05-20 12:10:16.000000 drf-bulk-editing-0.1.3/drf_bulk_editing.egg-info/PKG-INFO
+-rw-r--r--   0 brian     (1000) brian     (1000)      246 2024-05-20 12:10:16.000000 drf-bulk-editing-0.1.3/drf_bulk_editing.egg-info/SOURCES.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)        1 2024-05-20 12:10:16.000000 drf-bulk-editing-0.1.3/drf_bulk_editing.egg-info/dependency_links.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)       50 2024-05-20 12:10:16.000000 drf-bulk-editing-0.1.3/drf_bulk_editing.egg-info/entry_points.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)       17 2024-05-20 12:10:16.000000 drf-bulk-editing-0.1.3/drf_bulk_editing.egg-info/top_level.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)       38 2024-05-20 12:10:16.278991 drf-bulk-editing-0.1.3/setup.cfg
+-rw-r--r--   0 brian     (1000) brian     (1000)      490 2024-05-20 12:10:13.000000 drf-bulk-editing-0.1.3/setup.py
```


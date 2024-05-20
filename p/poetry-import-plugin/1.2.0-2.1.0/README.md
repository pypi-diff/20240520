# Comparing `tmp/poetry_import_plugin-1.2.0.tar.gz` & `tmp/poetry_import_plugin-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_import_plugin-1.2.0.tar", max compression
+gzip compressed data, was "poetry_import_plugin-2.1.0.tar", max compression
```

## Comparing `poetry_import_plugin-1.2.0.tar` & `poetry_import_plugin-2.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-05-02 18:09:07.309363 poetry_import_plugin-1.2.0/LICENSE
--rw-r--r--   0        0        0      817 2024-05-13 09:09:13.849939 poetry_import_plugin-1.2.0/README.md
--rw-r--r--   0        0        0     1188 2024-05-13 09:17:33.081034 poetry_import_plugin-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      557 2024-05-13 09:09:13.850450 poetry_import_plugin-1.2.0/req2toml/__init__.py
--rw-r--r--   0        0        0     2445 2024-05-13 09:09:13.850513 poetry_import_plugin-1.2.0/req2toml/console.py
--rw-r--r--   0        0        0     5997 2024-05-13 09:09:13.850595 poetry_import_plugin-1.2.0/req2toml/utils.py
--rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 poetry_import_plugin-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-20 13:45:56.845976 poetry_import_plugin-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3034 2024-05-20 13:45:56.845976 poetry_import_plugin-2.1.0/README.md
+-rw-r--r--   0        0        0     1241 2024-05-20 13:45:56.929977 poetry_import_plugin-2.1.0/poetry_import/__init__.py
+-rw-r--r--   0        0        0     2077 2024-05-20 13:45:56.929977 poetry_import_plugin-2.1.0/poetry_import/backport.py
+-rw-r--r--   0        0        0    15218 2024-05-20 13:45:56.929977 poetry_import_plugin-2.1.0/poetry_import/command.py
+-rw-r--r--   0        0        0     4115 2024-05-20 13:46:27.550040 poetry_import_plugin-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4033 1970-01-01 00:00:00.000000 poetry_import_plugin-2.1.0/PKG-INFO
```

### Comparing `poetry_import_plugin-1.2.0/LICENSE` & `poetry_import_plugin-2.1.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
                                  Apache License
-                           Version 2.0, January 2004
+                           Version 2.0, January 2024
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
 
       "License" shall mean the terms and conditions for use, reproduction,
```


# Comparing `tmp/jrpystan-1.1.1.tar.gz` & `tmp/jrpystan-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jrpystan-1.1.1.tar", max compression
+gzip compressed data, was "jrpystan-1.1.2.tar", max compression
```

## Comparing `jrpystan-1.1.1.tar` & `jrpystan-1.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      123 2023-11-12 15:58:36.271813 jrpystan-1.1.1/jrpystan/__init__.py
--rw-r--r--   0        0        0       22 2023-11-13 09:29:08.011891 jrpystan-1.1.1/jrpystan/__version__.py
--rw-r--r--   0        0        0     1969 2023-11-12 15:58:36.275813 jrpystan-1.1.1/jrpystan/data/api.zip
--rw-r--r--   0        0        0     1012 2023-11-12 15:58:36.275813 jrpystan-1.1.1/jrpystan/data/centipedes.zip
--rw-r--r--   0        0        0     1059 2023-11-12 15:58:36.275813 jrpystan-1.1.1/jrpystan/data/faithful.zip
--rw-r--r--   0        0        0    14130 2023-11-12 15:58:36.275813 jrpystan-1.1.1/jrpystan/data/housing.zip
--rw-r--r--   0        0        0     1576 2023-11-12 15:58:36.275813 jrpystan-1.1.1/jrpystan/data/oxboys.zip
--rw-r--r--   0        0        0      315 2023-11-12 15:58:36.271813 jrpystan-1.1.1/jrpystan/data.py
--rw-r--r--   0        0        0     1068 2023-11-12 15:58:36.275813 jrpystan-1.1.1/jrpystan/vignettes.py
--rw-r--r--   0        0        0      420 2023-11-13 09:29:08.011891 jrpystan-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 jrpystan-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      123 2024-05-20 11:25:35.325030 jrpystan-1.1.2/jrpystan/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-20 11:25:35.325030 jrpystan-1.1.2/jrpystan/__version__.py
+-rw-r--r--   0        0        0     1969 2024-05-20 11:25:35.325030 jrpystan-1.1.2/jrpystan/data/api.zip
+-rw-r--r--   0        0        0     1012 2024-05-20 11:25:35.325030 jrpystan-1.1.2/jrpystan/data/centipedes.zip
+-rw-r--r--   0        0        0     1059 2024-05-20 11:25:35.325030 jrpystan-1.1.2/jrpystan/data/faithful.zip
+-rw-r--r--   0        0        0    14130 2024-05-20 11:25:35.325030 jrpystan-1.1.2/jrpystan/data/housing.zip
+-rw-r--r--   0        0        0     1576 2024-05-20 11:25:35.325030 jrpystan-1.1.2/jrpystan/data/oxboys.zip
+-rw-r--r--   0        0        0      315 2024-05-20 11:25:35.325030 jrpystan-1.1.2/jrpystan/data.py
+-rw-r--r--   0        0        0     1068 2024-05-20 11:25:35.325030 jrpystan-1.1.2/jrpystan/vignettes.py
+-rw-r--r--   0        0        0      421 2024-05-20 11:25:35.325030 jrpystan-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      615 1970-01-01 00:00:00.000000 jrpystan-1.1.2/PKG-INFO
```

### Comparing `jrpystan-1.1.1/jrpystan/data/api.zip` & `jrpystan-1.1.2/jrpystan/data/api.zip`

 * *Files identical despite different names*

### Comparing `jrpystan-1.1.1/jrpystan/data/centipedes.zip` & `jrpystan-1.1.2/jrpystan/data/centipedes.zip`

 * *Files identical despite different names*

### Comparing `jrpystan-1.1.1/jrpystan/data/faithful.zip` & `jrpystan-1.1.2/jrpystan/data/faithful.zip`

 * *Files identical despite different names*

### Comparing `jrpystan-1.1.1/jrpystan/data/housing.zip` & `jrpystan-1.1.2/jrpystan/data/housing.zip`

 * *Files identical despite different names*

### Comparing `jrpystan-1.1.1/jrpystan/data/oxboys.zip` & `jrpystan-1.1.2/jrpystan/data/oxboys.zip`

 * *Files identical despite different names*

### Comparing `jrpystan-1.1.1/jrpystan/vignettes.py` & `jrpystan-1.1.2/jrpystan/vignettes.py`

 * *Files identical despite different names*


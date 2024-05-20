# Comparing `tmp/libcsv-1.0.0.tar.gz` & `tmp/libcsv-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libcsv-1.0.0.tar", last modified: Mon May 20 19:34:53 2024, max compression
+gzip compressed data, was "libcsv-1.0.1.tar", last modified: Mon May 20 19:38:16 2024, max compression
```

## Comparing `libcsv-1.0.0.tar` & `libcsv-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 marko2155   (501) staff       (20)        0 2024-05-20 19:34:53.866616 libcsv-1.0.0/
--rw-r--r--   0 marko2155   (501) staff       (20)      224 2024-05-20 19:34:53.866285 libcsv-1.0.0/PKG-INFO
-drwxr-xr-x   0 marko2155   (501) staff       (20)        0 2024-05-20 19:34:53.864948 libcsv-1.0.0/libcsv/
--rw-r--r--   0 marko2155   (501) staff       (20)     1599 2024-05-20 19:33:45.000000 libcsv-1.0.0/libcsv/__init__.py
-drwxr-xr-x   0 marko2155   (501) staff       (20)        0 2024-05-20 19:34:53.865902 libcsv-1.0.0/libcsv.egg-info/
--rw-r--r--   0 marko2155   (501) staff       (20)      224 2024-05-20 19:34:53.000000 libcsv-1.0.0/libcsv.egg-info/PKG-INFO
--rw-r--r--   0 marko2155   (501) staff       (20)      147 2024-05-20 19:34:53.000000 libcsv-1.0.0/libcsv.egg-info/SOURCES.txt
--rw-r--r--   0 marko2155   (501) staff       (20)        1 2024-05-20 19:34:53.000000 libcsv-1.0.0/libcsv.egg-info/dependency_links.txt
--rw-r--r--   0 marko2155   (501) staff       (20)        7 2024-05-20 19:34:53.000000 libcsv-1.0.0/libcsv.egg-info/top_level.txt
--rw-r--r--   0 marko2155   (501) staff       (20)       38 2024-05-20 19:34:53.866848 libcsv-1.0.0/setup.cfg
--rw-r--r--   0 marko2155   (501) staff       (20)      314 2024-05-17 11:07:16.000000 libcsv-1.0.0/setup.py
+drwxr-xr-x   0 marko2155   (501) staff       (20)        0 2024-05-20 19:38:16.664955 libcsv-1.0.1/
+-rw-r--r--   0 marko2155   (501) staff       (20)      173 2024-05-20 19:38:16.664697 libcsv-1.0.1/PKG-INFO
+-rw-r--r--   0 marko2155   (501) staff       (20)      173 2024-05-20 19:37:54.000000 libcsv-1.0.1/README.md
+drwxr-xr-x   0 marko2155   (501) staff       (20)        0 2024-05-20 19:38:16.663448 libcsv-1.0.1/libcsv/
+-rw-r--r--   0 marko2155   (501) staff       (20)     1599 2024-05-20 19:33:45.000000 libcsv-1.0.1/libcsv/__init__.py
+drwxr-xr-x   0 marko2155   (501) staff       (20)        0 2024-05-20 19:38:16.664455 libcsv-1.0.1/libcsv.egg-info/
+-rw-r--r--   0 marko2155   (501) staff       (20)      173 2024-05-20 19:38:16.000000 libcsv-1.0.1/libcsv.egg-info/PKG-INFO
+-rw-r--r--   0 marko2155   (501) staff       (20)      157 2024-05-20 19:38:16.000000 libcsv-1.0.1/libcsv.egg-info/SOURCES.txt
+-rw-r--r--   0 marko2155   (501) staff       (20)        1 2024-05-20 19:38:16.000000 libcsv-1.0.1/libcsv.egg-info/dependency_links.txt
+-rw-r--r--   0 marko2155   (501) staff       (20)        7 2024-05-20 19:38:16.000000 libcsv-1.0.1/libcsv.egg-info/top_level.txt
+-rw-r--r--   0 marko2155   (501) staff       (20)       38 2024-05-20 19:38:16.665012 libcsv-1.0.1/setup.cfg
+-rw-r--r--   0 marko2155   (501) staff       (20)      263 2024-05-20 19:38:15.000000 libcsv-1.0.1/setup.py
```

### Comparing `libcsv-1.0.0/libcsv/__init__.py` & `libcsv-1.0.1/libcsv/__init__.py`

 * *Files identical despite different names*


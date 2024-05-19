# Comparing `tmp/roofai-4.13.1.tar.gz` & `tmp/roofai-4.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roofai-4.13.1.tar", last modified: Sun May 19 23:01:24 2024, max compression
+gzip compressed data, was "roofai-4.14.1.tar", last modified: Sun May 19 23:02:38 2024, max compression
```

## Comparing `roofai-4.13.1.tar` & `roofai-4.14.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 23:01:24.130496 roofai-4.13.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-10-03 04:10:45.000000 roofai-4.13.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)      144 2024-05-19 23:01:24.129995 roofai-4.13.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     3137 2024-04-23 03:27:00.000000 roofai-4.13.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 23:01:24.126788 roofai-4.13.1/roofAI/
--rw-r--r--   0 kamangir   (502) staff       (20)      106 2024-05-19 23:01:19.000000 roofai-4.13.1/roofAI/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      751 2024-03-04 07:11:52.000000 roofai-4.13.1/roofAI/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       87 2024-03-24 00:16:41.000000 roofai-4.13.1/roofAI/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-10-03 04:10:45.000000 roofai-4.13.1/roofAI/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 23:01:24.129035 roofai-4.13.1/roofAI.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)      144 2024-05-19 23:01:24.000000 roofai-4.13.1/roofAI.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      216 2024-05-19 23:01:24.000000 roofai-4.13.1/roofAI.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-19 23:01:24.000000 roofai-4.13.1/roofAI.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        7 2024-05-19 23:01:24.000000 roofai-4.13.1/roofAI.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-19 23:01:24.130577 roofai-4.13.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      205 2024-03-24 01:15:02.000000 roofai-4.13.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 23:02:38.130900 roofai-4.14.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-10-03 04:10:45.000000 roofai-4.14.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)     3616 2024-05-19 23:02:38.130466 roofai-4.14.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     3137 2024-04-23 03:27:00.000000 roofai-4.14.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 23:02:38.127770 roofai-4.14.1/roofAI/
+-rw-r--r--   0 kamangir   (502) staff       (20)      106 2024-05-19 23:02:33.000000 roofai-4.14.1/roofAI/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      751 2024-03-04 07:11:52.000000 roofai-4.14.1/roofAI/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       87 2024-03-24 00:16:41.000000 roofai-4.14.1/roofAI/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-10-03 04:10:45.000000 roofai-4.14.1/roofAI/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 23:02:38.130047 roofai-4.14.1/roofAI.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     3616 2024-05-19 23:02:38.000000 roofai-4.14.1/roofAI.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      216 2024-05-19 23:02:38.000000 roofai-4.14.1/roofAI.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-19 23:02:38.000000 roofai-4.14.1/roofAI.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        7 2024-05-19 23:02:38.000000 roofai-4.14.1/roofAI.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-19 23:02:38.130978 roofai-4.14.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      493 2024-05-19 23:02:29.000000 roofai-4.14.1/setup.py
```

### Comparing `roofai-4.13.1/LICENSE` & `roofai-4.14.1/LICENSE`

 * *Files identical despite different names*

### Comparing `roofai-4.13.1/README.md` & `roofai-4.14.1/README.md`

 * *Files identical despite different names*

### Comparing `roofai-4.13.1/roofAI/__main__.py` & `roofai-4.14.1/roofAI/__main__.py`

 * *Files identical despite different names*


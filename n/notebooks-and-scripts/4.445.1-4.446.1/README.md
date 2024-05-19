# Comparing `tmp/notebooks_and_scripts-4.445.1.tar.gz` & `tmp/notebooks_and_scripts-4.446.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notebooks_and_scripts-4.445.1.tar", last modified: Sun May 19 22:55:59 2024, max compression
+gzip compressed data, was "notebooks_and_scripts-4.446.1.tar", last modified: Sun May 19 22:56:39 2024, max compression
```

## Comparing `notebooks_and_scripts-4.445.1.tar` & `notebooks_and_scripts-4.446.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:55:59.615355 notebooks_and_scripts-4.445.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.445.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)      191 2024-05-19 22:55:59.614795 notebooks_and_scripts-4.445.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     4193 2024-05-08 05:19:48.000000 notebooks_and_scripts-4.445.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:55:59.611024 notebooks_and_scripts-4.445.1/notebooks_and_scripts/
--rw-r--r--   0 kamangir   (502) staff       (20)      153 2024-05-19 22:55:54.000000 notebooks_and_scripts-4.445.1/notebooks_and_scripts/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      898 2024-04-27 03:49:23.000000 notebooks_and_scripts-4.445.1/notebooks_and_scripts/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      279 2024-05-08 01:33:41.000000 notebooks_and_scripts-4.445.1/notebooks_and_scripts/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      443 2024-05-08 01:33:52.000000 notebooks_and_scripts-4.445.1/notebooks_and_scripts/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)      102 2024-03-24 00:15:57.000000 notebooks_and_scripts-4.445.1/notebooks_and_scripts/logger.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:55:59.613263 notebooks_and_scripts-4.445.1/notebooks_and_scripts/sagemaker/
--rw-r--r--   0 kamangir   (502) staff       (20)      365 2024-03-04 07:47:37.000000 notebooks_and_scripts-4.445.1/notebooks_and_scripts/sagemaker/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.445.1/notebooks_and_scripts/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:55:59.614095 notebooks_and_scripts-4.445.1/notebooks_and_scripts.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)      191 2024-05-19 22:55:59.000000 notebooks_and_scripts-4.445.1/notebooks_and_scripts.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      442 2024-05-19 22:55:59.000000 notebooks_and_scripts-4.445.1/notebooks_and_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-19 22:55:59.000000 notebooks_and_scripts-4.445.1/notebooks_and_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       22 2024-05-19 22:55:59.000000 notebooks_and_scripts-4.445.1/notebooks_and_scripts.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-19 22:55:59.615445 notebooks_and_scripts-4.445.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      537 2024-05-19 22:55:13.000000 notebooks_and_scripts-4.445.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:56:39.556861 notebooks_and_scripts-4.446.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.446.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)     5085 2024-05-19 22:56:39.556091 notebooks_and_scripts-4.446.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     4193 2024-05-08 05:19:48.000000 notebooks_and_scripts-4.446.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:56:39.552750 notebooks_and_scripts-4.446.1/notebooks_and_scripts/
+-rw-r--r--   0 kamangir   (502) staff       (20)      153 2024-05-19 22:56:35.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      898 2024-04-27 03:49:23.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      279 2024-05-08 01:33:41.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      443 2024-05-08 01:33:52.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      102 2024-03-24 00:15:57.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts/logger.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:56:39.554799 notebooks_and_scripts-4.446.1/notebooks_and_scripts/sagemaker/
+-rw-r--r--   0 kamangir   (502) staff       (20)      365 2024-03-04 07:47:37.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts/sagemaker/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:56:39.555468 notebooks_and_scripts-4.446.1/notebooks_and_scripts.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     5085 2024-05-19 22:56:39.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      442 2024-05-19 22:56:39.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-19 22:56:39.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       22 2024-05-19 22:56:39.000000 notebooks_and_scripts-4.446.1/notebooks_and_scripts.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-19 22:56:39.557377 notebooks_and_scripts-4.446.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      627 2024-05-19 22:56:26.000000 notebooks_and_scripts-4.446.1/setup.py
```

### Comparing `notebooks_and_scripts-4.445.1/LICENSE` & `notebooks_and_scripts-4.446.1/LICENSE`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.445.1/README.md` & `notebooks_and_scripts-4.446.1/README.md`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.445.1/notebooks_and_scripts/__main__.py` & `notebooks_and_scripts-4.446.1/notebooks_and_scripts/__main__.py`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.445.1/setup.py` & `notebooks_and_scripts-4.446.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     )
 
 setup(
     name=NAME,
     author="arash@kamangir.net",
     version=VERSION,
     description=DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     packages=[
         NAME,
         f"{NAME}.sagemaker",
     ],
     package_data={
         NAME: ["config.env"],
     },
```


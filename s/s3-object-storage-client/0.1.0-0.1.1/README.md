# Comparing `tmp/s3_object_storage_client-0.1.0.tar.gz` & `tmp/s3_object_storage_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/s3_object_storage_client-0.1.0.tar", last modified: Mon May 20 08:35:36 2024, max compression
+gzip compressed data, was "dist/s3_object_storage_client-0.1.1.tar", last modified: Mon May 20 10:20:23 2024, max compression
```

## Comparing `s3_object_storage_client-0.1.0.tar` & `s3_object_storage_client-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lirui      (501) staff       (20)        0 2024-05-20 08:35:36.000000 s3_object_storage_client-0.1.0/
--rw-r--r--   0 lirui      (501) staff       (20)     1086 2022-07-15 07:21:28.000000 s3_object_storage_client-0.1.0/LICENSE
--rw-r--r--   0 lirui      (501) staff       (20)      304 2024-05-20 08:35:36.000000 s3_object_storage_client-0.1.0/PKG-INFO
--rw-r--r--   0 lirui      (501) staff       (20)        0 2022-10-25 02:05:30.000000 s3_object_storage_client-0.1.0/README.md
-drwxr-xr-x   0 lirui      (501) staff       (20)        0 2024-05-20 08:35:36.000000 s3_object_storage_client-0.1.0/pyCeph/
--rw-r--r--   0 lirui      (501) staff       (20)       36 2022-07-15 09:06:50.000000 s3_object_storage_client-0.1.0/pyCeph/__init__.py
--rw-r--r--   0 lirui      (501) staff       (20)     1190 2022-07-15 09:07:05.000000 s3_object_storage_client-0.1.0/pyCeph/aios3.py
--rw-r--r--   0 lirui      (501) staff       (20)      486 2022-07-14 07:21:24.000000 s3_object_storage_client-0.1.0/pyCeph/crypto.py
--rw-r--r--   0 lirui      (501) staff       (20)      979 2022-07-12 07:08:04.000000 s3_object_storage_client-0.1.0/pyCeph/log.py
--rw-r--r--   0 lirui      (501) staff       (20)     4241 2024-05-20 08:12:31.000000 s3_object_storage_client-0.1.0/pyCeph/s3.py
--rw-r--r--   0 lirui      (501) staff       (20)      645 2022-07-15 07:19:33.000000 s3_object_storage_client-0.1.0/pyproject.toml
-drwxr-xr-x   0 lirui      (501) staff       (20)        0 2024-05-20 08:35:36.000000 s3_object_storage_client-0.1.0/s3_object_storage_client.egg-info/
--rw-r--r--   0 lirui      (501) staff       (20)      304 2024-05-20 08:35:35.000000 s3_object_storage_client-0.1.0/s3_object_storage_client.egg-info/PKG-INFO
--rw-r--r--   0 lirui      (501) staff       (20)      359 2024-05-20 08:35:36.000000 s3_object_storage_client-0.1.0/s3_object_storage_client.egg-info/SOURCES.txt
--rw-r--r--   0 lirui      (501) staff       (20)        1 2024-05-20 08:35:35.000000 s3_object_storage_client-0.1.0/s3_object_storage_client.egg-info/dependency_links.txt
--rw-r--r--   0 lirui      (501) staff       (20)       23 2024-05-20 08:35:35.000000 s3_object_storage_client-0.1.0/s3_object_storage_client.egg-info/requires.txt
--rw-r--r--   0 lirui      (501) staff       (20)        7 2024-05-20 08:35:35.000000 s3_object_storage_client-0.1.0/s3_object_storage_client.egg-info/top_level.txt
--rw-r--r--   0 lirui      (501) staff       (20)       38 2024-05-20 08:35:36.000000 s3_object_storage_client-0.1.0/setup.cfg
--rw-r--r--   0 lirui      (501) staff       (20)      550 2024-05-20 08:35:21.000000 s3_object_storage_client-0.1.0/setup.py
+drwxr-xr-x   0 lirui      (501) staff       (20)        0 2024-05-20 10:20:23.000000 s3_object_storage_client-0.1.1/
+-rw-r--r--   0 lirui      (501) staff       (20)     1086 2022-07-15 07:21:28.000000 s3_object_storage_client-0.1.1/LICENSE
+-rw-r--r--   0 lirui      (501) staff       (20)      304 2024-05-20 10:20:23.000000 s3_object_storage_client-0.1.1/PKG-INFO
+-rw-r--r--   0 lirui      (501) staff       (20)        0 2022-10-25 02:05:30.000000 s3_object_storage_client-0.1.1/README.md
+drwxr-xr-x   0 lirui      (501) staff       (20)        0 2024-05-20 10:20:23.000000 s3_object_storage_client-0.1.1/pyCeph/
+-rw-r--r--   0 lirui      (501) staff       (20)       36 2022-07-15 09:06:50.000000 s3_object_storage_client-0.1.1/pyCeph/__init__.py
+-rw-r--r--   0 lirui      (501) staff       (20)     1190 2022-07-15 09:07:05.000000 s3_object_storage_client-0.1.1/pyCeph/aios3.py
+-rw-r--r--   0 lirui      (501) staff       (20)      486 2022-07-14 07:21:24.000000 s3_object_storage_client-0.1.1/pyCeph/crypto.py
+-rw-r--r--   0 lirui      (501) staff       (20)      979 2022-07-12 07:08:04.000000 s3_object_storage_client-0.1.1/pyCeph/log.py
+-rw-r--r--   0 lirui      (501) staff       (20)     4241 2024-05-20 08:12:31.000000 s3_object_storage_client-0.1.1/pyCeph/s3.py
+-rw-r--r--   0 lirui      (501) staff       (20)      645 2022-07-15 07:19:33.000000 s3_object_storage_client-0.1.1/pyproject.toml
+drwxr-xr-x   0 lirui      (501) staff       (20)        0 2024-05-20 10:20:23.000000 s3_object_storage_client-0.1.1/s3_object_storage_client.egg-info/
+-rw-r--r--   0 lirui      (501) staff       (20)      304 2024-05-20 10:20:22.000000 s3_object_storage_client-0.1.1/s3_object_storage_client.egg-info/PKG-INFO
+-rw-r--r--   0 lirui      (501) staff       (20)      359 2024-05-20 10:20:23.000000 s3_object_storage_client-0.1.1/s3_object_storage_client.egg-info/SOURCES.txt
+-rw-r--r--   0 lirui      (501) staff       (20)        1 2024-05-20 10:20:22.000000 s3_object_storage_client-0.1.1/s3_object_storage_client.egg-info/dependency_links.txt
+-rw-r--r--   0 lirui      (501) staff       (20)       23 2024-05-20 10:20:22.000000 s3_object_storage_client-0.1.1/s3_object_storage_client.egg-info/requires.txt
+-rw-r--r--   0 lirui      (501) staff       (20)        7 2024-05-20 10:20:23.000000 s3_object_storage_client-0.1.1/s3_object_storage_client.egg-info/top_level.txt
+-rw-r--r--   0 lirui      (501) staff       (20)       38 2024-05-20 10:20:23.000000 s3_object_storage_client-0.1.1/setup.cfg
+-rw-r--r--   0 lirui      (501) staff       (20)      550 2024-05-20 10:20:19.000000 s3_object_storage_client-0.1.1/setup.py
```

### Comparing `s3_object_storage_client-0.1.0/LICENSE` & `s3_object_storage_client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `s3_object_storage_client-0.1.0/pyCeph/aios3.py` & `s3_object_storage_client-0.1.1/pyCeph/aios3.py`

 * *Files identical despite different names*

### Comparing `s3_object_storage_client-0.1.0/pyCeph/log.py` & `s3_object_storage_client-0.1.1/pyCeph/log.py`

 * *Files identical despite different names*

### Comparing `s3_object_storage_client-0.1.0/pyCeph/s3.py` & `s3_object_storage_client-0.1.1/pyCeph/s3.py`

 * *Files identical despite different names*

### Comparing `s3_object_storage_client-0.1.0/pyproject.toml` & `s3_object_storage_client-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `s3_object_storage_client-0.1.0/setup.py` & `s3_object_storage_client-0.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="s3_object_storage_client",
-    version="0.1.0",
+    version="0.1.1",
     keywords=["pip", "py_s3", "s3", "ceph", "minio"],
     description="s3 using tool",
     long_description="s3 protocol using tool",
     license="MIT Licence",
     url="https://github.com/susufqx/pyCeph",
     author="susufqx",
     author_email="jiangsulirui@gmail.com",
```


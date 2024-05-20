# Comparing `tmp/adri_client-0.0.1.tar.gz` & `tmp/adri_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adri_client-0.0.1.tar", last modified: Mon May 20 11:44:06 2024, max compression
+gzip compressed data, was "adri_client-0.0.2.tar", last modified: Mon May 20 12:05:20 2024, max compression
```

## Comparing `adri_client-0.0.1.tar` & `adri_client-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 11:44:06.356195 adri_client-0.0.1/
--rw-rw-rw-   0        0        0      484 2024-05-20 11:44:06.354192 adri_client-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-20 11:44:06.351196 adri_client-0.0.1/adri_client.egg-info/
--rw-rw-rw-   0        0        0      484 2024-05-20 11:44:06.000000 adri_client-0.0.1/adri_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2024-05-20 11:44:06.000000 adri_client-0.0.1/adri_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 11:44:06.000000 adri_client-0.0.1/adri_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-05-20 11:44:06.000000 adri_client-0.0.1/adri_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-20 11:44:06.000000 adri_client-0.0.1/adri_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-20 11:44:06.348176 adri_client-0.0.1/adri_storage/
--rw-rw-rw-   0        0        0        0 2024-05-20 11:27:28.000000 adri_client-0.0.1/adri_storage/__init__.py
--rw-rw-rw-   0        0        0     1098 2024-05-20 11:18:27.000000 adri_client-0.0.1/adri_storage/client.py
--rw-rw-rw-   0        0        0       88 2024-05-19 11:03:38.000000 adri_client-0.0.1/adri_storage/client_enums.py
--rw-rw-rw-   0        0        0     7740 2024-05-20 10:35:56.000000 adri_client-0.0.1/adri_storage/local_client.py
--rw-rw-rw-   0        0        0     1996 2024-05-20 11:32:52.000000 adri_client-0.0.1/adri_storage/main.py
--rw-rw-rw-   0        0        0     4774 2024-05-20 11:18:04.000000 adri_client-0.0.1/adri_storage/s3_client.py
--rw-rw-rw-   0        0        0      618 2024-05-20 11:43:45.000000 adri_client-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-20 11:44:06.357195 adri_client-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 12:05:20.325100 adri_client-0.0.2/
+-rw-rw-rw-   0        0        0      485 2024-05-20 12:05:20.322095 adri_client-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 12:05:20.319502 adri_client-0.0.2/adri_client.egg-info/
+-rw-rw-rw-   0        0        0      485 2024-05-20 12:05:20.000000 adri_client-0.0.2/adri_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2024-05-20 12:05:20.000000 adri_client-0.0.2/adri_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 12:05:20.000000 adri_client-0.0.2/adri_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-20 12:05:20.000000 adri_client-0.0.2/adri_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-20 12:05:20.000000 adri_client-0.0.2/adri_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 12:05:20.316525 adri_client-0.0.2/adri_storage/
+-rw-rw-rw-   0        0        0        0 2024-05-20 11:27:28.000000 adri_client-0.0.2/adri_storage/__init__.py
+-rw-rw-rw-   0        0        0     1098 2024-05-20 11:18:27.000000 adri_client-0.0.2/adri_storage/client.py
+-rw-rw-rw-   0        0        0       88 2024-05-19 11:03:38.000000 adri_client-0.0.2/adri_storage/client_enums.py
+-rw-rw-rw-   0        0        0     7740 2024-05-20 10:35:56.000000 adri_client-0.0.2/adri_storage/local_client.py
+-rw-rw-rw-   0        0        0     1996 2024-05-20 11:32:52.000000 adri_client-0.0.2/adri_storage/main.py
+-rw-rw-rw-   0        0        0     4774 2024-05-20 11:18:04.000000 adri_client-0.0.2/adri_storage/s3_client.py
+-rw-rw-rw-   0        0        0      619 2024-05-20 12:04:58.000000 adri_client-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 12:05:20.325623 adri_client-0.0.2/setup.cfg
```

### Comparing `adri_client-0.0.1/adri_storage/client.py` & `adri_client-0.0.2/adri_storage/client.py`

 * *Files identical despite different names*

### Comparing `adri_client-0.0.1/adri_storage/local_client.py` & `adri_client-0.0.2/adri_storage/local_client.py`

 * *Files identical despite different names*

### Comparing `adri_client-0.0.1/adri_storage/main.py` & `adri_client-0.0.2/adri_storage/main.py`

 * *Files identical despite different names*

### Comparing `adri_client-0.0.1/adri_storage/s3_client.py` & `adri_client-0.0.2/adri_storage/s3_client.py`

 * *Files identical despite different names*

### Comparing `adri_client-0.0.1/pyproject.toml` & `adri_client-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "adri_client"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Khalid Rasool", email="khalid.rasool@adri.nz" },
   { name="Eslam Allam", email="eslam.allam@adri.nz" }
 ]
 description = "ADRI Storage Python SDK"
 requires-python = ">=3.8"
 classifiers = [
@@ -16,9 +16,9 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "boto3 ==1.18.0",
     "botocore ==1.21.0",
     "requests ==2.26.0",
-    "tracemalloc ==3.0.0"
+    "tracemalloc ==3.12.3"
 ]
```


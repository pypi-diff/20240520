# Comparing `tmp/sop_deutils-0.9.8.tar.gz` & `tmp/sop_deutils-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sop_deutils-0.9.8.tar", last modified: Fri Jan 12 10:10:43 2024, max compression
+gzip compressed data, was "sop_deutils-0.9.9.tar", last modified: Fri Jan 12 10:12:20 2024, max compression
```

## Comparing `sop_deutils-0.9.8.tar` & `sop_deutils-0.9.9.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:10:43.575005 sop_deutils-0.9.8/
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     1073 2023-10-06 10:24:21.000000 sop_deutils-0.9.8/LICENSE
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)       37 2023-10-06 10:24:21.000000 sop_deutils-0.9.8/MANIFEST.in
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)    43327 2024-01-12 10:10:43.575005 sop_deutils-0.9.8/PKG-INFO
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)    42882 2023-12-21 08:57:51.000000 sop_deutils-0.9.8/README.rst
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)      531 2024-01-12 10:10:27.000000 sop_deutils-0.9.8/pyproject.toml
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)       38 2024-01-12 10:10:43.575005 sop_deutils-0.9.8/setup.cfg
-drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:10:43.571005 sop_deutils-0.9.8/sop_deutils/
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2023-10-06 10:19:43.000000 sop_deutils-0.9.8/sop_deutils/__init__.py
-drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:10:43.575005 sop_deutils-0.9.8/sop_deutils/base/
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     1470 2023-10-18 08:51:46.000000 sop_deutils-0.9.8/sop_deutils/base/y4a_da_cfg.py
-drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:10:43.575005 sop_deutils-0.9.8/sop_deutils/datalake/
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     8133 2023-10-20 03:28:20.000000 sop_deutils-0.9.8/sop_deutils/datalake/y4a_minio.py
-drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:10:43.575005 sop_deutils-0.9.8/sop_deutils/gg_api/
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)       41 2023-10-11 04:30:07.000000 sop_deutils-0.9.8/sop_deutils/gg_api/config.ini
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)    14846 2024-01-08 08:03:23.000000 sop_deutils-0.9.8/sop_deutils/gg_api/y4a_sheet.py
-drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:10:43.575005 sop_deutils-0.9.8/sop_deutils/sql/
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     3499 2023-11-03 02:16:22.000000 sop_deutils-0.9.8/sop_deutils/sql/y4a_monitor_user.py
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     5820 2023-10-26 04:54:49.000000 sop_deutils-0.9.8/sop_deutils/sql/y4a_mysql.py
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)    52175 2024-01-12 10:07:30.000000 sop_deutils-0.9.8/sop_deutils/sql/y4a_postgresql.py
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     3927 2024-01-12 03:18:06.000000 sop_deutils-0.9.8/sop_deutils/y4a_airflow.py
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     1332 2023-11-28 02:11:29.000000 sop_deutils-0.9.8/sop_deutils/y4a_credentials.py
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     1016 2023-11-03 02:14:18.000000 sop_deutils-0.9.8/sop_deutils/y4a_retry.py
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     1096 2023-12-21 09:49:29.000000 sop_deutils-0.9.8/sop_deutils/y4a_telegram.py
-drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:10:43.575005 sop_deutils-0.9.8/sop_deutils.egg-info/
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)    43327 2024-01-12 10:10:43.000000 sop_deutils-0.9.8/sop_deutils.egg-info/PKG-INFO
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)      546 2024-01-12 10:10:43.000000 sop_deutils-0.9.8/sop_deutils.egg-info/SOURCES.txt
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        1 2024-01-12 10:10:43.000000 sop_deutils-0.9.8/sop_deutils.egg-info/dependency_links.txt
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)       12 2024-01-12 10:10:43.000000 sop_deutils-0.9.8/sop_deutils.egg-info/top_level.txt
+drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:12:20.151277 sop_deutils-0.9.9/
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     1073 2023-10-06 10:24:21.000000 sop_deutils-0.9.9/LICENSE
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)       37 2023-10-06 10:24:21.000000 sop_deutils-0.9.9/MANIFEST.in
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)    43826 2024-01-12 10:12:20.151277 sop_deutils-0.9.9/PKG-INFO
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)    42882 2023-12-21 08:57:51.000000 sop_deutils-0.9.9/README.rst
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)      895 2024-01-12 10:11:54.000000 sop_deutils-0.9.9/pyproject.toml
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)       38 2024-01-12 10:12:20.151277 sop_deutils-0.9.9/setup.cfg
+drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:12:20.151277 sop_deutils-0.9.9/sop_deutils/
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2023-10-06 10:19:43.000000 sop_deutils-0.9.9/sop_deutils/__init__.py
+drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:12:20.151277 sop_deutils-0.9.9/sop_deutils/base/
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     1470 2023-10-18 08:51:46.000000 sop_deutils-0.9.9/sop_deutils/base/y4a_da_cfg.py
+drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:12:20.151277 sop_deutils-0.9.9/sop_deutils/datalake/
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     8133 2023-10-20 03:28:20.000000 sop_deutils-0.9.9/sop_deutils/datalake/y4a_minio.py
+drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:12:20.151277 sop_deutils-0.9.9/sop_deutils/gg_api/
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)       41 2023-10-11 04:30:07.000000 sop_deutils-0.9.9/sop_deutils/gg_api/config.ini
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)    14846 2024-01-08 08:03:23.000000 sop_deutils-0.9.9/sop_deutils/gg_api/y4a_sheet.py
+drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:12:20.151277 sop_deutils-0.9.9/sop_deutils/sql/
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     3499 2023-11-03 02:16:22.000000 sop_deutils-0.9.9/sop_deutils/sql/y4a_monitor_user.py
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     5820 2023-10-26 04:54:49.000000 sop_deutils-0.9.9/sop_deutils/sql/y4a_mysql.py
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)    52175 2024-01-12 10:07:30.000000 sop_deutils-0.9.9/sop_deutils/sql/y4a_postgresql.py
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     3927 2024-01-12 03:18:06.000000 sop_deutils-0.9.9/sop_deutils/y4a_airflow.py
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     1332 2023-11-28 02:11:29.000000 sop_deutils-0.9.9/sop_deutils/y4a_credentials.py
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     1016 2023-11-03 02:14:18.000000 sop_deutils-0.9.9/sop_deutils/y4a_retry.py
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     1096 2023-12-21 09:49:29.000000 sop_deutils-0.9.9/sop_deutils/y4a_telegram.py
+drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:12:20.151277 sop_deutils-0.9.9/sop_deutils.egg-info/
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)    43826 2024-01-12 10:12:20.000000 sop_deutils-0.9.9/sop_deutils.egg-info/PKG-INFO
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)      580 2024-01-12 10:12:20.000000 sop_deutils-0.9.9/sop_deutils.egg-info/SOURCES.txt
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        1 2024-01-12 10:12:20.000000 sop_deutils-0.9.9/sop_deutils.egg-info/dependency_links.txt
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)      274 2024-01-12 10:12:20.000000 sop_deutils-0.9.9/sop_deutils.egg-info/requires.txt
+-rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)       12 2024-01-12 10:12:20.000000 sop_deutils-0.9.9/sop_deutils.egg-info/top_level.txt
```

### Comparing `sop_deutils-0.9.8/LICENSE` & `sop_deutils-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sop_deutils-0.9.8/PKG-INFO` & `sop_deutils-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,34 @@
 Metadata-Version: 2.1
 Name: sop_deutils
-Version: 0.9.8
+Version: 0.9.9
 Summary: A utils package for Yes4All SOP
 Author-email: liuliukiki aka clong <longnc@yes4all.com>
 Project-URL: Author_Github, https://github.com/dribblewithclong
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: openpyxl==3.1.2
+Requires-Dist: pytz==2023.3
+Requires-Dist: pandas==2.0.3
+Requires-Dist: python-telegram-bot==20.5
+Requires-Dist: SQLAlchemy==1.4.49
+Requires-Dist: lxml==4.9.3
+Requires-Dist: gspread==5.11.1
+Requires-Dist: psycopg2-binary==2.9.7
+Requires-Dist: minio==7.1.16
+Requires-Dist: pyarrow==11.0.0
+Requires-Dist: requests==2.30.0
+Requires-Dist: aiofiles==23.2.1
+Requires-Dist: fastparquet==2023.8.0
+Requires-Dist: mysql-connector-python==8.1.0
+Requires-Dist: SQLAlchemy==1.4.49
 
 Yes4All SOP Utils Packages
 ==========================
 
 This is a utils package served for SOP Data Analytics team at **Yes4All**. It contains various modules to work with **PostgreSQL, MinIO, Google API, Airflow, Telegram…**
 
 .. image::
```

### Comparing `sop_deutils-0.9.8/README.rst` & `sop_deutils-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `sop_deutils-0.9.8/sop_deutils/base/y4a_da_cfg.py` & `sop_deutils-0.9.9/sop_deutils/base/y4a_da_cfg.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-0.9.8/sop_deutils/datalake/y4a_minio.py` & `sop_deutils-0.9.9/sop_deutils/datalake/y4a_minio.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-0.9.8/sop_deutils/gg_api/y4a_sheet.py` & `sop_deutils-0.9.9/sop_deutils/gg_api/y4a_sheet.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-0.9.8/sop_deutils/sql/y4a_monitor_user.py` & `sop_deutils-0.9.9/sop_deutils/sql/y4a_monitor_user.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-0.9.8/sop_deutils/sql/y4a_mysql.py` & `sop_deutils-0.9.9/sop_deutils/sql/y4a_mysql.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-0.9.8/sop_deutils/sql/y4a_postgresql.py` & `sop_deutils-0.9.9/sop_deutils/sql/y4a_postgresql.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-0.9.8/sop_deutils/y4a_airflow.py` & `sop_deutils-0.9.9/sop_deutils/y4a_airflow.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-0.9.8/sop_deutils/y4a_credentials.py` & `sop_deutils-0.9.9/sop_deutils/y4a_credentials.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-0.9.8/sop_deutils/y4a_retry.py` & `sop_deutils-0.9.9/sop_deutils/y4a_retry.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-0.9.8/sop_deutils/y4a_telegram.py` & `sop_deutils-0.9.9/sop_deutils/y4a_telegram.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-0.9.8/sop_deutils.egg-info/PKG-INFO` & `sop_deutils-0.9.9/sop_deutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,34 @@
 Metadata-Version: 2.1
 Name: sop_deutils
-Version: 0.9.8
+Version: 0.9.9
 Summary: A utils package for Yes4All SOP
 Author-email: liuliukiki aka clong <longnc@yes4all.com>
 Project-URL: Author_Github, https://github.com/dribblewithclong
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: openpyxl==3.1.2
+Requires-Dist: pytz==2023.3
+Requires-Dist: pandas==2.0.3
+Requires-Dist: python-telegram-bot==20.5
+Requires-Dist: SQLAlchemy==1.4.49
+Requires-Dist: lxml==4.9.3
+Requires-Dist: gspread==5.11.1
+Requires-Dist: psycopg2-binary==2.9.7
+Requires-Dist: minio==7.1.16
+Requires-Dist: pyarrow==11.0.0
+Requires-Dist: requests==2.30.0
+Requires-Dist: aiofiles==23.2.1
+Requires-Dist: fastparquet==2023.8.0
+Requires-Dist: mysql-connector-python==8.1.0
+Requires-Dist: SQLAlchemy==1.4.49
 
 Yes4All SOP Utils Packages
 ==========================
 
 This is a utils package served for SOP Data Analytics team at **Yes4All**. It contains various modules to work with **PostgreSQL, MinIO, Google API, Airflow, Telegram…**
 
 .. image::
```

### Comparing `sop_deutils-0.9.8/sop_deutils.egg-info/SOURCES.txt` & `sop_deutils-0.9.9/sop_deutils.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 sop_deutils/y4a_airflow.py
 sop_deutils/y4a_credentials.py
 sop_deutils/y4a_retry.py
 sop_deutils/y4a_telegram.py
 sop_deutils.egg-info/PKG-INFO
 sop_deutils.egg-info/SOURCES.txt
 sop_deutils.egg-info/dependency_links.txt
+sop_deutils.egg-info/requires.txt
 sop_deutils.egg-info/top_level.txt
 sop_deutils/base/y4a_da_cfg.py
 sop_deutils/datalake/y4a_minio.py
 sop_deutils/gg_api/config.ini
 sop_deutils/gg_api/y4a_sheet.py
 sop_deutils/sql/y4a_monitor_user.py
 sop_deutils/sql/y4a_mysql.py
```


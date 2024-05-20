# Comparing `tmp/sop_deutils-1.0.1.tar.gz` & `tmp/sop_deutils-1.0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sop_deutils-1.0.1.tar", last modified: Mon May 20 02:20:17 2024, max compression
+gzip compressed data, was "sop_deutils-1.0.1.dev0.tar", last modified: Mon May 20 02:19:58 2024, max compression
```

## Comparing `sop_deutils-1.0.1.tar` & `sop_deutils-1.0.1.dev0.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 02:20:17.323488 sop_deutils-1.0.1/
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     1091 2024-05-18 13:33:42.000000 sop_deutils-1.0.1/LICENSE
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)       63 2024-05-18 13:35:44.000000 sop_deutils-1.0.1/MANIFEST.in
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    53435 2024-05-20 02:20:17.323488 sop_deutils-1.0.1/PKG-INFO
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    52285 2024-05-19 07:45:03.000000 sop_deutils-1.0.1/README.rst
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     1002 2024-05-20 02:20:16.000000 sop_deutils-1.0.1/pyproject.toml
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)       38 2024-05-20 02:20:17.323488 sop_deutils-1.0.1/setup.cfg
-drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 02:20:17.323488 sop_deutils-1.0.1/sop_deutils/
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-18 02:26:47.000000 sop_deutils-1.0.1/sop_deutils/__init__.py
-drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 02:20:17.323488 sop_deutils-1.0.1/sop_deutils/base/
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     1470 2024-05-18 02:26:47.000000 sop_deutils-1.0.1/sop_deutils/base/y4a_da_cfg.py
-drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 02:20:17.323488 sop_deutils-1.0.1/sop_deutils/datalake/
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     8133 2024-05-18 02:26:47.000000 sop_deutils-1.0.1/sop_deutils/datalake/y4a_minio.py
-drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 02:20:17.323488 sop_deutils-1.0.1/sop_deutils/gg_api/
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)       41 2024-05-18 02:26:47.000000 sop_deutils-1.0.1/sop_deutils/gg_api/config.ini
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     2131 2024-05-18 02:26:47.000000 sop_deutils-1.0.1/sop_deutils/gg_api/y4a_chat.py
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     6236 2024-05-18 02:26:47.000000 sop_deutils-1.0.1/sop_deutils/gg_api/y4a_mail.py
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    19617 2024-05-19 07:09:02.000000 sop_deutils-1.0.1/sop_deutils/gg_api/y4a_sheet.py
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    11827 2024-05-18 13:05:12.000000 sop_deutils-1.0.1/sop_deutils/r.zip
-drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 02:20:17.323488 sop_deutils-1.0.1/sop_deutils/sql/
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     4330 2024-05-18 02:26:47.000000 sop_deutils-1.0.1/sop_deutils/sql/y4a_monitor_user.py
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     5820 2024-05-18 02:26:47.000000 sop_deutils-1.0.1/sop_deutils/sql/y4a_mysql.py
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    50237 2024-05-19 06:00:03.000000 sop_deutils-1.0.1/sop_deutils/sql/y4a_postgresql.py
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     3927 2024-05-18 02:26:47.000000 sop_deutils-1.0.1/sop_deutils/y4a_airflow.py
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)      748 2024-05-19 04:32:14.000000 sop_deutils-1.0.1/sop_deutils/y4a_credentials.py
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     1218 2024-05-18 02:26:47.000000 sop_deutils-1.0.1/sop_deutils/y4a_retry.py
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     2925 2024-05-18 02:26:47.000000 sop_deutils-1.0.1/sop_deutils/y4a_telegram.py
-drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 02:20:17.323488 sop_deutils-1.0.1/sop_deutils.egg-info/
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    53435 2024-05-20 02:20:17.000000 sop_deutils-1.0.1/sop_deutils.egg-info/PKG-INFO
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)      660 2024-05-20 02:20:17.000000 sop_deutils-1.0.1/sop_deutils.egg-info/SOURCES.txt
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        1 2024-05-20 02:20:17.000000 sop_deutils-1.0.1/sop_deutils.egg-info/dependency_links.txt
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)      380 2024-05-20 02:20:17.000000 sop_deutils-1.0.1/sop_deutils.egg-info/requires.txt
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)       12 2024-05-20 02:20:17.000000 sop_deutils-1.0.1/sop_deutils.egg-info/top_level.txt
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 02:19:58.202513 sop_deutils-1.0.1.dev0/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     1091 2024-05-18 13:33:42.000000 sop_deutils-1.0.1.dev0/LICENSE
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)       63 2024-05-18 13:35:44.000000 sop_deutils-1.0.1.dev0/MANIFEST.in
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    52760 2024-05-20 02:19:58.202513 sop_deutils-1.0.1.dev0/PKG-INFO
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    52285 2024-05-19 07:45:03.000000 sop_deutils-1.0.1.dev0/README.rst
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)      548 2024-05-20 02:19:57.000000 sop_deutils-1.0.1.dev0/pyproject.toml
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)       38 2024-05-20 02:19:58.202513 sop_deutils-1.0.1.dev0/setup.cfg
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 02:19:58.192513 sop_deutils-1.0.1.dev0/sop_deutils/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-18 02:26:47.000000 sop_deutils-1.0.1.dev0/sop_deutils/__init__.py
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 02:19:58.192513 sop_deutils-1.0.1.dev0/sop_deutils/base/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     1470 2024-05-18 02:26:47.000000 sop_deutils-1.0.1.dev0/sop_deutils/base/y4a_da_cfg.py
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 02:19:58.192513 sop_deutils-1.0.1.dev0/sop_deutils/datalake/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     8133 2024-05-18 02:26:47.000000 sop_deutils-1.0.1.dev0/sop_deutils/datalake/y4a_minio.py
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 02:19:58.192513 sop_deutils-1.0.1.dev0/sop_deutils/gg_api/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)       41 2024-05-18 02:26:47.000000 sop_deutils-1.0.1.dev0/sop_deutils/gg_api/config.ini
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     2131 2024-05-18 02:26:47.000000 sop_deutils-1.0.1.dev0/sop_deutils/gg_api/y4a_chat.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     6236 2024-05-18 02:26:47.000000 sop_deutils-1.0.1.dev0/sop_deutils/gg_api/y4a_mail.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    19617 2024-05-19 07:09:02.000000 sop_deutils-1.0.1.dev0/sop_deutils/gg_api/y4a_sheet.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    11827 2024-05-18 13:05:12.000000 sop_deutils-1.0.1.dev0/sop_deutils/r.zip
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 02:19:58.192513 sop_deutils-1.0.1.dev0/sop_deutils/sql/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     4330 2024-05-18 02:26:47.000000 sop_deutils-1.0.1.dev0/sop_deutils/sql/y4a_monitor_user.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     5820 2024-05-18 02:26:47.000000 sop_deutils-1.0.1.dev0/sop_deutils/sql/y4a_mysql.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    50237 2024-05-19 06:00:03.000000 sop_deutils-1.0.1.dev0/sop_deutils/sql/y4a_postgresql.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     3927 2024-05-18 02:26:47.000000 sop_deutils-1.0.1.dev0/sop_deutils/y4a_airflow.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)      748 2024-05-19 04:32:14.000000 sop_deutils-1.0.1.dev0/sop_deutils/y4a_credentials.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     1218 2024-05-18 02:26:47.000000 sop_deutils-1.0.1.dev0/sop_deutils/y4a_retry.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     2925 2024-05-18 02:26:47.000000 sop_deutils-1.0.1.dev0/sop_deutils/y4a_telegram.py
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 02:19:58.192513 sop_deutils-1.0.1.dev0/sop_deutils.egg-info/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    52760 2024-05-20 02:19:58.000000 sop_deutils-1.0.1.dev0/sop_deutils.egg-info/PKG-INFO
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)      626 2024-05-20 02:19:58.000000 sop_deutils-1.0.1.dev0/sop_deutils.egg-info/SOURCES.txt
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        1 2024-05-20 02:19:58.000000 sop_deutils-1.0.1.dev0/sop_deutils.egg-info/dependency_links.txt
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)       12 2024-05-20 02:19:58.000000 sop_deutils-1.0.1.dev0/sop_deutils.egg-info/top_level.txt
```

### Comparing `sop_deutils-1.0.1/LICENSE` & `sop_deutils-1.0.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.1/PKG-INFO` & `sop_deutils-1.0.1.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,19 @@
 Metadata-Version: 2.1
 Name: sop_deutils
-Version: 1.0.1
+Version: 1.0.1.dev0
 Summary: A utils package for Yes4All SOP
 Author-email: liuliukiki aka clong aka ifyouknowyouknow101 <longnc@yes4all.com>
 Project-URL: Author_Github, https://github.com/dribblewithclong
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: openpyxl==3.1.2
-Requires-Dist: pytz==2023.3
-Requires-Dist: pandas==2.0.3
-Requires-Dist: python-telegram-bot==20.5
-Requires-Dist: SQLAlchemy==1.4.49
-Requires-Dist: lxml==4.9.3
-Requires-Dist: gspread==5.11.1
-Requires-Dist: psycopg2-binary==2.9.7
-Requires-Dist: minio==7.1.16
-Requires-Dist: pyarrow==11.0.0
-Requires-Dist: requests==2.30.0
-Requires-Dist: aiofiles==23.2.1
-Requires-Dist: fastparquet==2023.8.0
-Requires-Dist: mysql-connector-python==8.1.0
-Requires-Dist: SQLAlchemy==1.4.49
-Requires-Dist: httplib2==0.22.0
-Requires-Dist: python-dateutil==2.9.0.post0
-Requires-Dist: cryptography==42.0.7
-Requires-Dist: PyYAML==6.0.1
-Requires-Dist: gspread-dataframe==3.3.1
 
 Yes4All SOP Utils Packages
 ==========================
 
 This is a utils package served for SOP Data Analytics team at **Yes4All**. It contains various modules to work with **PostgreSQL, MinIO, Google API, Airflow, Telegram…**
 
 .. image::
```

### Comparing `sop_deutils-1.0.1/README.rst` & `sop_deutils-1.0.1.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.1/sop_deutils/base/y4a_da_cfg.py` & `sop_deutils-1.0.1.dev0/sop_deutils/base/y4a_da_cfg.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.1/sop_deutils/datalake/y4a_minio.py` & `sop_deutils-1.0.1.dev0/sop_deutils/datalake/y4a_minio.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.1/sop_deutils/gg_api/y4a_chat.py` & `sop_deutils-1.0.1.dev0/sop_deutils/gg_api/y4a_chat.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.1/sop_deutils/gg_api/y4a_mail.py` & `sop_deutils-1.0.1.dev0/sop_deutils/gg_api/y4a_mail.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.1/sop_deutils/gg_api/y4a_sheet.py` & `sop_deutils-1.0.1.dev0/sop_deutils/gg_api/y4a_sheet.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.1/sop_deutils/r.zip` & `sop_deutils-1.0.1.dev0/sop_deutils/r.zip`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.1/sop_deutils/sql/y4a_monitor_user.py` & `sop_deutils-1.0.1.dev0/sop_deutils/sql/y4a_monitor_user.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.1/sop_deutils/sql/y4a_mysql.py` & `sop_deutils-1.0.1.dev0/sop_deutils/sql/y4a_mysql.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.1/sop_deutils/sql/y4a_postgresql.py` & `sop_deutils-1.0.1.dev0/sop_deutils/sql/y4a_postgresql.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.1/sop_deutils/y4a_airflow.py` & `sop_deutils-1.0.1.dev0/sop_deutils/y4a_airflow.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.1/sop_deutils/y4a_credentials.py` & `sop_deutils-1.0.1.dev0/sop_deutils/y4a_credentials.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.1/sop_deutils/y4a_retry.py` & `sop_deutils-1.0.1.dev0/sop_deutils/y4a_retry.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.1/sop_deutils/y4a_telegram.py` & `sop_deutils-1.0.1.dev0/sop_deutils/y4a_telegram.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.1/sop_deutils.egg-info/PKG-INFO` & `sop_deutils-1.0.1.dev0/sop_deutils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,19 @@
 Metadata-Version: 2.1
 Name: sop_deutils
-Version: 1.0.1
+Version: 1.0.1.dev0
 Summary: A utils package for Yes4All SOP
 Author-email: liuliukiki aka clong aka ifyouknowyouknow101 <longnc@yes4all.com>
 Project-URL: Author_Github, https://github.com/dribblewithclong
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: openpyxl==3.1.2
-Requires-Dist: pytz==2023.3
-Requires-Dist: pandas==2.0.3
-Requires-Dist: python-telegram-bot==20.5
-Requires-Dist: SQLAlchemy==1.4.49
-Requires-Dist: lxml==4.9.3
-Requires-Dist: gspread==5.11.1
-Requires-Dist: psycopg2-binary==2.9.7
-Requires-Dist: minio==7.1.16
-Requires-Dist: pyarrow==11.0.0
-Requires-Dist: requests==2.30.0
-Requires-Dist: aiofiles==23.2.1
-Requires-Dist: fastparquet==2023.8.0
-Requires-Dist: mysql-connector-python==8.1.0
-Requires-Dist: SQLAlchemy==1.4.49
-Requires-Dist: httplib2==0.22.0
-Requires-Dist: python-dateutil==2.9.0.post0
-Requires-Dist: cryptography==42.0.7
-Requires-Dist: PyYAML==6.0.1
-Requires-Dist: gspread-dataframe==3.3.1
 
 Yes4All SOP Utils Packages
 ==========================
 
 This is a utils package served for SOP Data Analytics team at **Yes4All**. It contains various modules to work with **PostgreSQL, MinIO, Google API, Airflow, Telegram…**
 
 .. image::
```

### Comparing `sop_deutils-1.0.1/sop_deutils.egg-info/SOURCES.txt` & `sop_deutils-1.0.1.dev0/sop_deutils.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 sop_deutils/y4a_airflow.py
 sop_deutils/y4a_credentials.py
 sop_deutils/y4a_retry.py
 sop_deutils/y4a_telegram.py
 sop_deutils.egg-info/PKG-INFO
 sop_deutils.egg-info/SOURCES.txt
 sop_deutils.egg-info/dependency_links.txt
-sop_deutils.egg-info/requires.txt
 sop_deutils.egg-info/top_level.txt
 sop_deutils/base/y4a_da_cfg.py
 sop_deutils/datalake/y4a_minio.py
 sop_deutils/gg_api/config.ini
 sop_deutils/gg_api/y4a_chat.py
 sop_deutils/gg_api/y4a_mail.py
 sop_deutils/gg_api/y4a_sheet.py
```


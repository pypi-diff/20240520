# Comparing `tmp/sop_deutils-0.9.9.tar.gz` & `tmp/sop_deutils-1.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sop_deutils-0.9.9.tar", last modified: Fri Jan 12 10:12:20 2024, max compression
+gzip compressed data, was "sop_deutils-1.0.0.dev0.tar", last modified: Mon May 20 01:58:13 2024, max compression
```

## Comparing `sop_deutils-0.9.9.tar` & `sop_deutils-1.0.0.dev0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:12:20.151277 sop_deutils-0.9.9/
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     1073 2023-10-06 10:24:21.000000 sop_deutils-0.9.9/LICENSE
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)       37 2023-10-06 10:24:21.000000 sop_deutils-0.9.9/MANIFEST.in
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)    43826 2024-01-12 10:12:20.151277 sop_deutils-0.9.9/PKG-INFO
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)    42882 2023-12-21 08:57:51.000000 sop_deutils-0.9.9/README.rst
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)      895 2024-01-12 10:11:54.000000 sop_deutils-0.9.9/pyproject.toml
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)       38 2024-01-12 10:12:20.151277 sop_deutils-0.9.9/setup.cfg
-drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:12:20.151277 sop_deutils-0.9.9/sop_deutils/
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2023-10-06 10:19:43.000000 sop_deutils-0.9.9/sop_deutils/__init__.py
-drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:12:20.151277 sop_deutils-0.9.9/sop_deutils/base/
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     1470 2023-10-18 08:51:46.000000 sop_deutils-0.9.9/sop_deutils/base/y4a_da_cfg.py
-drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:12:20.151277 sop_deutils-0.9.9/sop_deutils/datalake/
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     8133 2023-10-20 03:28:20.000000 sop_deutils-0.9.9/sop_deutils/datalake/y4a_minio.py
-drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:12:20.151277 sop_deutils-0.9.9/sop_deutils/gg_api/
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)       41 2023-10-11 04:30:07.000000 sop_deutils-0.9.9/sop_deutils/gg_api/config.ini
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)    14846 2024-01-08 08:03:23.000000 sop_deutils-0.9.9/sop_deutils/gg_api/y4a_sheet.py
-drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:12:20.151277 sop_deutils-0.9.9/sop_deutils/sql/
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     3499 2023-11-03 02:16:22.000000 sop_deutils-0.9.9/sop_deutils/sql/y4a_monitor_user.py
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     5820 2023-10-26 04:54:49.000000 sop_deutils-0.9.9/sop_deutils/sql/y4a_mysql.py
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)    52175 2024-01-12 10:07:30.000000 sop_deutils-0.9.9/sop_deutils/sql/y4a_postgresql.py
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     3927 2024-01-12 03:18:06.000000 sop_deutils-0.9.9/sop_deutils/y4a_airflow.py
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     1332 2023-11-28 02:11:29.000000 sop_deutils-0.9.9/sop_deutils/y4a_credentials.py
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     1016 2023-11-03 02:14:18.000000 sop_deutils-0.9.9/sop_deutils/y4a_retry.py
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)     1096 2023-12-21 09:49:29.000000 sop_deutils-0.9.9/sop_deutils/y4a_telegram.py
-drwxr-xr-x   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        0 2024-01-12 10:12:20.151277 sop_deutils-0.9.9/sop_deutils.egg-info/
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)    43826 2024-01-12 10:12:20.000000 sop_deutils-0.9.9/sop_deutils.egg-info/PKG-INFO
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)      580 2024-01-12 10:12:20.000000 sop_deutils-0.9.9/sop_deutils.egg-info/SOURCES.txt
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)        1 2024-01-12 10:12:20.000000 sop_deutils-0.9.9/sop_deutils.egg-info/dependency_links.txt
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)      274 2024-01-12 10:12:20.000000 sop_deutils-0.9.9/sop_deutils.egg-info/requires.txt
--rw-r--r--   0 longnc@yes4all.internal (596403369) s-1-5-21-2340968596-4135200257-3917301534-513@yes4all.internal (596400513)       12 2024-01-12 10:12:20.000000 sop_deutils-0.9.9/sop_deutils.egg-info/top_level.txt
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 01:58:13.122522 sop_deutils-1.0.0.dev0/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     1091 2024-05-18 13:33:42.000000 sop_deutils-1.0.0.dev0/LICENSE
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)       63 2024-05-18 13:35:44.000000 sop_deutils-1.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    52760 2024-05-20 01:58:13.122522 sop_deutils-1.0.0.dev0/PKG-INFO
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    52285 2024-05-19 07:45:03.000000 sop_deutils-1.0.0.dev0/README.rst
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)      548 2024-05-20 01:58:12.000000 sop_deutils-1.0.0.dev0/pyproject.toml
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)       38 2024-05-20 01:58:13.122522 sop_deutils-1.0.0.dev0/setup.cfg
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 01:58:13.122522 sop_deutils-1.0.0.dev0/sop_deutils/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-18 02:26:47.000000 sop_deutils-1.0.0.dev0/sop_deutils/__init__.py
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 01:58:13.122522 sop_deutils-1.0.0.dev0/sop_deutils/base/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     1470 2024-05-18 02:26:47.000000 sop_deutils-1.0.0.dev0/sop_deutils/base/y4a_da_cfg.py
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 01:58:13.122522 sop_deutils-1.0.0.dev0/sop_deutils/datalake/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     8133 2024-05-18 02:26:47.000000 sop_deutils-1.0.0.dev0/sop_deutils/datalake/y4a_minio.py
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 01:58:13.122522 sop_deutils-1.0.0.dev0/sop_deutils/gg_api/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)       41 2024-05-18 02:26:47.000000 sop_deutils-1.0.0.dev0/sop_deutils/gg_api/config.ini
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     2131 2024-05-18 02:26:47.000000 sop_deutils-1.0.0.dev0/sop_deutils/gg_api/y4a_chat.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     6236 2024-05-18 02:26:47.000000 sop_deutils-1.0.0.dev0/sop_deutils/gg_api/y4a_mail.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    19617 2024-05-19 07:09:02.000000 sop_deutils-1.0.0.dev0/sop_deutils/gg_api/y4a_sheet.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    11827 2024-05-18 13:05:12.000000 sop_deutils-1.0.0.dev0/sop_deutils/r.zip
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 01:58:13.122522 sop_deutils-1.0.0.dev0/sop_deutils/sql/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     4330 2024-05-18 02:26:47.000000 sop_deutils-1.0.0.dev0/sop_deutils/sql/y4a_monitor_user.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     5820 2024-05-18 02:26:47.000000 sop_deutils-1.0.0.dev0/sop_deutils/sql/y4a_mysql.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    50237 2024-05-19 06:00:03.000000 sop_deutils-1.0.0.dev0/sop_deutils/sql/y4a_postgresql.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     3927 2024-05-18 02:26:47.000000 sop_deutils-1.0.0.dev0/sop_deutils/y4a_airflow.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)      748 2024-05-19 04:32:14.000000 sop_deutils-1.0.0.dev0/sop_deutils/y4a_credentials.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     1218 2024-05-18 02:26:47.000000 sop_deutils-1.0.0.dev0/sop_deutils/y4a_retry.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     2925 2024-05-18 02:26:47.000000 sop_deutils-1.0.0.dev0/sop_deutils/y4a_telegram.py
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 01:58:13.122522 sop_deutils-1.0.0.dev0/sop_deutils.egg-info/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    52760 2024-05-20 01:58:13.000000 sop_deutils-1.0.0.dev0/sop_deutils.egg-info/PKG-INFO
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)      626 2024-05-20 01:58:13.000000 sop_deutils-1.0.0.dev0/sop_deutils.egg-info/SOURCES.txt
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        1 2024-05-20 01:58:13.000000 sop_deutils-1.0.0.dev0/sop_deutils.egg-info/dependency_links.txt
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)       12 2024-05-20 01:58:13.000000 sop_deutils-1.0.0.dev0/sop_deutils.egg-info/top_level.txt
```

### Comparing `sop_deutils-0.9.9/LICENSE` & `sop_deutils-1.0.0.dev0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `sop_deutils-0.9.9/PKG-INFO` & `sop_deutils-1.0.0.dev0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,27 @@
 Metadata-Version: 2.1
 Name: sop_deutils
-Version: 0.9.9
+Version: 1.0.0.dev0
 Summary: A utils package for Yes4All SOP
-Author-email: liuliukiki aka clong <longnc@yes4all.com>
+Author-email: liuliukiki aka clong aka ifyouknowyouknow101 <longnc@yes4all.com>
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
 
 Yes4All SOP Utils Packages
 ==========================
 
 This is a utils package served for SOP Data Analytics team at **Yes4All**. It contains various modules to work with **PostgreSQL, MinIO, Google API, Airflow, Telegram…**
 
 .. image::
-   https://lh3.googleusercontent.com/drive-viewer/AK7aPaASSw5LzlIMog6XonAGba7CsmObYVMzQLzxMeBMFTuK30MCmuvB9ZOR-9VCq47rQpdgou849BL-oj5cufSECqxuE67c_w=s1600
+   https://lh3.googleusercontent.com/drive-viewer/AKGpihbzwqCnULTRFR1ihxbk2jwhfwhVfiZWGLfZ2W1argxs96TxMzfRTfaGgNQoL7NALlz94lMLrQnoK2y3jgOxh7raeq2rKJzU5sQ=s1600-rw-v1
    :scale: 20%
    :alt: liuliukiki
 
 --------------
 
 Contents Overview
 -----------------
@@ -262,14 +247,18 @@
 
 - ``sheet_name`` (optional): Worksheet name. The default value is ``'Sheet1'``. **(str)**
 
 - ``from_row_index`` (optional): The index of the row from which to begin inserting. The default value is ``1``. **(int)**
 
 - ``insert_column_names`` (optional): Whether to insert column names. The default value is ``False``. **(bool)**
 
+- ``parse_input`` (optional): Whether to parse input values as if the user typed them into the UI. The default value is ``True``. **(bool)**
+
+- ``pre_process`` (optional): Whether to process input based on the pre-defined function of DA. The default value is ``True``. **(bool)**
+
 .. code-block:: python
 
     sheet_utils.insert_data(
         data=df,
         sheet_id='your-sheet-id',
         from_row_index=2,
         insert_column_names=False,
@@ -284,14 +273,18 @@
 
 - ``sheet_id`` (required): Spreadsheet ID. **(str)**
 
 - ``sheet_name`` (optional): Worksheet name. The default value is ``'Sheet1'``. **(str)**
 
 - ``range_from`` (optional): The beginning of the range of data to update. The default value is ``'A1'``. **(str)**
 
+- ``parse_input`` (optional): Whether to parse input values as if the user typed them into the UI. The default value is ``True``. **(bool)**
+
+- ``pre_process`` (optional): Whether to process input based on the pre-defined function of DA. The default value is ``True``. **(bool)**
+
 .. code-block:: python
 
     sheet_utils.update_data(
         data=new_df,
         sheet_id='your-sheet-id',
         range_from='A4',
     )
@@ -392,27 +385,64 @@
 
 .. code-block:: python
 
     ss = sheet_utils.open_spread_sheet(
         sheet_id='your-sheet-id',
     )
 
+2.14 ``gspread_load_data``
+''''''''''''''''''''''''''''''''''''''
+
+To load data to the given sheet, using ``gspread_load_data`` method. This method is integrated with GSpread load data function that provides the high efficiency and convenience, it can be used as the alternative of two methods ``insert_data`` and ``update_data``, it has the following parameters:
+
+- ``data`` (required): Dataframe containing data to load. **(pd.DataFrame)**
+
+- ``sheet_id`` (required): Spreadsheet ID. **(str)**
+
+- ``sheet_name`` (optional): Worksheet name. The default value is ``'Sheet1'``. **(str)**
+
+- ``from_row`` (optional): Row at which to start loading the DataFrame. The default value is ``1``. **(int)**
+
+- ``from_col`` (optional): Column at which to start loading the DataFrame. The default value is ``1``. **(int)**
+
+- ``include_index`` (optional): Whether to include the DataFrame's index as an additional column. The default value is ``False``. **(bool)**
+
+- ``include_column`` (optional): Whether to add a header row or rows before data with column names (if include_index is True, the index's name(s) will be used as its columns' headers). The default value is ``True``. **(bool)**
+
+- ``resize_worksheet`` (optional): If True, changes the worksheet's size to match the shape of the provided DataFrame, if False, worksheet will only be resized as necessary to contain the DataFrame contents. The default value is ``False``. **(bool)**
+
+- ``allow_formulas`` (optional): Whether to interprets ``=foo`` as a formula in cell values; otherwise all text beginning with ``=`` is escaped to avoid its interpretation as a formula. The default value is ``True``. **(bool)**
+
+- ``string_escaping`` (optional): Determines when string values are escaped as text literals (by adding an initial ``'`` character) in requests to Sheets API, 3 parameter values are accepted: ('default': only escape strings starting with a literal ``'`` character. 'off': escape nothing; cell values starting with a ``'`` will be interpreted by sheets as an escape character followed by a text literal. 'full': escape all string values), the escaping done when allow_formulas=False (escaping string values beginning with ``=``) is unaffected by this parameter's value. The default value is ``'default'``. **(str)**
+
+.. code-block:: python
+
+    sheet_utils.gspread_load_data(
+        data=df,
+        sheet_id='your-sheet-id',
+        sheet_name='Sheet1',
+        from_row=3,
+        from_col=4,
+        include_index=True,
+        include_column=True,
+    )
+
 --------------
 
 MinIO
 ^^^^^
 
 MinIO is an object storage, it is API compatible with the Amazon S3 cloud storage service. MinIO can be used as a **datalake** to store unstructured data (photos, videos, log files, backups, and container images) and structured data.
 
 **Use case:** when need to store raw data or get raw data from datalake. Notes that the stored data extension must be ``.parquet`` .
 
 **Notes about how to determine the** ``file_path`` **parameter in minIO when using this module:**
 
 .. figure::
-   https://lh3.googleusercontent.com/drive-viewer/AEYmBYTeW1mCFR9M_cI4vg_bRRaLUVVxPtvkoWenEecrXSbmju3Xujj8jMI_MgiGBn-F5ozkkDPAWLPATwZ8JtdkciDopAaf=s1600
+   https://lh3.googleusercontent.com/drive-viewer/AEYmBYTnHBUSHkf9nTE9TuXWpEh12YMfUvHp2If3pJnjiRlmw6kdhqPrrprI-zMmdgM4O5pvSR8q1u5m5-XNRCo4Mc4rKJ-J=s1600
    :alt: minIO file path
 
 ..
 
    For example, if the directory to the data file in minIO is as above, then the ``file_path`` is ``"/scraping/amazon_vendor/avc_bulk_buy_request/2023/9/24/batch_1695525619"`` (after removing bucket name, data storage mode, and data file extension).
 
 **Functional:**
@@ -600,16 +630,14 @@
 
     pg_utils = PostgreSQLUtils(
         pg_name='serving_master',
         pg_account='y4a_sop_user1',
         pg_password='password-of-user1',
     )
 
-    # đều được
-
 4.2 ``read_sql_file``
 '''''''''''''''''''''
 
 To get the SQL query from an SQL file, using the ``read_sql_file`` method, it has the following parameter:
 
 - ``sql_file_path`` (required): The located path of the SQL file. **(str)**
 
@@ -686,14 +714,16 @@
 
 - ``schema`` (required): The schema containing the table to upsert. **(str)**
 
 - ``table`` (required): The name of the table to upsert the data into. **(str)**
 
 - ``where_conditions`` (optional): A string of a query that uses conditions to update. The default value is ``None``. **(str)**
 
+- ``ignore_existence`` (optional): Whether to insert only new transactions and ignore existing transactions. The default value is ``False``. **(bool)**
+
 - ``commit_every`` (optional): The number of rows of data to commit each time. The default value is ``5000``. **(int)**
 
 - ``db_pool_conn`` (optional): The connection pool to connect to the database. The default value is ``None``. If the value is ``None``, a new connection will be created and automatically closed after being used. **(callable)**
 
 .. code-block:: python
 
     pg_utils.upsert_data(
@@ -711,17 +741,19 @@
 
 - ``schema`` (required): The schema containing the table to upsert. **(str)**
 
 - ``table`` (required): The name of the table to upsert the data into. **(str)**
 
 - ``where_conditions`` (optional): A string of a query that uses conditions to update. The default value is ``None``. **(str)**
 
+- ``ignore_existence`` (optional): Whether to insert only new transactions and ignore existing transactions. The default value is ``False``. **(bool)**
+
 - ``commit_every`` (optional): The number of rows of data to commit each time. The default value is ``5000``. **(int)**
 
-- ``db_pool_conn`` (optional): A connection pool to connect to the database. The default value is ``None``. If the value is ``None``, a new connection will be created and automatically closed after being used. **(callable)**
+- ``db_pool_conn`` (optional): The connection pool to connect to the database. The default value is ``None``. If the value is ``None``, a new connection will be created and automatically closed after being used. **(callable)**
 
 .. code-block:: python
 
     pg_utils.bulk_upsert_data(
         data=your_df,
         schema='your-schema',
         table='your-table',
@@ -967,16 +999,14 @@
 
 - ``list_users`` (optional): A list of users to grant access. The default value is ``None``. If ``None``, the table will be granted for all the predefined users. **(list)**
 
 - ``privileges`` (optional): A list of privileges to grant. The default value is ``['SELECT']``. Accepted values in the privileges list are: ``'SELECT'``, ``'INSERT'``, ``'UPDATE'``, ``'DELETE'``, ``'TRUNCATE'``, ``'REFERENCES'``, ``'TRIGGER'``. **(list)**
 
 - ``all_privileges`` (optional): Whether to grant all privileges. The default value is ``False``. **(bool)**
 
-- ``predefined_rules`` (optional): Whether to grant with the predefined rules. The default value is ``False``. **(bool)**
-
 .. code-block:: python
 
     pg_utils.auto_grant(
         schema='your-schema',
         list_tables=['your-new-table'],
         list_users=[
             'linhvk',
@@ -1109,30 +1139,209 @@
 Telegram
 ^^^^^^^^
 
 **Use case:** When need to send messages to Telegram by using bot
 
 **Functional:**
 
+5.1 ``send_message``
+'''''''''''''''''''''''''
+
 To send messages to Telegram, using ``send_message`` method, it has the following parameters:
 
 - ``text`` (required): Message to send. **(str)**
 
 - ``bot_token`` (optional): Token of the bot which send the message. The default value is ``None``. If the value is ``None``, the bot ``sleep at 9pm`` will be used to send messages. **(str)**
 
 - ``chat_id`` (optional): ID of group chat where the message is sent. The default value is ``None``. If the value is ``None``, the group chat ``Airflow Status Alert`` will be used. **(str)**
 
+- ``parse_mode`` (optional): Sending mode, the accepted value is ``Markdown`` or ``HTML``. The default value is ``Markdown``. **(str)**
+
 .. code-block:: python
 
     from sop_deutils.y4a_telegram import send_message
 
     send_message(
         text='Hello liuliukiki'
     )
 
+5.2 ``send_data``
+'''''''''''''''''''''''''
+
+To send data to Telegram, using ``send_data`` method, it has the following parameters:
+
+- ``data`` (required): Data to send. **(pd.DataFrame)**
+
+- ``title`` (optional): The title of the message. The default value is ``None``. **(str)**
+
+- ``bot_token`` (optional): Token of the bot which send the data. The default value is ``None``. If the value is ``None``, the bot ``sleep at 9pm`` will be used to send data. **(str)**
+
+- ``chat_id`` (optional): ID of group chat where the data is sent. The default value is ``None``. If the value is ``None``, the group chat ``Airflow Status Alert`` will be used. **(str)**
+
+- ``parse_mode`` (optional): Sending mode, the accepted value is ``Markdown`` or ``HTML``. The default value is ``Markdown``. **(str)**
+
+.. code-block:: python
+
+    from sop_deutils.y4a_telegram import send_data
+
+    send_data(
+        data=my_df,
+        title='Sample Data',
+    )
+
+--------------
+
+GoogleChat
+^^^^^^^^^^
+
+**Use case:** When need to send messages to Google Chat space by using bot
+
+**Functional:**
+
+6.1 ``send_message``
+'''''''''''''''''''''''''
+
+To send messages to chat space of Google, using ``send_message`` method, it has the following parameters:
+
+- ``webhook_url`` (required): Url of the webhook that is registered in the chat space. `How to create webhook <https://developers.google.com/chat/how-tos/webhooks#create_a_webhook>`__. **(str)**
+
+- ``message`` (required): The content to send to the chat space. **(str)**
+
+.. code-block:: python
+
+    from sop_deutils.gg_api.y4a_chat import send_message
+
+    send_message(
+        webhook_url=f'https://chat.googleapis.com/v1/spaces/{SPACE_ID}/messages?key={KEY}&token={TOKEN}'
+        message='Hello liuliukiki',
+    )
+
+6.2 ``send_data``
+'''''''''''''''''''''''''
+
+To send data to chat space of Google, using ``send_data`` method, it has the following parameters:
+
+- ``webhook_url`` (required): Url of the webhook that is registered in the chat space. `How to create webhook <https://developers.google.com/chat/how-tos/webhooks#create_a_webhook>`__. **(str)**
+
+- ``data`` (required): Data to send. **(pd.DataFrame)**
+
+- ``title`` (optional): The title of the message. The default value is ``None``. **(str)**
+
+.. code-block:: python
+
+    from sop_deutils.gg_api.y4a_chat import send_data
+
+    send_data(
+        webhook_url=f'https://chat.googleapis.com/v1/spaces/{SPACE_ID}/messages?key={KEY}&token={TOKEN}'
+        data=my_df,
+        title='Sample Data',
+    )
+
+--------------
+
+GoogleMail
+^^^^^^^^^^
+
+**Use case:** when need to send email to group of people.
+
+**Functional:**
+
+7.1 initialize
+''''''''''''''
+
+Firstly, import GGMail utils module class. This class has two parameters:
+
+- ``sender_email``: The email of sender. The default value is ``None``. If not provide, the email of DA team will be used. **(str)**
+- ``sender_password``: The password email of sender. The default value is ``None``. If not provide, the email of DA team will be used. **(str)**
+
+.. code-block:: python
+
+    from sop_deutils.gg_api.y4a_mail import GGMailUtils
+
+    mail_utils = GGMailUtils() # This utils will use email of DA team
+
+    # or
+
+    mail_utils = GGMailUtils(
+        sender_email='user@domain.abc',
+        sender_password='something',
+    )
+
+7.2 ``send_mail``
+'''''''''''''''''''''
+
+To send plain text email, using the ``send_mail`` method, it has the following parameter:
+
+- ``receiver_email`` (required): List of people to receive email. **(list)**
+
+- ``content`` (required): The content of email. **(str)**
+
+- ``cc_email`` (optional): List of people to receive CC. The default value is ``None``. **(list)**
+
+- ``subject`` (optional): The subject of email. The default value is ``None``. **(str)**
+
+.. code-block:: python
+
+    mail_utils.send_mail(
+        receiver_email=['user1@domain.abc', 'user2@domain.abc'],
+        content='j ai biec',
+    )
+
+7.3 ``send_mail_w_attachments``
+'''''''''''''''''''''''''''''''''''
+
+To send email with attachments, using the ``send_mail_w_attachments`` method, it has the following parameters:
+
+- ``receiver_email`` (required): List of people to receive email. **(list)**
+
+- ``content`` (required): The content of email. **(str)**
+
+- ``attachment_path`` (required): List of file path to attach. **(list)**
+
+- ``cc_email`` (optional): List of people to receive CC. The default value is ``None``. **(list)**
+
+- ``subject`` (optional): The subject of email. The default value is ``None``. **(str)**
+
+.. code-block:: python
+
+    mail_utils.send_mail_w_attachments(
+        receiver_email=['user1@domain.abc', 'user2@domain.abc'],
+        content='j ai biec',
+        attachment_path=['parent_dir/file1.xlsx', 'parent_dir/file2.xlsx'],
+    )
+
+7.4 ``send_mail_w_pandas_df``
+''''''''''''''''''''''''''''''''''
+
+To send email with pandas dataframe as Excel file to group of people, using the ``send_mail_w_pandas_df`` method, it has the following parameters:
+
+- ``receiver_email`` (required): List of people to receive email. **(list)**
+
+- ``content`` (required): The content of email. **(str)**
+
+- ``data_list`` (required): List of dataframe to attach. **(list)**
+
+- ``file_name`` (required): List of file name respectively to list of dataframe. Notes that each file name must contain ``.xlsx``.  **(list)**
+
+- ``cc_email`` (optional): List of people to receive CC. The default value is ``None``. **(list)**
+
+- ``subject`` (optional): The subject of email. The default value is ``None``. **(str)**
+
+.. code-block:: python
+
+    df1 = pd.DataFrame([1, 2, 3], columns=['d1'])
+    df2 = pd.DataFrame([4, 5, 6], columns=['d2'])
+
+    mail_utils.send_mail_w_pandas_df(
+        receiver_email=['user1@domain.abc', 'user2@domain.abc'],
+        content='j ai biec',
+        data_list=[df1, df2],
+        file_name=['data1.xlsx', 'data2.xlsx'],
+    )
+
 --------------
 
 All in one (DAConfig)
 ^^^^^^^^^^^^^^^^^^^^^
 
 **Use case:** So far, there are a lot of platforms that needs to access frequently, in order not to import lots of modules, users can inherit all of above modules as simplest way.
 
@@ -1300,11 +1509,16 @@
                 >>  etl_from_sheet_to_db(spread_sheet_id) \
                     >> execute_query()
 
 --------------
 
    provided by ``liuliukiki``
 
-..
+--------------
+
+   ``hinh anh users feedback thu vien kieu``
 
-   and special thank to ``duiikha`` for contributing api method to get
-   and secure account credentials.
+
+.. image::
+   https://lh3.googleusercontent.com/drive-viewer/AKGpihbUbW3ahIwUoCZq72pzvL8LVxRw-SkAzoYjsvg6pUY_hp6LSoklWol3oPSDPTb-Ny9kY8U1lY8pw3lFAYvjFUtfRI_6S8toISk=s1600-rw-v1
+   :scale: 44%
+   :alt: DA team
```

### Comparing `sop_deutils-0.9.9/README.rst` & `sop_deutils-1.0.0.dev0/sop_deutils.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,27 @@
+Metadata-Version: 2.1
+Name: sop_deutils
+Version: 1.0.0.dev0
+Summary: A utils package for Yes4All SOP
+Author-email: liuliukiki aka clong aka ifyouknowyouknow101 <longnc@yes4all.com>
+Project-URL: Author_Github, https://github.com/dribblewithclong
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 Yes4All SOP Utils Packages
 ==========================
 
 This is a utils package served for SOP Data Analytics team at **Yes4All**. It contains various modules to work with **PostgreSQL, MinIO, Google API, Airflow, Telegram…**
 
 .. image::
-   https://lh3.googleusercontent.com/drive-viewer/AK7aPaASSw5LzlIMog6XonAGba7CsmObYVMzQLzxMeBMFTuK30MCmuvB9ZOR-9VCq47rQpdgou849BL-oj5cufSECqxuE67c_w=s1600
+   https://lh3.googleusercontent.com/drive-viewer/AKGpihbzwqCnULTRFR1ihxbk2jwhfwhVfiZWGLfZ2W1argxs96TxMzfRTfaGgNQoL7NALlz94lMLrQnoK2y3jgOxh7raeq2rKJzU5sQ=s1600-rw-v1
    :scale: 20%
    :alt: liuliukiki
 
 --------------
 
 Contents Overview
 -----------------
@@ -234,14 +247,18 @@
 
 - ``sheet_name`` (optional): Worksheet name. The default value is ``'Sheet1'``. **(str)**
 
 - ``from_row_index`` (optional): The index of the row from which to begin inserting. The default value is ``1``. **(int)**
 
 - ``insert_column_names`` (optional): Whether to insert column names. The default value is ``False``. **(bool)**
 
+- ``parse_input`` (optional): Whether to parse input values as if the user typed them into the UI. The default value is ``True``. **(bool)**
+
+- ``pre_process`` (optional): Whether to process input based on the pre-defined function of DA. The default value is ``True``. **(bool)**
+
 .. code-block:: python
 
     sheet_utils.insert_data(
         data=df,
         sheet_id='your-sheet-id',
         from_row_index=2,
         insert_column_names=False,
@@ -256,14 +273,18 @@
 
 - ``sheet_id`` (required): Spreadsheet ID. **(str)**
 
 - ``sheet_name`` (optional): Worksheet name. The default value is ``'Sheet1'``. **(str)**
 
 - ``range_from`` (optional): The beginning of the range of data to update. The default value is ``'A1'``. **(str)**
 
+- ``parse_input`` (optional): Whether to parse input values as if the user typed them into the UI. The default value is ``True``. **(bool)**
+
+- ``pre_process`` (optional): Whether to process input based on the pre-defined function of DA. The default value is ``True``. **(bool)**
+
 .. code-block:: python
 
     sheet_utils.update_data(
         data=new_df,
         sheet_id='your-sheet-id',
         range_from='A4',
     )
@@ -364,27 +385,64 @@
 
 .. code-block:: python
 
     ss = sheet_utils.open_spread_sheet(
         sheet_id='your-sheet-id',
     )
 
+2.14 ``gspread_load_data``
+''''''''''''''''''''''''''''''''''''''
+
+To load data to the given sheet, using ``gspread_load_data`` method. This method is integrated with GSpread load data function that provides the high efficiency and convenience, it can be used as the alternative of two methods ``insert_data`` and ``update_data``, it has the following parameters:
+
+- ``data`` (required): Dataframe containing data to load. **(pd.DataFrame)**
+
+- ``sheet_id`` (required): Spreadsheet ID. **(str)**
+
+- ``sheet_name`` (optional): Worksheet name. The default value is ``'Sheet1'``. **(str)**
+
+- ``from_row`` (optional): Row at which to start loading the DataFrame. The default value is ``1``. **(int)**
+
+- ``from_col`` (optional): Column at which to start loading the DataFrame. The default value is ``1``. **(int)**
+
+- ``include_index`` (optional): Whether to include the DataFrame's index as an additional column. The default value is ``False``. **(bool)**
+
+- ``include_column`` (optional): Whether to add a header row or rows before data with column names (if include_index is True, the index's name(s) will be used as its columns' headers). The default value is ``True``. **(bool)**
+
+- ``resize_worksheet`` (optional): If True, changes the worksheet's size to match the shape of the provided DataFrame, if False, worksheet will only be resized as necessary to contain the DataFrame contents. The default value is ``False``. **(bool)**
+
+- ``allow_formulas`` (optional): Whether to interprets ``=foo`` as a formula in cell values; otherwise all text beginning with ``=`` is escaped to avoid its interpretation as a formula. The default value is ``True``. **(bool)**
+
+- ``string_escaping`` (optional): Determines when string values are escaped as text literals (by adding an initial ``'`` character) in requests to Sheets API, 3 parameter values are accepted: ('default': only escape strings starting with a literal ``'`` character. 'off': escape nothing; cell values starting with a ``'`` will be interpreted by sheets as an escape character followed by a text literal. 'full': escape all string values), the escaping done when allow_formulas=False (escaping string values beginning with ``=``) is unaffected by this parameter's value. The default value is ``'default'``. **(str)**
+
+.. code-block:: python
+
+    sheet_utils.gspread_load_data(
+        data=df,
+        sheet_id='your-sheet-id',
+        sheet_name='Sheet1',
+        from_row=3,
+        from_col=4,
+        include_index=True,
+        include_column=True,
+    )
+
 --------------
 
 MinIO
 ^^^^^
 
 MinIO is an object storage, it is API compatible with the Amazon S3 cloud storage service. MinIO can be used as a **datalake** to store unstructured data (photos, videos, log files, backups, and container images) and structured data.
 
 **Use case:** when need to store raw data or get raw data from datalake. Notes that the stored data extension must be ``.parquet`` .
 
 **Notes about how to determine the** ``file_path`` **parameter in minIO when using this module:**
 
 .. figure::
-   https://lh3.googleusercontent.com/drive-viewer/AEYmBYTeW1mCFR9M_cI4vg_bRRaLUVVxPtvkoWenEecrXSbmju3Xujj8jMI_MgiGBn-F5ozkkDPAWLPATwZ8JtdkciDopAaf=s1600
+   https://lh3.googleusercontent.com/drive-viewer/AEYmBYTnHBUSHkf9nTE9TuXWpEh12YMfUvHp2If3pJnjiRlmw6kdhqPrrprI-zMmdgM4O5pvSR8q1u5m5-XNRCo4Mc4rKJ-J=s1600
    :alt: minIO file path
 
 ..
 
    For example, if the directory to the data file in minIO is as above, then the ``file_path`` is ``"/scraping/amazon_vendor/avc_bulk_buy_request/2023/9/24/batch_1695525619"`` (after removing bucket name, data storage mode, and data file extension).
 
 **Functional:**
@@ -572,16 +630,14 @@
 
     pg_utils = PostgreSQLUtils(
         pg_name='serving_master',
         pg_account='y4a_sop_user1',
         pg_password='password-of-user1',
     )
 
-    # đều được
-
 4.2 ``read_sql_file``
 '''''''''''''''''''''
 
 To get the SQL query from an SQL file, using the ``read_sql_file`` method, it has the following parameter:
 
 - ``sql_file_path`` (required): The located path of the SQL file. **(str)**
 
@@ -658,14 +714,16 @@
 
 - ``schema`` (required): The schema containing the table to upsert. **(str)**
 
 - ``table`` (required): The name of the table to upsert the data into. **(str)**
 
 - ``where_conditions`` (optional): A string of a query that uses conditions to update. The default value is ``None``. **(str)**
 
+- ``ignore_existence`` (optional): Whether to insert only new transactions and ignore existing transactions. The default value is ``False``. **(bool)**
+
 - ``commit_every`` (optional): The number of rows of data to commit each time. The default value is ``5000``. **(int)**
 
 - ``db_pool_conn`` (optional): The connection pool to connect to the database. The default value is ``None``. If the value is ``None``, a new connection will be created and automatically closed after being used. **(callable)**
 
 .. code-block:: python
 
     pg_utils.upsert_data(
@@ -683,17 +741,19 @@
 
 - ``schema`` (required): The schema containing the table to upsert. **(str)**
 
 - ``table`` (required): The name of the table to upsert the data into. **(str)**
 
 - ``where_conditions`` (optional): A string of a query that uses conditions to update. The default value is ``None``. **(str)**
 
+- ``ignore_existence`` (optional): Whether to insert only new transactions and ignore existing transactions. The default value is ``False``. **(bool)**
+
 - ``commit_every`` (optional): The number of rows of data to commit each time. The default value is ``5000``. **(int)**
 
-- ``db_pool_conn`` (optional): A connection pool to connect to the database. The default value is ``None``. If the value is ``None``, a new connection will be created and automatically closed after being used. **(callable)**
+- ``db_pool_conn`` (optional): The connection pool to connect to the database. The default value is ``None``. If the value is ``None``, a new connection will be created and automatically closed after being used. **(callable)**
 
 .. code-block:: python
 
     pg_utils.bulk_upsert_data(
         data=your_df,
         schema='your-schema',
         table='your-table',
@@ -939,16 +999,14 @@
 
 - ``list_users`` (optional): A list of users to grant access. The default value is ``None``. If ``None``, the table will be granted for all the predefined users. **(list)**
 
 - ``privileges`` (optional): A list of privileges to grant. The default value is ``['SELECT']``. Accepted values in the privileges list are: ``'SELECT'``, ``'INSERT'``, ``'UPDATE'``, ``'DELETE'``, ``'TRUNCATE'``, ``'REFERENCES'``, ``'TRIGGER'``. **(list)**
 
 - ``all_privileges`` (optional): Whether to grant all privileges. The default value is ``False``. **(bool)**
 
-- ``predefined_rules`` (optional): Whether to grant with the predefined rules. The default value is ``False``. **(bool)**
-
 .. code-block:: python
 
     pg_utils.auto_grant(
         schema='your-schema',
         list_tables=['your-new-table'],
         list_users=[
             'linhvk',
@@ -1081,30 +1139,209 @@
 Telegram
 ^^^^^^^^
 
 **Use case:** When need to send messages to Telegram by using bot
 
 **Functional:**
 
+5.1 ``send_message``
+'''''''''''''''''''''''''
+
 To send messages to Telegram, using ``send_message`` method, it has the following parameters:
 
 - ``text`` (required): Message to send. **(str)**
 
 - ``bot_token`` (optional): Token of the bot which send the message. The default value is ``None``. If the value is ``None``, the bot ``sleep at 9pm`` will be used to send messages. **(str)**
 
 - ``chat_id`` (optional): ID of group chat where the message is sent. The default value is ``None``. If the value is ``None``, the group chat ``Airflow Status Alert`` will be used. **(str)**
 
+- ``parse_mode`` (optional): Sending mode, the accepted value is ``Markdown`` or ``HTML``. The default value is ``Markdown``. **(str)**
+
 .. code-block:: python
 
     from sop_deutils.y4a_telegram import send_message
 
     send_message(
         text='Hello liuliukiki'
     )
 
+5.2 ``send_data``
+'''''''''''''''''''''''''
+
+To send data to Telegram, using ``send_data`` method, it has the following parameters:
+
+- ``data`` (required): Data to send. **(pd.DataFrame)**
+
+- ``title`` (optional): The title of the message. The default value is ``None``. **(str)**
+
+- ``bot_token`` (optional): Token of the bot which send the data. The default value is ``None``. If the value is ``None``, the bot ``sleep at 9pm`` will be used to send data. **(str)**
+
+- ``chat_id`` (optional): ID of group chat where the data is sent. The default value is ``None``. If the value is ``None``, the group chat ``Airflow Status Alert`` will be used. **(str)**
+
+- ``parse_mode`` (optional): Sending mode, the accepted value is ``Markdown`` or ``HTML``. The default value is ``Markdown``. **(str)**
+
+.. code-block:: python
+
+    from sop_deutils.y4a_telegram import send_data
+
+    send_data(
+        data=my_df,
+        title='Sample Data',
+    )
+
+--------------
+
+GoogleChat
+^^^^^^^^^^
+
+**Use case:** When need to send messages to Google Chat space by using bot
+
+**Functional:**
+
+6.1 ``send_message``
+'''''''''''''''''''''''''
+
+To send messages to chat space of Google, using ``send_message`` method, it has the following parameters:
+
+- ``webhook_url`` (required): Url of the webhook that is registered in the chat space. `How to create webhook <https://developers.google.com/chat/how-tos/webhooks#create_a_webhook>`__. **(str)**
+
+- ``message`` (required): The content to send to the chat space. **(str)**
+
+.. code-block:: python
+
+    from sop_deutils.gg_api.y4a_chat import send_message
+
+    send_message(
+        webhook_url=f'https://chat.googleapis.com/v1/spaces/{SPACE_ID}/messages?key={KEY}&token={TOKEN}'
+        message='Hello liuliukiki',
+    )
+
+6.2 ``send_data``
+'''''''''''''''''''''''''
+
+To send data to chat space of Google, using ``send_data`` method, it has the following parameters:
+
+- ``webhook_url`` (required): Url of the webhook that is registered in the chat space. `How to create webhook <https://developers.google.com/chat/how-tos/webhooks#create_a_webhook>`__. **(str)**
+
+- ``data`` (required): Data to send. **(pd.DataFrame)**
+
+- ``title`` (optional): The title of the message. The default value is ``None``. **(str)**
+
+.. code-block:: python
+
+    from sop_deutils.gg_api.y4a_chat import send_data
+
+    send_data(
+        webhook_url=f'https://chat.googleapis.com/v1/spaces/{SPACE_ID}/messages?key={KEY}&token={TOKEN}'
+        data=my_df,
+        title='Sample Data',
+    )
+
+--------------
+
+GoogleMail
+^^^^^^^^^^
+
+**Use case:** when need to send email to group of people.
+
+**Functional:**
+
+7.1 initialize
+''''''''''''''
+
+Firstly, import GGMail utils module class. This class has two parameters:
+
+- ``sender_email``: The email of sender. The default value is ``None``. If not provide, the email of DA team will be used. **(str)**
+- ``sender_password``: The password email of sender. The default value is ``None``. If not provide, the email of DA team will be used. **(str)**
+
+.. code-block:: python
+
+    from sop_deutils.gg_api.y4a_mail import GGMailUtils
+
+    mail_utils = GGMailUtils() # This utils will use email of DA team
+
+    # or
+
+    mail_utils = GGMailUtils(
+        sender_email='user@domain.abc',
+        sender_password='something',
+    )
+
+7.2 ``send_mail``
+'''''''''''''''''''''
+
+To send plain text email, using the ``send_mail`` method, it has the following parameter:
+
+- ``receiver_email`` (required): List of people to receive email. **(list)**
+
+- ``content`` (required): The content of email. **(str)**
+
+- ``cc_email`` (optional): List of people to receive CC. The default value is ``None``. **(list)**
+
+- ``subject`` (optional): The subject of email. The default value is ``None``. **(str)**
+
+.. code-block:: python
+
+    mail_utils.send_mail(
+        receiver_email=['user1@domain.abc', 'user2@domain.abc'],
+        content='j ai biec',
+    )
+
+7.3 ``send_mail_w_attachments``
+'''''''''''''''''''''''''''''''''''
+
+To send email with attachments, using the ``send_mail_w_attachments`` method, it has the following parameters:
+
+- ``receiver_email`` (required): List of people to receive email. **(list)**
+
+- ``content`` (required): The content of email. **(str)**
+
+- ``attachment_path`` (required): List of file path to attach. **(list)**
+
+- ``cc_email`` (optional): List of people to receive CC. The default value is ``None``. **(list)**
+
+- ``subject`` (optional): The subject of email. The default value is ``None``. **(str)**
+
+.. code-block:: python
+
+    mail_utils.send_mail_w_attachments(
+        receiver_email=['user1@domain.abc', 'user2@domain.abc'],
+        content='j ai biec',
+        attachment_path=['parent_dir/file1.xlsx', 'parent_dir/file2.xlsx'],
+    )
+
+7.4 ``send_mail_w_pandas_df``
+''''''''''''''''''''''''''''''''''
+
+To send email with pandas dataframe as Excel file to group of people, using the ``send_mail_w_pandas_df`` method, it has the following parameters:
+
+- ``receiver_email`` (required): List of people to receive email. **(list)**
+
+- ``content`` (required): The content of email. **(str)**
+
+- ``data_list`` (required): List of dataframe to attach. **(list)**
+
+- ``file_name`` (required): List of file name respectively to list of dataframe. Notes that each file name must contain ``.xlsx``.  **(list)**
+
+- ``cc_email`` (optional): List of people to receive CC. The default value is ``None``. **(list)**
+
+- ``subject`` (optional): The subject of email. The default value is ``None``. **(str)**
+
+.. code-block:: python
+
+    df1 = pd.DataFrame([1, 2, 3], columns=['d1'])
+    df2 = pd.DataFrame([4, 5, 6], columns=['d2'])
+
+    mail_utils.send_mail_w_pandas_df(
+        receiver_email=['user1@domain.abc', 'user2@domain.abc'],
+        content='j ai biec',
+        data_list=[df1, df2],
+        file_name=['data1.xlsx', 'data2.xlsx'],
+    )
+
 --------------
 
 All in one (DAConfig)
 ^^^^^^^^^^^^^^^^^^^^^
 
 **Use case:** So far, there are a lot of platforms that needs to access frequently, in order not to import lots of modules, users can inherit all of above modules as simplest way.
 
@@ -1272,11 +1509,16 @@
                 >>  etl_from_sheet_to_db(spread_sheet_id) \
                     >> execute_query()
 
 --------------
 
    provided by ``liuliukiki``
 
-..
+--------------
+
+   ``hinh anh users feedback thu vien kieu``
 
-   and special thank to ``duiikha`` for contributing api method to get
-   and secure account credentials.
+
+.. image::
+   https://lh3.googleusercontent.com/drive-viewer/AKGpihbUbW3ahIwUoCZq72pzvL8LVxRw-SkAzoYjsvg6pUY_hp6LSoklWol3oPSDPTb-Ny9kY8U1lY8pw3lFAYvjFUtfRI_6S8toISk=s1600-rw-v1
+   :scale: 44%
+   :alt: DA team
```

### Comparing `sop_deutils-0.9.9/sop_deutils/base/y4a_da_cfg.py` & `sop_deutils-1.0.0.dev0/sop_deutils/base/y4a_da_cfg.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-0.9.9/sop_deutils/datalake/y4a_minio.py` & `sop_deutils-1.0.0.dev0/sop_deutils/datalake/y4a_minio.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-0.9.9/sop_deutils/gg_api/y4a_sheet.py` & `sop_deutils-1.0.0.dev0/sop_deutils/gg_api/y4a_sheet.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 import logging
 import warnings
 from typing import Callable
 import pandas as pd
 import gspread
+from gspread_dataframe import set_with_dataframe
 from ..y4a_retry import retry_on_error
 from ..y4a_credentials import get_credentials
 
 warnings.filterwarnings("ignore", category=UserWarning)
 
 logging.basicConfig(
     level=logging.INFO,
@@ -409,83 +410,115 @@
     def insert_data(
         self,
         data: pd.DataFrame,
         sheet_id: str,
         sheet_name: str = 'Sheet1',
         from_row_index: int = 1,
         insert_column_names: bool = False,
+        parse_input: bool = True,
+        pre_process: bool = True,
     ) -> None:
         """
         Insert data to the given sheet
 
         :param data: dataframe contains data to insert
         :param sheet_id: spreadsheet id
         :param sheet_name: worksheet name
             defaults to 'Sheet1'
         :param from_row_index: the index of the row
             beginning to insert
             defaults to 1
         :param insert_column_names: whether to insert column names
             defaults to False
+        :param parse_input: whether to parse input values
+            as if the user typed them into the UI
+            defaults to True
+        :param pre_process: whether to process input values
+            based on the pre-defined function of DA
+            defaults to True
         """
 
         spread_sheet = self.open_spread_sheet(sheet_id)
 
         work_sheet = self.get_work_sheet(
             spread_sheet=spread_sheet,
             sheet_name=sheet_name,
         )
 
-        constructed_data = self.construct_data(data)
+        input_option = 'RAW'
+        if parse_input:
+            input_option = 'USER_ENTERED'
+
+        if pre_process:
+            constructed_data = self.construct_data(data)
+        else:
+            constructed_data = data.copy()
         data_values = constructed_data.values.tolist()
 
         if insert_column_names:
             col_values = [data.columns.to_list()]
             work_sheet.insert_rows(
                 col_values,
                 row=from_row_index,
             )
             work_sheet.insert_rows(
                 data_values,
                 row=from_row_index+1,
+                value_input_option=input_option,
             )
         else:
             work_sheet.insert_rows(
                 data_values,
                 row=from_row_index,
+                value_input_option=input_option,
             )
 
     @retry_on_error(delay=30)
     def update_data(
         self,
         data: pd.DataFrame,
         sheet_id: str,
         sheet_name: str = 'Sheet1',
         range_from: str = 'A1',
+        parse_input: bool = True,
+        pre_process: bool = True,
     ) -> None:
         """
         Update data of the given sheet
 
         :param data: dataframe contains data to update
         :param sheet_id: spreadsheet name
         :param sheet_name: worksheet name
             defaults to 'Sheet1'
         :param range_from: the begining of the range
             of data from sheet to update
             defaults to 'A1'
+        :param parse_input: whether to parse input values
+            as if the user typed them into the UI
+            defaults to True
+        :param pre_process: whether to process input values
+            based on the pre-defined function of DA
+            defaults to True
         """
 
         spread_sheet = self.open_spread_sheet(sheet_id)
 
         work_sheet = self.get_work_sheet(
             spread_sheet=spread_sheet,
             sheet_name=sheet_name,
         )
 
-        constructed_data = self.construct_data(data)
+        input_option = 'RAW'
+        if parse_input:
+            input_option = 'USER_ENTERED'
+
+        if pre_process:
+            constructed_data = self.construct_data(data)
+        else:
+            constructed_data = data.copy()
         data_values = constructed_data.values.tolist()
 
         num_current_rows = work_sheet.row_count
         num_current_cols = work_sheet.col_count
 
         range_from_index = gspread.utils.a1_to_rowcol(range_from)
         row_from_index = range_from_index[0]
@@ -505,14 +538,98 @@
             rows=rows_to_resize,
             cols=cols_to_resize,
         )
 
         work_sheet.update(
             f'{range_from}',
             data_values,
+            value_input_option=input_option,
+        )
+
+    @retry_on_error(delay=30)
+    def gspread_load_data(
+        self,
+        data: pd.DataFrame,
+        sheet_id: str,
+        sheet_name: str = 'Sheet1',
+        from_row: int = 1,
+        from_col: int = 1,
+        include_index: bool = False,
+        include_column: bool = True,
+        resize_worksheet: bool = False,
+        allow_formulas: bool = True,
+        string_escaping: str = 'default',
+    ) -> None:
+        """
+        Load data to the given sheet. This method
+        is integrated with GSpread load data function
+        that provides the high efficiency and convenience,
+        it can be used as the alternative of two methods
+        'insert_data' and 'update_data'
+
+        :param data: dataframe contains data to load
+        :param sheet_id: spreadsheet name
+        :param sheet_name: worksheet name
+            defaults to 'Sheet1'
+        :param from_row: row at which to start loading the DataFrame
+            defaults to 1
+        :param from_col: column at which to start loading the DataFrame
+            defaults to 1
+        :param include_index: if True, include the DataFrame's index as an
+            additional column
+            defaults to False
+        :param include_column: if True, add a header row or rows before data
+            with column names (if include_index is True, the index's name(s)
+            will be used as its columns' headers)
+            defaults to True
+        :param resize_worksheet: if True, changes the worksheet's
+            size to match the shape of the provided DataFrame,
+            if False, worksheet will only be
+            resized as necessary to contain the DataFrame contents
+            defaults to False
+        :param allow_formulas: if True, interprets `=foo` as a formula in
+            cell values; otherwise all text beginning with `=` is escaped
+            to avoid its interpretation as a formula
+            defaults to True
+        :param string_escaping: determines when string values are
+            escaped as text literals (by adding an initial `'` character)
+            in requests to Sheets API
+            4 parameter values are accepted:
+            - 'default': only escape strings starting with a literal `'`
+                character
+            - 'off': escape nothing; cell values starting with a `'` will be
+                interpreted by sheets as an escape character followed by
+                a text literal
+            - 'full': escape all string values
+            - any callable object: will be called once for each cell's string
+                value; if return value is true, string will be escaped
+                with preceding `'` (A useful technique is to pass a
+                regular expression bound method, e.g.
+                `re.compile(r'^my_regex_.*$').search`.)
+            the escaping done when allow_formulas=False (escaping string values
+            beginning with `=`) is unaffected by this parameter's value
+            defaults to 'default'
+        """
+
+        spreadsheet = self.open_spread_sheet(sheet_id)
+        worksheet = self.get_work_sheet(
+            spreadsheet,
+            sheet_name,
+        )
+
+        set_with_dataframe(
+            worksheet=worksheet,
+            dataframe=data,
+            row=from_row,
+            col=from_col,
+            include_index=include_index,
+            include_column_header=include_column,
+            resize=resize_worksheet,
+            allow_formulas=allow_formulas,
+            string_escaping=string_escaping,
         )
 
     @retry_on_error(delay=30)
     def remove_data(
         self,
         sheet_id: str,
         sheet_name: str = 'Sheet1',
```

### Comparing `sop_deutils-0.9.9/sop_deutils/sql/y4a_monitor_user.py` & `sop_deutils-1.0.0.dev0/sop_deutils/sql/y4a_monitor_user.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 import logging
+import hashlib
 import pytz
 import warnings
 import pandas as pd
 from psycopg2 import connect
 from ..y4a_credentials import get_credentials
 
 logging.basicConfig(
@@ -31,25 +32,36 @@
         self.conn_number = conn_number
 
         self.log_conn_df = pd.DataFrame(
             {
                 'time_conn': str(
                     datetime.datetime.now(
                         pytz.timezone('Asia/Ho_Chi_Minh'),
-                    ).replace(microsecond=0).replace(tzinfo=None)
+                    ).replace(tzinfo=None)
                 ),
                 'host': self.conn_host,
                 'username': self.conn_username,
                 'password': self.conn_password,
                 'database': self.conn_db,
                 'num_conn': self.conn_number,
             },
             index=[0],
         )
 
+    def id_gen(
+        self,
+        value: str,
+    ) -> str:
+        sha256 = hashlib.sha256()
+        sha256.update(
+            value.encode()
+        )
+
+        return sha256.hexdigest()
+
     def execute(
         self,
         sql: str,
         vars: tuple = None,
         fetch_output: bool = False,
     ) -> list:
         output = None
@@ -81,39 +93,66 @@
         except Exception as e:
             logging.error(e)
             conn.close()
 
         return output
 
     def generate_log_conn(self) -> None:
-        sql = "INSERT INTO y4a_sop.monitor_user_sql_connection "
-        sql += "(time_conn, host, username, database, num_conn) "
-        sql += f"VALUES ('{self.log_conn_df['time_conn'].values[0]}', "
-        sql += f"'{self.log_conn_df['host'].values[0]}', "
-        sql += f"'{self.log_conn_df['username'].values[0]}', "
+        time_conn = self.log_conn_df['time_conn'].values[0]
+        host = self.log_conn_df['host'].values[0]
+        username = self.log_conn_df['username'].values[0]
+        id_log = self.id_gen(
+            '_'.join(
+                [
+                    time_conn,
+                    host,
+                    username,
+                ]
+            )
+        )
+        sql = "INSERT INTO y4a_sop.pg_user_sql_connection "
+        sql += "(time_conn, host, username, id, database, num_conn) "
+        sql += f"VALUES ('{time_conn}', "
+        sql += f"'{host}', "
+        sql += f"'{username}', "
+        sql += f"'{id_log}', "
         sql += f"'{self.log_conn_df['database'].values[0]}', "
         sql += f"{self.log_conn_df['num_conn'].values[0]}) "
 
         self.execute(
             sql=sql,
             fetch_output=False,
         )
 
     def generate_log_query(
         self,
         sql_query: str,
         duration_query: float,
         is_successed: int,
     ) -> None:
-        sql = "INSERT INTO y4a_sop.monitor_user_sql_query "
-        sql += "(time_query, host, username, database, "
+        time_conn = self.log_conn_df['time_conn'].values[0]
+        host = self.log_conn_df['host'].values[0]
+        username = self.log_conn_df['username'].values[0]
+        id_log = self.id_gen(
+            '_'.join(
+                [
+                    time_conn,
+                    host,
+                    username,
+                    sql_query,
+                ]
+            )
+        )
+        sql = "INSERT INTO y4a_sop.pg_user_sql_query "
+        sql += "(time_query, host, username, id, database, "
         sql += "sql_query, duration, is_successed) "
-        sql += f"VALUES ('{self.log_conn_df['time_conn'].values[0]}', "
-        sql += f"'{self.log_conn_df['host'].values[0]}', "
-        sql += f"'{self.log_conn_df['username'].values[0]}', "
+        sql += f"VALUES ('{time_conn}', "
+        sql += f"'{host}', "
+        sql += f"'{username}', "
+        sql += f"'{id_log}', "
         sql += f"'{self.log_conn_df['database'].values[0]}', "
         sql += "%s, "
         sql += f"{duration_query}, "
         sql += f"{is_successed}) "
 
         self.execute(
             sql=sql,
```

### Comparing `sop_deutils-0.9.9/sop_deutils/sql/y4a_mysql.py` & `sop_deutils-1.0.0.dev0/sop_deutils/sql/y4a_mysql.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-0.9.9/sop_deutils/sql/y4a_postgresql.py` & `sop_deutils-1.0.0.dev0/sop_deutils/sql/y4a_postgresql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 import time
 import datetime
 import warnings
-import requests
 from functools import reduce
 from itertools import product
 from typing import Callable
 import pandas as pd
 import numpy as np
 from sqlalchemy import create_engine
 from psycopg2 import connect
@@ -75,26 +74,20 @@
         """
         Create a new connection to PostgreSQL
 
         :return: connection object to connect to database
         """
 
         if self.account_name:
-            try:
-                credentials = get_credentials(
-                    platform='pg',
-                    account_name=self.account_name,
-                )
-                db_user = credentials['user_name']
-                db_password = credentials['password']
-            except Exception:
-                logging.error('Failed to get account credentials from minIO')
-                logging.info('Try using backup account')
-                db_user = 'y4a_sop_af_trino'
-                db_password = 'FJ!dlskjd0912lkjsd'
+            credentials = get_credentials(
+                platform='pg',
+                account_name=self.account_name,
+            )
+            db_user = credentials['user_name']
+            db_password = credentials['password']
         else:
             db_user = self.pg_account
             db_password = self.pg_password
 
         conn = connect(
             user=db_user,
             password=db_password,
@@ -477,26 +470,30 @@
 
     def upsert_data(
         self,
         data: pd.DataFrame,
         schema: str,
         table: str,
         where_conditions: str = None,
+        ignore_existence: bool = False,
         commit_every: int = 5000,
         db_pool_conn: Callable = None,
     ) -> None:
         """
         Upsert data (update the row if it already exist when inserting)
             to PostgreSQL table
 
         :param data: a dataframe contains data to upsert
         :param schema: schema contains table to upsert
         :param table: table name to upsert
         :param where_conditions: string of query that use conditions to update
             defaults to None
+        :param ignore_existence: whether to insert only new transactions
+            and ignore existing transactions
+            defaults to False
         :param commit_every: number rows of data to commit each time
             defaults to 5000
         :param db_pool_conn: connection pool contains multiple connections
             to connect to database
             defaults to None
             if None, a new connection will be created and automatically closed
             after being used
@@ -573,18 +570,21 @@
                 sql += "{0} {1} VALUES ({2})".format(
                     f'{schema}.{table}',
                     target_fields,
                     ",".join(placeholders)
                 )
                 sql += " ON CONFLICT "
                 sql += f"({', '.join(primary_keys)}) "
-                sql += "DO UPDATE SET "
-                sql += f"{', '.join(to_update_columns_sql)}"
-                if where_conditions:
-                    sql += f" WHERE {where_conditions}"
+                if ignore_existence:
+                    sql += "DO NOTHING"
+                else:
+                    sql += "DO UPDATE SET "
+                    sql += f"{', '.join(to_update_columns_sql)}"
+                    if where_conditions:
+                        sql += f" WHERE {where_conditions}"
 
                 cur.execute(sql, values)
                 if i % commit_every == 0:
                     conn.commit()
                     logging.info(
                         f"Loaded {i} into {table} rows so far"
                     )
@@ -629,27 +629,31 @@
 
     def bulk_upsert_data(
         self,
         data: pd.DataFrame,
         schema: str,
         table: str,
         where_conditions: str = None,
+        ignore_existence: bool = False,
         commit_every: int = 5000,
         db_pool_conn: Callable = None,
     ) -> None:
         """
         Upsert data (update the row if it already exist when inserting)
             to PostgreSQL table using COPY method
             (using when the data to uspert is large)
 
         :param data: a dataframe contains data to upsert
         :param schema: schema contains table to upsert
         :param table: table name to upsert
         :param where_conditions: string of query that use conditions to update
             defaults to None
+        :param ignore_existence: whether to insert only new transactions
+            and ignore existing transactions
+            defaults to False
         :param commit_every: number rows of data to commit each time
             defaults to 5000
         :param db_pool_conn: connection pool contains multiple connections
             to connect to database
             defaults to None
             if None, a new connection will be created and automatically closed
             after being used
@@ -708,18 +712,14 @@
                 )
 
             columns_dq = [
                 f'"{col}"' for col in columns
             ]
 
             tmp_table = f'tmp_{table}_bulk_upsert'
-            # create_tmp_table_sql = f"CREATE TEMP TABLE {tmp_table} "
-            # create_tmp_table_sql += "ON COMMIT DROP "
-            # create_tmp_table_sql += f"AS SELECT * FROM {schema}.{table} "
-            # create_tmp_table_sql += "WITH NO DATA"
 
             create_tmp_table_sql = f"CREATE TEMP TABLE {tmp_table} "
             create_tmp_table_sql += f"(LIKE {schema}.{table} "
             create_tmp_table_sql += "INCLUDING DEFAULTS "
             create_tmp_table_sql += "INCLUDING CONSTRAINTS) "
             create_tmp_table_sql += "ON COMMIT DROP"
 
@@ -765,18 +765,21 @@
 
                 cur.copy_expert(sql=copy_sql, file=output)
 
                 upsert_data_sql = f"INSERT INTO {schema}.{table} "
                 upsert_data_sql += f"(SELECT * FROM {tmp_table}) "
                 upsert_data_sql += "ON CONFLICT "
                 upsert_data_sql += f"({', '.join(primary_keys)}) "
-                upsert_data_sql += "DO UPDATE SET "
-                upsert_data_sql += f"{', '.join(to_update_columns_sql)}"
-                if where_conditions:
-                    upsert_data_sql += f" WHERE {where_conditions}"
+                if ignore_existence:
+                    upsert_data_sql += "DO NOTHING"
+                else:
+                    upsert_data_sql += "DO UPDATE SET "
+                    upsert_data_sql += f"{', '.join(to_update_columns_sql)}"
+                    if where_conditions:
+                        upsert_data_sql += f" WHERE {where_conditions}"
 
                 cur.execute(upsert_data_sql)
 
                 conn.commit()
                 logging.info(
                     f'Loaded {commit_every} into {table} rows so far'
                 )
@@ -1203,44 +1206,44 @@
 
     def add_column(
         self,
         schema: str,
         table: str,
         column_name: str = None,
         dtype: str = None,
-        muliple_columns: dict = {},
+        multiple_columns: dict = {},
         db_pool_conn: Callable = None,
     ) -> None:
         """
         Create new column for a specific table
 
         :param schema: the schema contains table to create column
         :param table: the table to create column
         :param column_name: name of the column to create
             available when creating single column
             defaults to None
         :param dtype: data type of the column to create
             available when creating single column
             defaults to None
-        :param muliple_columns: dictionary contains columns name as key
+        :param multiple_columns: dictionary contains columns name as key
             and data type of columns as value respectively
             defaults to empty dictionary
         :param db_pool_conn: connection pool contains multiple connections
             to connect to database
             defaults to None
             if None, a new connection will be created and automatically closed
             after being used
         """
 
         sql = f"ALTER TABLE {schema}.{table} "
-        if muliple_columns:
+        if multiple_columns:
             sql += ", ".join(
                 [
-                    f"ADD COLUMN IF NOT EXISTS {col} {muliple_columns[col]}"
-                    for col in muliple_columns.keys()
+                    f"ADD COLUMN IF NOT EXISTS {col} {multiple_columns[col]}"
+                    for col in multiple_columns.keys()
                 ]
             )
         else:
             sql += f"ADD COLUMN IF NOT EXISTS {column_name} {dtype}"
 
         self.execute(
             sql=sql,
@@ -1298,20 +1301,14 @@
         sql += f"({', '.join(cols_sql)})"
 
         self.execute(
             sql=sql,
             db_pool_conn=db_pool_conn,
         )
 
-        self.auto_grant(
-            schema=schema,
-            list_tables=[table],
-            predefined_rules=True,
-        )
-
     def create_table_from_df(
         self,
         data: pd.DataFrame,
         schema: str,
         table: str,
     ) -> None:
         """
@@ -1319,26 +1316,20 @@
 
         :param data: reference dataframe for table creation
         :param schema: schema contains table to create
         :param table: table name to create
         """
 
         if self.account_name:
-            try:
-                credentials = get_credentials(
-                    platform='pg',
-                    account_name=self.account_name,
-                )
-                db_user = credentials['user_name']
-                db_password = credentials['password']
-            except Exception:
-                logging.error('Failed to get account credentials from minIO')
-                logging.info('Try using backup account')
-                db_user = 'y4a_sop_af_trino'
-                db_password = 'FJ!dlskjd0912lkjsd'
+            credentials = get_credentials(
+                platform='pg',
+                account_name=self.account_name,
+            )
+            db_user = credentials['user_name']
+            db_password = credentials['password']
         else:
             db_user = self.pg_account
             db_password = self.pg_password
 
         engine = create_engine(
             f'postgresql+psycopg2://{db_user}:{db_password}'
             f'@{self.host}:5432/{self.db}'
@@ -1347,20 +1338,14 @@
         data.head(0).to_sql(
             name=table,
             schema=schema,
             con=engine,
             index=False,
         )
 
-        self.auto_grant(
-            schema=schema,
-            list_tables=[table],
-            predefined_rules=True,
-        )
-
     def generate_log_data_path(
         self,
         file_path: str,
         database: str,
         mode: str,
         schema: str = None,
         table: str = None,
@@ -1566,111 +1551,81 @@
 
         return exists
 
     def auto_grant(
         self,
         schema: str,
         list_tables: list,
-        list_users: list = None,
+        list_users: list,
         privileges: list = ['SELECT'],
         all_privileges: bool = False,
-        predefined_rules: bool = False,
     ) -> None:
         """
         Grant table privileges to users in PostgreSQL
 
         :param schema: schema containing the table to grant
         :param list_tables: list of tables name to grant
         :param list_users: list of users to grant access
-            defaults to None
-            if None, the table will be granted for
-            all the predefined users
         :param privileges: list of privileges to grant
             defaults to ['SELECT']
         :param all_privileges: whether to grant all privileges
             defaults to False
-        :param predefined_rules: whether to grant the table with
-            the predefined rules
-            defaults to False
         """
-
-        if self.pg_name in ['raw_master', 'raw_repl']:
-            raw_users = [
-                'y4a_sop_longnc',
-                'y4a_sop_airflow_longnc',
-                'y4a_sop_trieuna',
-                'y4a_sop_airflow_trieuna',
-                'y4a_sop_khald',
-                'y4a_sop_airflow_khald',
-                'y4a_sop_airflow_linhvu',
-                'y4a_sop_linhvu',
-            ]
-
-            for table, user in product(
-                list_tables,
-                raw_users,
-            ):
+        to_grant = list()
+        for user in list_users:
+            try:
+                to_grant.append(
+                    get_credentials(
+                        platform='pg',
+                        account_name=user,
+                    )['user_name']
+                )
+            except IndexError:
+                to_grant.append(user)
+
+        for table, user in product(
+            list_tables,
+            to_grant,
+        ):
+            if all_privileges:
                 table_grant = f"GRANT ALL PRIVILEGES ON {schema}.{table} "
                 table_grant += f"to {user}"
+            else:
+                table_privileges = ', '.join(privileges)
+                table_grant = f"GRANT {table_privileges} ON "
+                table_grant += f"{schema}.{table} to {user}"
 
-                self.execute(table_grant)
-                logging.info(table_grant)
-
-            return
+            self.execute(table_grant)
+            logging.info(table_grant)
 
-        response = requests.get(
-            f"http://172.30.15.171:5431/v1/postgres/grant/{schema}"
-        ).json()
-
-        list_user_read = response["list_user_read"]
-        list_user_privileges = response["list_user_privileges"]
-
-        if predefined_rules:
-            for table, user in product(
-                list_tables,
-                list_user_read,
-            ):
-                table_grant = "GRANT SELECT ON "
-                table_grant += f"{schema}.{table} to {user}"
+    def sync_tmp2cdm(
+        self,
+        from_table: str,
+        to_table: str,
+    ) -> None:
+        conn = self.open_conn()
 
-                self.execute(table_grant)
-                logging.info(table_grant)
+        try:
+            cur = conn.cursor()
 
-            for table, user in product(
-                list_tables,
-                list_user_privileges,
-            ):
-                table_grant = f"GRANT ALL PRIVILEGES ON {schema}.{table} "
-                table_grant += f"to {user}"
+            truncate_sql = f"TRUNCATE TABLE y4a_cdm.{to_table}"
+            cur.execute(truncate_sql)
 
-                self.execute(table_grant)
-                logging.info(table_grant)
-        else:
-            if not list_users:
-                to_grant = list_user_read + list_user_privileges
-            else:
-                to_grant = list()
-                for user in list_users:
-                    try:
-                        to_grant.append(
-                            get_credentials(
-                                platform='pg',
-                                account_name=user,
-                            )['user_name']
-                        )
-                    except IndexError:
-                        to_grant.append(user)
-
-            for table, user in product(
-                list_tables,
-                to_grant,
-            ):
-                if all_privileges:
-                    table_grant = f"GRANT ALL PRIVILEGES ON {schema}.{table} "
-                    table_grant += f"to {user}"
-                else:
-                    table_privileges = ', '.join(privileges)
-                    table_grant = f"GRANT {table_privileges} ON "
-                    table_grant += f"{schema}.{table} to {user}"
+            insert_sql = f"""
+            INSERT INTO
+                y4a_cdm.{to_table}
+            SELECT
+                *
+            FROM
+                y4a_temp.{from_table}
+            """
+            cur.execute(insert_sql)
 
-                self.execute(table_grant)
-                logging.info(table_grant)
+            conn.commit()
+            cur.close()
+            self.close_conn(conn)
+            logging.info('Data synced')
+        except Exception as e:
+            conn.rollback()
+            cur.close()
+            self.close_conn(conn)
+            raise e
```

### Comparing `sop_deutils-0.9.9/sop_deutils/y4a_airflow.py` & `sop_deutils-1.0.0.dev0/sop_deutils/y4a_airflow.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-0.9.9/sop_deutils.egg-info/PKG-INFO` & `sop_deutils-1.0.0.dev0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,14 @@
-Metadata-Version: 2.1
-Name: sop_deutils
-Version: 0.9.9
-Summary: A utils package for Yes4All SOP
-Author-email: liuliukiki aka clong <longnc@yes4all.com>
-Project-URL: Author_Github, https://github.com/dribblewithclong
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE
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
-
 Yes4All SOP Utils Packages
 ==========================
 
 This is a utils package served for SOP Data Analytics team at **Yes4All**. It contains various modules to work with **PostgreSQL, MinIO, Google API, Airflow, Telegram…**
 
 .. image::
-   https://lh3.googleusercontent.com/drive-viewer/AK7aPaASSw5LzlIMog6XonAGba7CsmObYVMzQLzxMeBMFTuK30MCmuvB9ZOR-9VCq47rQpdgou849BL-oj5cufSECqxuE67c_w=s1600
+   https://lh3.googleusercontent.com/drive-viewer/AKGpihbzwqCnULTRFR1ihxbk2jwhfwhVfiZWGLfZ2W1argxs96TxMzfRTfaGgNQoL7NALlz94lMLrQnoK2y3jgOxh7raeq2rKJzU5sQ=s1600-rw-v1
    :scale: 20%
    :alt: liuliukiki
 
 --------------
 
 Contents Overview
 -----------------
@@ -262,14 +234,18 @@
 
 - ``sheet_name`` (optional): Worksheet name. The default value is ``'Sheet1'``. **(str)**
 
 - ``from_row_index`` (optional): The index of the row from which to begin inserting. The default value is ``1``. **(int)**
 
 - ``insert_column_names`` (optional): Whether to insert column names. The default value is ``False``. **(bool)**
 
+- ``parse_input`` (optional): Whether to parse input values as if the user typed them into the UI. The default value is ``True``. **(bool)**
+
+- ``pre_process`` (optional): Whether to process input based on the pre-defined function of DA. The default value is ``True``. **(bool)**
+
 .. code-block:: python
 
     sheet_utils.insert_data(
         data=df,
         sheet_id='your-sheet-id',
         from_row_index=2,
         insert_column_names=False,
@@ -284,14 +260,18 @@
 
 - ``sheet_id`` (required): Spreadsheet ID. **(str)**
 
 - ``sheet_name`` (optional): Worksheet name. The default value is ``'Sheet1'``. **(str)**
 
 - ``range_from`` (optional): The beginning of the range of data to update. The default value is ``'A1'``. **(str)**
 
+- ``parse_input`` (optional): Whether to parse input values as if the user typed them into the UI. The default value is ``True``. **(bool)**
+
+- ``pre_process`` (optional): Whether to process input based on the pre-defined function of DA. The default value is ``True``. **(bool)**
+
 .. code-block:: python
 
     sheet_utils.update_data(
         data=new_df,
         sheet_id='your-sheet-id',
         range_from='A4',
     )
@@ -392,27 +372,64 @@
 
 .. code-block:: python
 
     ss = sheet_utils.open_spread_sheet(
         sheet_id='your-sheet-id',
     )
 
+2.14 ``gspread_load_data``
+''''''''''''''''''''''''''''''''''''''
+
+To load data to the given sheet, using ``gspread_load_data`` method. This method is integrated with GSpread load data function that provides the high efficiency and convenience, it can be used as the alternative of two methods ``insert_data`` and ``update_data``, it has the following parameters:
+
+- ``data`` (required): Dataframe containing data to load. **(pd.DataFrame)**
+
+- ``sheet_id`` (required): Spreadsheet ID. **(str)**
+
+- ``sheet_name`` (optional): Worksheet name. The default value is ``'Sheet1'``. **(str)**
+
+- ``from_row`` (optional): Row at which to start loading the DataFrame. The default value is ``1``. **(int)**
+
+- ``from_col`` (optional): Column at which to start loading the DataFrame. The default value is ``1``. **(int)**
+
+- ``include_index`` (optional): Whether to include the DataFrame's index as an additional column. The default value is ``False``. **(bool)**
+
+- ``include_column`` (optional): Whether to add a header row or rows before data with column names (if include_index is True, the index's name(s) will be used as its columns' headers). The default value is ``True``. **(bool)**
+
+- ``resize_worksheet`` (optional): If True, changes the worksheet's size to match the shape of the provided DataFrame, if False, worksheet will only be resized as necessary to contain the DataFrame contents. The default value is ``False``. **(bool)**
+
+- ``allow_formulas`` (optional): Whether to interprets ``=foo`` as a formula in cell values; otherwise all text beginning with ``=`` is escaped to avoid its interpretation as a formula. The default value is ``True``. **(bool)**
+
+- ``string_escaping`` (optional): Determines when string values are escaped as text literals (by adding an initial ``'`` character) in requests to Sheets API, 3 parameter values are accepted: ('default': only escape strings starting with a literal ``'`` character. 'off': escape nothing; cell values starting with a ``'`` will be interpreted by sheets as an escape character followed by a text literal. 'full': escape all string values), the escaping done when allow_formulas=False (escaping string values beginning with ``=``) is unaffected by this parameter's value. The default value is ``'default'``. **(str)**
+
+.. code-block:: python
+
+    sheet_utils.gspread_load_data(
+        data=df,
+        sheet_id='your-sheet-id',
+        sheet_name='Sheet1',
+        from_row=3,
+        from_col=4,
+        include_index=True,
+        include_column=True,
+    )
+
 --------------
 
 MinIO
 ^^^^^
 
 MinIO is an object storage, it is API compatible with the Amazon S3 cloud storage service. MinIO can be used as a **datalake** to store unstructured data (photos, videos, log files, backups, and container images) and structured data.
 
 **Use case:** when need to store raw data or get raw data from datalake. Notes that the stored data extension must be ``.parquet`` .
 
 **Notes about how to determine the** ``file_path`` **parameter in minIO when using this module:**
 
 .. figure::
-   https://lh3.googleusercontent.com/drive-viewer/AEYmBYTeW1mCFR9M_cI4vg_bRRaLUVVxPtvkoWenEecrXSbmju3Xujj8jMI_MgiGBn-F5ozkkDPAWLPATwZ8JtdkciDopAaf=s1600
+   https://lh3.googleusercontent.com/drive-viewer/AEYmBYTnHBUSHkf9nTE9TuXWpEh12YMfUvHp2If3pJnjiRlmw6kdhqPrrprI-zMmdgM4O5pvSR8q1u5m5-XNRCo4Mc4rKJ-J=s1600
    :alt: minIO file path
 
 ..
 
    For example, if the directory to the data file in minIO is as above, then the ``file_path`` is ``"/scraping/amazon_vendor/avc_bulk_buy_request/2023/9/24/batch_1695525619"`` (after removing bucket name, data storage mode, and data file extension).
 
 **Functional:**
@@ -600,16 +617,14 @@
 
     pg_utils = PostgreSQLUtils(
         pg_name='serving_master',
         pg_account='y4a_sop_user1',
         pg_password='password-of-user1',
     )
 
-    # đều được
-
 4.2 ``read_sql_file``
 '''''''''''''''''''''
 
 To get the SQL query from an SQL file, using the ``read_sql_file`` method, it has the following parameter:
 
 - ``sql_file_path`` (required): The located path of the SQL file. **(str)**
 
@@ -686,14 +701,16 @@
 
 - ``schema`` (required): The schema containing the table to upsert. **(str)**
 
 - ``table`` (required): The name of the table to upsert the data into. **(str)**
 
 - ``where_conditions`` (optional): A string of a query that uses conditions to update. The default value is ``None``. **(str)**
 
+- ``ignore_existence`` (optional): Whether to insert only new transactions and ignore existing transactions. The default value is ``False``. **(bool)**
+
 - ``commit_every`` (optional): The number of rows of data to commit each time. The default value is ``5000``. **(int)**
 
 - ``db_pool_conn`` (optional): The connection pool to connect to the database. The default value is ``None``. If the value is ``None``, a new connection will be created and automatically closed after being used. **(callable)**
 
 .. code-block:: python
 
     pg_utils.upsert_data(
@@ -711,17 +728,19 @@
 
 - ``schema`` (required): The schema containing the table to upsert. **(str)**
 
 - ``table`` (required): The name of the table to upsert the data into. **(str)**
 
 - ``where_conditions`` (optional): A string of a query that uses conditions to update. The default value is ``None``. **(str)**
 
+- ``ignore_existence`` (optional): Whether to insert only new transactions and ignore existing transactions. The default value is ``False``. **(bool)**
+
 - ``commit_every`` (optional): The number of rows of data to commit each time. The default value is ``5000``. **(int)**
 
-- ``db_pool_conn`` (optional): A connection pool to connect to the database. The default value is ``None``. If the value is ``None``, a new connection will be created and automatically closed after being used. **(callable)**
+- ``db_pool_conn`` (optional): The connection pool to connect to the database. The default value is ``None``. If the value is ``None``, a new connection will be created and automatically closed after being used. **(callable)**
 
 .. code-block:: python
 
     pg_utils.bulk_upsert_data(
         data=your_df,
         schema='your-schema',
         table='your-table',
@@ -967,16 +986,14 @@
 
 - ``list_users`` (optional): A list of users to grant access. The default value is ``None``. If ``None``, the table will be granted for all the predefined users. **(list)**
 
 - ``privileges`` (optional): A list of privileges to grant. The default value is ``['SELECT']``. Accepted values in the privileges list are: ``'SELECT'``, ``'INSERT'``, ``'UPDATE'``, ``'DELETE'``, ``'TRUNCATE'``, ``'REFERENCES'``, ``'TRIGGER'``. **(list)**
 
 - ``all_privileges`` (optional): Whether to grant all privileges. The default value is ``False``. **(bool)**
 
-- ``predefined_rules`` (optional): Whether to grant with the predefined rules. The default value is ``False``. **(bool)**
-
 .. code-block:: python
 
     pg_utils.auto_grant(
         schema='your-schema',
         list_tables=['your-new-table'],
         list_users=[
             'linhvk',
@@ -1109,30 +1126,209 @@
 Telegram
 ^^^^^^^^
 
 **Use case:** When need to send messages to Telegram by using bot
 
 **Functional:**
 
+5.1 ``send_message``
+'''''''''''''''''''''''''
+
 To send messages to Telegram, using ``send_message`` method, it has the following parameters:
 
 - ``text`` (required): Message to send. **(str)**
 
 - ``bot_token`` (optional): Token of the bot which send the message. The default value is ``None``. If the value is ``None``, the bot ``sleep at 9pm`` will be used to send messages. **(str)**
 
 - ``chat_id`` (optional): ID of group chat where the message is sent. The default value is ``None``. If the value is ``None``, the group chat ``Airflow Status Alert`` will be used. **(str)**
 
+- ``parse_mode`` (optional): Sending mode, the accepted value is ``Markdown`` or ``HTML``. The default value is ``Markdown``. **(str)**
+
 .. code-block:: python
 
     from sop_deutils.y4a_telegram import send_message
 
     send_message(
         text='Hello liuliukiki'
     )
 
+5.2 ``send_data``
+'''''''''''''''''''''''''
+
+To send data to Telegram, using ``send_data`` method, it has the following parameters:
+
+- ``data`` (required): Data to send. **(pd.DataFrame)**
+
+- ``title`` (optional): The title of the message. The default value is ``None``. **(str)**
+
+- ``bot_token`` (optional): Token of the bot which send the data. The default value is ``None``. If the value is ``None``, the bot ``sleep at 9pm`` will be used to send data. **(str)**
+
+- ``chat_id`` (optional): ID of group chat where the data is sent. The default value is ``None``. If the value is ``None``, the group chat ``Airflow Status Alert`` will be used. **(str)**
+
+- ``parse_mode`` (optional): Sending mode, the accepted value is ``Markdown`` or ``HTML``. The default value is ``Markdown``. **(str)**
+
+.. code-block:: python
+
+    from sop_deutils.y4a_telegram import send_data
+
+    send_data(
+        data=my_df,
+        title='Sample Data',
+    )
+
+--------------
+
+GoogleChat
+^^^^^^^^^^
+
+**Use case:** When need to send messages to Google Chat space by using bot
+
+**Functional:**
+
+6.1 ``send_message``
+'''''''''''''''''''''''''
+
+To send messages to chat space of Google, using ``send_message`` method, it has the following parameters:
+
+- ``webhook_url`` (required): Url of the webhook that is registered in the chat space. `How to create webhook <https://developers.google.com/chat/how-tos/webhooks#create_a_webhook>`__. **(str)**
+
+- ``message`` (required): The content to send to the chat space. **(str)**
+
+.. code-block:: python
+
+    from sop_deutils.gg_api.y4a_chat import send_message
+
+    send_message(
+        webhook_url=f'https://chat.googleapis.com/v1/spaces/{SPACE_ID}/messages?key={KEY}&token={TOKEN}'
+        message='Hello liuliukiki',
+    )
+
+6.2 ``send_data``
+'''''''''''''''''''''''''
+
+To send data to chat space of Google, using ``send_data`` method, it has the following parameters:
+
+- ``webhook_url`` (required): Url of the webhook that is registered in the chat space. `How to create webhook <https://developers.google.com/chat/how-tos/webhooks#create_a_webhook>`__. **(str)**
+
+- ``data`` (required): Data to send. **(pd.DataFrame)**
+
+- ``title`` (optional): The title of the message. The default value is ``None``. **(str)**
+
+.. code-block:: python
+
+    from sop_deutils.gg_api.y4a_chat import send_data
+
+    send_data(
+        webhook_url=f'https://chat.googleapis.com/v1/spaces/{SPACE_ID}/messages?key={KEY}&token={TOKEN}'
+        data=my_df,
+        title='Sample Data',
+    )
+
+--------------
+
+GoogleMail
+^^^^^^^^^^
+
+**Use case:** when need to send email to group of people.
+
+**Functional:**
+
+7.1 initialize
+''''''''''''''
+
+Firstly, import GGMail utils module class. This class has two parameters:
+
+- ``sender_email``: The email of sender. The default value is ``None``. If not provide, the email of DA team will be used. **(str)**
+- ``sender_password``: The password email of sender. The default value is ``None``. If not provide, the email of DA team will be used. **(str)**
+
+.. code-block:: python
+
+    from sop_deutils.gg_api.y4a_mail import GGMailUtils
+
+    mail_utils = GGMailUtils() # This utils will use email of DA team
+
+    # or
+
+    mail_utils = GGMailUtils(
+        sender_email='user@domain.abc',
+        sender_password='something',
+    )
+
+7.2 ``send_mail``
+'''''''''''''''''''''
+
+To send plain text email, using the ``send_mail`` method, it has the following parameter:
+
+- ``receiver_email`` (required): List of people to receive email. **(list)**
+
+- ``content`` (required): The content of email. **(str)**
+
+- ``cc_email`` (optional): List of people to receive CC. The default value is ``None``. **(list)**
+
+- ``subject`` (optional): The subject of email. The default value is ``None``. **(str)**
+
+.. code-block:: python
+
+    mail_utils.send_mail(
+        receiver_email=['user1@domain.abc', 'user2@domain.abc'],
+        content='j ai biec',
+    )
+
+7.3 ``send_mail_w_attachments``
+'''''''''''''''''''''''''''''''''''
+
+To send email with attachments, using the ``send_mail_w_attachments`` method, it has the following parameters:
+
+- ``receiver_email`` (required): List of people to receive email. **(list)**
+
+- ``content`` (required): The content of email. **(str)**
+
+- ``attachment_path`` (required): List of file path to attach. **(list)**
+
+- ``cc_email`` (optional): List of people to receive CC. The default value is ``None``. **(list)**
+
+- ``subject`` (optional): The subject of email. The default value is ``None``. **(str)**
+
+.. code-block:: python
+
+    mail_utils.send_mail_w_attachments(
+        receiver_email=['user1@domain.abc', 'user2@domain.abc'],
+        content='j ai biec',
+        attachment_path=['parent_dir/file1.xlsx', 'parent_dir/file2.xlsx'],
+    )
+
+7.4 ``send_mail_w_pandas_df``
+''''''''''''''''''''''''''''''''''
+
+To send email with pandas dataframe as Excel file to group of people, using the ``send_mail_w_pandas_df`` method, it has the following parameters:
+
+- ``receiver_email`` (required): List of people to receive email. **(list)**
+
+- ``content`` (required): The content of email. **(str)**
+
+- ``data_list`` (required): List of dataframe to attach. **(list)**
+
+- ``file_name`` (required): List of file name respectively to list of dataframe. Notes that each file name must contain ``.xlsx``.  **(list)**
+
+- ``cc_email`` (optional): List of people to receive CC. The default value is ``None``. **(list)**
+
+- ``subject`` (optional): The subject of email. The default value is ``None``. **(str)**
+
+.. code-block:: python
+
+    df1 = pd.DataFrame([1, 2, 3], columns=['d1'])
+    df2 = pd.DataFrame([4, 5, 6], columns=['d2'])
+
+    mail_utils.send_mail_w_pandas_df(
+        receiver_email=['user1@domain.abc', 'user2@domain.abc'],
+        content='j ai biec',
+        data_list=[df1, df2],
+        file_name=['data1.xlsx', 'data2.xlsx'],
+    )
+
 --------------
 
 All in one (DAConfig)
 ^^^^^^^^^^^^^^^^^^^^^
 
 **Use case:** So far, there are a lot of platforms that needs to access frequently, in order not to import lots of modules, users can inherit all of above modules as simplest way.
 
@@ -1300,11 +1496,16 @@
                 >>  etl_from_sheet_to_db(spread_sheet_id) \
                     >> execute_query()
 
 --------------
 
    provided by ``liuliukiki``
 
-..
+--------------
+
+   ``hinh anh users feedback thu vien kieu``
 
-   and special thank to ``duiikha`` for contributing api method to get
-   and secure account credentials.
+
+.. image::
+   https://lh3.googleusercontent.com/drive-viewer/AKGpihbUbW3ahIwUoCZq72pzvL8LVxRw-SkAzoYjsvg6pUY_hp6LSoklWol3oPSDPTb-Ny9kY8U1lY8pw3lFAYvjFUtfRI_6S8toISk=s1600-rw-v1
+   :scale: 44%
+   :alt: DA team
```

### Comparing `sop_deutils-0.9.9/sop_deutils.egg-info/SOURCES.txt` & `sop_deutils-1.0.0.dev0/sop_deutils.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 sop_deutils/__init__.py
+sop_deutils/r.zip
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
+sop_deutils/gg_api/y4a_chat.py
+sop_deutils/gg_api/y4a_mail.py
 sop_deutils/gg_api/y4a_sheet.py
 sop_deutils/sql/y4a_monitor_user.py
 sop_deutils/sql/y4a_mysql.py
 sop_deutils/sql/y4a_postgresql.py
```


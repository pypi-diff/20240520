# Comparing `tmp/suse_udfs_cyy-0.1.0.tar.gz` & `tmp/suse_udfs_cyy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suse_udfs_cyy-0.1.0.tar", last modified: Thu Dec 21 09:07:38 2023, max compression
+gzip compressed data, was "suse_udfs_cyy-0.1.1.tar", last modified: Mon May 20 20:11:00 2024, max compression
```

## Comparing `suse_udfs_cyy-0.1.0.tar` & `suse_udfs_cyy-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-12-21 09:07:38.303185 suse_udfs_cyy-0.1.0/
--rw-rw-rw-   0        0        0      900 2023-12-21 09:07:38.303185 suse_udfs_cyy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-12-21 07:59:59.000000 suse_udfs_cyy-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-12-21 09:07:38.303185 suse_udfs_cyy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      930 2023-12-21 09:07:35.000000 suse_udfs_cyy-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-21 09:07:38.301181 suse_udfs_cyy-0.1.0/suse_udfs_cyy/
--rw-rw-rw-   0        0        0    21348 2023-12-21 07:47:13.000000 suse_udfs_cyy-0.1.0/suse_udfs_cyy/UDFs.py
--rw-rw-rw-   0        0        0       34 2023-12-21 07:47:13.000000 suse_udfs_cyy-0.1.0/suse_udfs_cyy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-21 09:07:38.303185 suse_udfs_cyy-0.1.0/suse_udfs_cyy.egg-info/
--rw-rw-rw-   0        0        0      900 2023-12-21 09:07:38.000000 suse_udfs_cyy-0.1.0/suse_udfs_cyy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-12-21 09:07:38.000000 suse_udfs_cyy-0.1.0/suse_udfs_cyy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-21 09:07:38.000000 suse_udfs_cyy-0.1.0/suse_udfs_cyy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-12-21 09:07:38.000000 suse_udfs_cyy-0.1.0/suse_udfs_cyy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 20:11:00.218645 suse_udfs_cyy-0.1.1/
+-rw-rw-rw-   0        0        0      900 2024-05-20 20:11:00.218645 suse_udfs_cyy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2024-01-22 02:17:28.000000 suse_udfs_cyy-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-20 20:11:00.218645 suse_udfs_cyy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      930 2024-05-20 20:05:07.000000 suse_udfs_cyy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 20:11:00.216138 suse_udfs_cyy-0.1.1/suse_udfs_cyy/
+-rw-rw-rw-   0        0        0    21587 2024-05-20 19:58:57.000000 suse_udfs_cyy-0.1.1/suse_udfs_cyy/UDFs.py
+-rw-rw-rw-   0        0        0       34 2024-01-22 02:17:28.000000 suse_udfs_cyy-0.1.1/suse_udfs_cyy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 20:11:00.218645 suse_udfs_cyy-0.1.1/suse_udfs_cyy.egg-info/
+-rw-rw-rw-   0        0        0      900 2024-05-20 20:11:00.000000 suse_udfs_cyy-0.1.1/suse_udfs_cyy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-05-20 20:11:00.000000 suse_udfs_cyy-0.1.1/suse_udfs_cyy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 20:11:00.000000 suse_udfs_cyy-0.1.1/suse_udfs_cyy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-20 20:11:00.000000 suse_udfs_cyy-0.1.1/suse_udfs_cyy.egg-info/top_level.txt
```

### Comparing `suse_udfs_cyy-0.1.0/PKG-INFO` & `suse_udfs_cyy-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suse_udfs_cyy
-Version: 0.1.0
+Version: 0.1.1
 Summary: A useful tool for extracting data using WindPy
 Home-page: 
 Author: YaoyuChenWilliam
 Author-email: yaoyuchenslm@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `suse_udfs_cyy-0.1.0/setup.py` & `suse_udfs_cyy-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='suse_udfs_cyy',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     description='A useful tool for extracting data using WindPy',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='',
     author='YaoyuChenWilliam',
     author_email='yaoyuchenslm@gmail.com',
```

### Comparing `suse_udfs_cyy-0.1.0/suse_udfs_cyy/UDFs.py` & `suse_udfs_cyy-0.1.1/suse_udfs_cyy/UDFs.py`

 * *Files 5% similar despite different names*

```diff
@@ -606,7 +606,14 @@
     task_list=list_ongoing_process()
     # 遍历当前活动的进程
     for proc in task_list:
         if process_name.lower() in proc:
             detect=True
             break
     return detect
+
+def pandas_df_display_full():
+    import pandas as pd
+    pd.set_option('display.max_columns', None)
+    pd.set_option('display.max_rows', None)
+    pd.set_option('max_colwidth', 1000)
+    pd.set_option('expand_frame_repr', False)
```

### Comparing `suse_udfs_cyy-0.1.0/suse_udfs_cyy.egg-info/PKG-INFO` & `suse_udfs_cyy-0.1.1/suse_udfs_cyy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suse-udfs-cyy
-Version: 0.1.0
+Version: 0.1.1
 Summary: A useful tool for extracting data using WindPy
 Home-page: 
 Author: YaoyuChenWilliam
 Author-email: yaoyuchenslm@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```


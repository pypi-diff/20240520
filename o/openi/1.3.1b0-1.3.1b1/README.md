# Comparing `tmp/openi-1.3.1b0.tar.gz` & `tmp/openi-1.3.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-1.3.1b0.tar", last modified: Fri May 17 03:16:19 2024, max compression
+gzip compressed data, was "openi-1.3.1b1.tar", last modified: Mon May 20 06:33:10 2024, max compression
```

## Comparing `openi-1.3.1b0.tar` & `openi-1.3.1b1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 03:16:19.654557 openi-1.3.1b0/
--rw-rw-rw-   0        0        0     3052 2024-05-17 03:16:19.653557 openi-1.3.1b0/PKG-INFO
--rw-rw-rw-   0        0        0     2368 2023-11-10 01:52:31.000000 openi-1.3.1b0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-17 03:16:19.654557 openi-1.3.1b0/setup.cfg
--rw-rw-rw-   0        0        0     1059 2024-05-17 03:14:10.000000 openi-1.3.1b0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 03:16:19.598557 openi-1.3.1b0/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 03:16:19.610556 openi-1.3.1b0/src/openi/
--rw-rw-rw-   0        0        0      119 2024-05-17 03:02:56.000000 openi-1.3.1b0/src/openi/__init__.py
--rw-rw-rw-   0        0        0     3109 2024-05-17 03:02:56.000000 openi-1.3.1b0/src/openi/_login.py
--rw-rw-rw-   0        0        0    13681 2024-05-17 03:02:56.000000 openi-1.3.1b0/src/openi/apis.py
--rw-rw-rw-   0        0        0     7871 2024-05-17 03:05:23.000000 openi-1.3.1b0/src/openi/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-17 03:16:19.621556 openi-1.3.1b0/src/openi/dataset/
--rw-rw-rw-   0        0        0       48 2024-05-17 03:02:56.000000 openi-1.3.1b0/src/openi/dataset/__init__.py
--rw-rw-rw-   0        0        0     2763 2024-05-17 03:02:56.000000 openi-1.3.1b0/src/openi/dataset/download.py
--rw-rw-rw-   0        0        0     1902 2024-05-17 03:05:18.000000 openi-1.3.1b0/src/openi/dataset/upload.py
-drwxrwxrwx   0        0        0        0 2024-05-17 03:16:19.624556 openi-1.3.1b0/src/openi/model/
--rw-rw-rw-   0        0        0       48 2024-05-17 03:02:56.000000 openi-1.3.1b0/src/openi/model/__init__.py
--rw-rw-rw-   0        0        0     4951 2024-05-17 03:02:56.000000 openi-1.3.1b0/src/openi/model/download.py
--rw-rw-rw-   0        0        0     5329 2024-05-17 03:02:56.000000 openi-1.3.1b0/src/openi/model/upload.py
-drwxrwxrwx   0        0        0        0 2024-05-17 03:16:19.633557 openi-1.3.1b0/src/openi/services/
--rw-rw-rw-   0        0        0      182 2024-05-17 03:02:56.000000 openi-1.3.1b0/src/openi/services/__init__.py
--rw-rw-rw-   0        0        0     2262 2024-05-17 03:02:56.000000 openi-1.3.1b0/src/openi/services/dataset_struct.py
--rw-rw-rw-   0        0        0     3552 2024-05-17 03:02:56.000000 openi-1.3.1b0/src/openi/services/file_download.py
--rw-rw-rw-   0        0        0     1416 2024-05-17 03:02:56.000000 openi-1.3.1b0/src/openi/services/file_progress_bar.py
--rw-rw-rw-   0        0        0    10985 2024-05-17 03:02:56.000000 openi-1.3.1b0/src/openi/services/file_upload.py
--rw-rw-rw-   0        0        0     2829 2024-05-17 03:02:56.000000 openi-1.3.1b0/src/openi/services/model_struct.py
--rw-rw-rw-   0        0        0     2602 2024-05-17 03:02:56.000000 openi-1.3.1b0/src/openi/services/repo_struct.py
-drwxrwxrwx   0        0        0        0 2024-05-17 03:16:19.637562 openi-1.3.1b0/src/openi/utils/
--rw-rw-rw-   0        0        0       49 2024-05-17 03:02:56.000000 openi-1.3.1b0/src/openi/utils/__init__.py
--rw-rw-rw-   0        0        0     4832 2024-05-17 03:09:23.000000 openi-1.3.1b0/src/openi/utils/constants.py
--rw-rw-rw-   0        0        0     1956 2024-05-17 03:02:56.000000 openi-1.3.1b0/src/openi/utils/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-17 03:16:19.652557 openi-1.3.1b0/src/openi.egg-info/
--rw-rw-rw-   0        0        0     3052 2024-05-17 03:16:19.000000 openi-1.3.1b0/src/openi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      827 2024-05-17 03:16:19.000000 openi-1.3.1b0/src/openi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 03:16:19.000000 openi-1.3.1b0/src/openi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-17 03:16:19.000000 openi-1.3.1b0/src/openi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-17 03:16:19.000000 openi-1.3.1b0/src/openi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-17 03:16:19.000000 openi-1.3.1b0/src/openi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-17 03:16:19.651557 openi-1.3.1b0/test/
--rw-rw-rw-   0        0        0     1149 2024-04-29 07:10:45.000000 openi-1.3.1b0/test/test.py
--rw-rw-rw-   0        0        0      124 2024-04-28 08:58:09.000000 openi-1.3.1b0/test/test_openi.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:33:10.238489 openi-1.3.1b1/
+-rw-rw-rw-   0        0        0     3052 2024-05-20 06:33:10.237490 openi-1.3.1b1/PKG-INFO
+-rw-rw-rw-   0        0        0     2368 2023-11-10 01:52:31.000000 openi-1.3.1b1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-20 06:33:10.238489 openi-1.3.1b1/setup.cfg
+-rw-rw-rw-   0        0        0     1059 2024-05-20 06:30:34.000000 openi-1.3.1b1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:33:10.187947 openi-1.3.1b1/src/
+drwxrwxrwx   0        0        0        0 2024-05-20 06:33:10.199460 openi-1.3.1b1/src/openi/
+-rw-rw-rw-   0        0        0      119 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/__init__.py
+-rw-rw-rw-   0        0        0     3109 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/_login.py
+-rw-rw-rw-   0        0        0    13681 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/apis.py
+-rw-rw-rw-   0        0        0     7871 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:33:10.214489 openi-1.3.1b1/src/openi/dataset/
+-rw-rw-rw-   0        0        0       48 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/dataset/__init__.py
+-rw-rw-rw-   0        0        0     2763 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/dataset/download.py
+-rw-rw-rw-   0        0        0     1902 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/dataset/upload.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:33:10.218488 openi-1.3.1b1/src/openi/model/
+-rw-rw-rw-   0        0        0       48 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/model/__init__.py
+-rw-rw-rw-   0        0        0     4951 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/model/download.py
+-rw-rw-rw-   0        0        0     5329 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/model/upload.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:33:10.227488 openi-1.3.1b1/src/openi/services/
+-rw-rw-rw-   0        0        0      182 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/services/__init__.py
+-rw-rw-rw-   0        0        0     2262 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/services/dataset_struct.py
+-rw-rw-rw-   0        0        0     3552 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/services/file_download.py
+-rw-rw-rw-   0        0        0     1416 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/services/file_progress_bar.py
+-rw-rw-rw-   0        0        0    10985 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/services/file_upload.py
+-rw-rw-rw-   0        0        0     2829 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/services/model_struct.py
+-rw-rw-rw-   0        0        0     2602 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/services/repo_struct.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:33:10.232488 openi-1.3.1b1/src/openi/utils/
+-rw-rw-rw-   0        0        0       49 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/utils/__init__.py
+-rw-rw-rw-   0        0        0     4832 2024-05-20 06:30:28.000000 openi-1.3.1b1/src/openi/utils/constants.py
+-rw-rw-rw-   0        0        0     1956 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/utils/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:33:10.236501 openi-1.3.1b1/src/openi.egg-info/
+-rw-rw-rw-   0        0        0     3052 2024-05-20 06:33:10.000000 openi-1.3.1b1/src/openi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      827 2024-05-20 06:33:10.000000 openi-1.3.1b1/src/openi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 06:33:10.000000 openi-1.3.1b1/src/openi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-20 06:33:10.000000 openi-1.3.1b1/src/openi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-20 06:33:10.000000 openi-1.3.1b1/src/openi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-20 06:33:10.000000 openi-1.3.1b1/src/openi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 06:33:10.234488 openi-1.3.1b1/test/
+-rw-rw-rw-   0        0        0     1149 2024-04-29 07:10:45.000000 openi-1.3.1b1/test/test.py
+-rw-rw-rw-   0        0        0      124 2024-04-28 08:58:09.000000 openi-1.3.1b1/test/test_openi.py
```

### Comparing `openi-1.3.1b0/PKG-INFO` & `openi-1.3.1b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi
-Version: 1.3.1b0
+Version: 1.3.1b1
 Summary: A package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-1.3.1b0/README.md` & `openi-1.3.1b1/README.md`

 * *Files identical despite different names*

### Comparing `openi-1.3.1b0/setup.py` & `openi-1.3.1b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="openi",
-    version="1.3.1b0",
+    version="1.3.1b1",
     description="A package for openi pypi",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi",
     author="chenzh05",
```

### Comparing `openi-1.3.1b0/src/openi/_login.py` & `openi-1.3.1b1/src/openi/_login.py`

 * *Files identical despite different names*

### Comparing `openi-1.3.1b0/src/openi/apis.py` & `openi-1.3.1b1/src/openi/apis.py`

 * *Files identical despite different names*

### Comparing `openi-1.3.1b0/src/openi/cli.py` & `openi-1.3.1b1/src/openi/cli.py`

 * *Files identical despite different names*

### Comparing `openi-1.3.1b0/src/openi/dataset/download.py` & `openi-1.3.1b1/src/openi/dataset/download.py`

 * *Files identical despite different names*

### Comparing `openi-1.3.1b0/src/openi/dataset/upload.py` & `openi-1.3.1b1/src/openi/dataset/upload.py`

 * *Files identical despite different names*

### Comparing `openi-1.3.1b0/src/openi/model/download.py` & `openi-1.3.1b1/src/openi/model/download.py`

 * *Files identical despite different names*

### Comparing `openi-1.3.1b0/src/openi/model/upload.py` & `openi-1.3.1b1/src/openi/model/upload.py`

 * *Files identical despite different names*

### Comparing `openi-1.3.1b0/src/openi/services/dataset_struct.py` & `openi-1.3.1b1/src/openi/services/dataset_struct.py`

 * *Files identical despite different names*

### Comparing `openi-1.3.1b0/src/openi/services/file_download.py` & `openi-1.3.1b1/src/openi/services/file_download.py`

 * *Files identical despite different names*

### Comparing `openi-1.3.1b0/src/openi/services/file_progress_bar.py` & `openi-1.3.1b1/src/openi/services/file_progress_bar.py`

 * *Files identical despite different names*

### Comparing `openi-1.3.1b0/src/openi/services/file_upload.py` & `openi-1.3.1b1/src/openi/services/file_upload.py`

 * *Files identical despite different names*

### Comparing `openi-1.3.1b0/src/openi/services/model_struct.py` & `openi-1.3.1b1/src/openi/services/model_struct.py`

 * *Files identical despite different names*

### Comparing `openi-1.3.1b0/src/openi/services/repo_struct.py` & `openi-1.3.1b1/src/openi/services/repo_struct.py`

 * *Files identical despite different names*

### Comparing `openi-1.3.1b0/src/openi/utils/constants.py` & `openi-1.3.1b1/src/openi/utils/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 
     command_model_upload = "上传模型文件夹，需指定本地路径,仓库路径及模型名称"
     model_upload_help = "上传模型文件夹, openi model upload -h 查看更多说明"
     model_upload_usage = (
         "openi model upload [-f folder] [-r repo_id] [-m model_name] [-h]"
     )
     model_upload_param_folder = (
-        "本地文件夹路径，路径下可包含多个模型文件，不能包含子目录"
+        "本地文件夹路径，路径下可包含多个模型文件，允许包含子目录"
     )
     model_upload_param_repo_id = (
         "所在仓库路径，格式为`拥有者/仓库名`，登录用户需要拥有此仓库权限"
     )
     model_upload_param_model_name = "网页端模型名称"
 
     command_model_download = "下载模型文件夹，需指定仓库路径及模型名称"
```

### Comparing `openi-1.3.1b0/src/openi/utils/logger.py` & `openi-1.3.1b1/src/openi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `openi-1.3.1b0/src/openi.egg-info/PKG-INFO` & `openi-1.3.1b1/src/openi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi
-Version: 1.3.1b0
+Version: 1.3.1b1
 Summary: A package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-1.3.1b0/src/openi.egg-info/SOURCES.txt` & `openi-1.3.1b1/src/openi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openi-1.3.1b0/test/test.py` & `openi-1.3.1b1/test/test.py`

 * *Files identical despite different names*


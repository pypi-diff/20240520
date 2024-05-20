# Comparing `tmp/eliasliu-0.1.55.tar.gz` & `tmp/eliasliu-0.1.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eliasliu-0.1.55.tar", last modified: Mon May  6 15:56:27 2024, max compression
+gzip compressed data, was "eliasliu-0.1.56.tar", last modified: Mon May 20 06:47:48 2024, max compression
```

## Comparing `eliasliu-0.1.55.tar` & `eliasliu-0.1.56.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 15:56:27.461258 eliasliu-0.1.55/
--rw-rw-rw-   0        0        0     6990 2024-05-06 15:56:27.458266 eliasliu-0.1.55/PKG-INFO
--rw-rw-rw-   0        0        0     5851 2024-05-06 15:18:50.000000 eliasliu-0.1.55/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 15:56:27.418373 eliasliu-0.1.55/elias/
-drwxrwxrwx   0        0        0        0 2024-05-06 15:56:27.432345 eliasliu-0.1.55/elias/Scripts/
--rw-rw-rw-   0        0        0     2788 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/Scripts/MysqlTool.py
--rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/Scripts/__init__.py
--rw-rw-rw-   0        0        0     6723 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/Scripts/douyin.py
--rw-rw-rw-   0        0        0     5118 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/Scripts/jd.py
--rw-rw-rw-   0        0        0     2407 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/Scripts/name_in_db.py
--rw-rw-rw-   0        0        0    15915 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/Scripts/py_clickhouse.py
--rw-rw-rw-   0        0        0    15332 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/Scripts/vm_clickhouse.py
--rw-rw-rw-   0        0        0     3396 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/Scripts/youdao.py
--rw-rw-rw-   0        0        0      368 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/__init__.py
--rw-rw-rw-   0        0        0    30771 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/check.py
--rw-rw-rw-   0        0        0     1376 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/config_env_variable.py
--rw-rw-rw-   0        0        0     9670 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/datamove.py
-drwxrwxrwx   0        0        0        0 2024-05-06 15:56:27.446298 eliasliu-0.1.55/elias/datax/
--rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/datax/__init__.py
--rw-rw-rw-   0        0        0    15834 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/datax/auto_create_table.py
--rw-rw-rw-   0        0        0     3493 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/datax/job.py
--rw-rw-rw-   0        0        0     4138 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/datax/main.py
--rw-rw-rw-   0        0        0     5480 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/datax/reader.py
--rw-rw-rw-   0        0        0     1756 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/datax/run.py
--rw-rw-rw-   0        0        0     3588 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/datax/writer.py
--rw-rw-rw-   0        0        0    92990 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/etl.py
--rw-rw-rw-   0        0        0     9840 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/picture.py
--rw-rw-rw-   0        0        0    77789 2024-05-06 15:55:38.000000 eliasliu-0.1.55/elias/usual.py
--rw-rw-rw-   0        0        0    13040 2024-05-06 15:18:50.000000 eliasliu-0.1.55/elias/wechat.py
-drwxrwxrwx   0        0        0        0 2024-05-06 15:56:27.456271 eliasliu-0.1.55/eliasliu.egg-info/
--rw-rw-rw-   0        0        0     6990 2024-05-06 15:56:27.000000 eliasliu-0.1.55/eliasliu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      688 2024-05-06 15:56:27.000000 eliasliu-0.1.55/eliasliu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 15:56:27.000000 eliasliu-0.1.55/eliasliu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2024-05-06 15:56:27.000000 eliasliu-0.1.55/eliasliu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-06 15:56:27.000000 eliasliu-0.1.55/eliasliu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 15:56:27.461258 eliasliu-0.1.55/setup.cfg
--rw-rw-rw-   0        0        0     1928 2024-05-06 15:56:15.000000 eliasliu-0.1.55/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:47:48.822179 eliasliu-0.1.56/
+-rw-rw-rw-   0        0        0     7013 2024-05-20 06:47:48.821179 eliasliu-0.1.56/PKG-INFO
+-rw-rw-rw-   0        0        0     5851 2024-05-06 15:18:50.000000 eliasliu-0.1.56/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 06:47:48.806179 eliasliu-0.1.56/elias/
+drwxrwxrwx   0        0        0        0 2024-05-20 06:47:48.812179 eliasliu-0.1.56/elias/Scripts/
+-rw-rw-rw-   0        0        0     2788 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/Scripts/MysqlTool.py
+-rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/Scripts/__init__.py
+-rw-rw-rw-   0        0        0     6723 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/Scripts/douyin.py
+-rw-rw-rw-   0        0        0     5118 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/Scripts/jd.py
+-rw-rw-rw-   0        0        0     2407 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/Scripts/name_in_db.py
+-rw-rw-rw-   0        0        0    15915 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/Scripts/py_clickhouse.py
+-rw-rw-rw-   0        0        0    15332 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/Scripts/vm_clickhouse.py
+-rw-rw-rw-   0        0        0     3396 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/Scripts/youdao.py
+-rw-rw-rw-   0        0        0      368 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/__init__.py
+-rw-rw-rw-   0        0        0      955 2024-05-20 06:42:43.000000 eliasliu-0.1.56/elias/ai.py
+-rw-rw-rw-   0        0        0    30771 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/check.py
+-rw-rw-rw-   0        0        0     1376 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/config_env_variable.py
+-rw-rw-rw-   0        0        0     9670 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/datamove.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:47:48.817179 eliasliu-0.1.56/elias/datax/
+-rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/datax/__init__.py
+-rw-rw-rw-   0        0        0    15834 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/datax/auto_create_table.py
+-rw-rw-rw-   0        0        0     3493 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/datax/job.py
+-rw-rw-rw-   0        0        0     4138 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/datax/main.py
+-rw-rw-rw-   0        0        0     5480 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/datax/reader.py
+-rw-rw-rw-   0        0        0     1756 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/datax/run.py
+-rw-rw-rw-   0        0        0     3588 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/datax/writer.py
+-rw-rw-rw-   0        0        0    92990 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/etl.py
+-rw-rw-rw-   0        0        0     9840 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/picture.py
+-rw-rw-rw-   0        0        0    77789 2024-05-06 15:55:38.000000 eliasliu-0.1.56/elias/usual.py
+-rw-rw-rw-   0        0        0    13040 2024-05-06 15:18:50.000000 eliasliu-0.1.56/elias/wechat.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:47:48.820180 eliasliu-0.1.56/eliasliu.egg-info/
+-rw-rw-rw-   0        0        0     7013 2024-05-20 06:47:48.000000 eliasliu-0.1.56/eliasliu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      700 2024-05-20 06:47:48.000000 eliasliu-0.1.56/eliasliu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 06:47:48.000000 eliasliu-0.1.56/eliasliu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      169 2024-05-20 06:47:48.000000 eliasliu-0.1.56/eliasliu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-20 06:47:48.000000 eliasliu-0.1.56/eliasliu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 06:47:48.822179 eliasliu-0.1.56/setup.cfg
+-rw-rw-rw-   0        0        0     1947 2024-05-20 06:43:37.000000 eliasliu-0.1.56/setup.py
```

### Comparing `eliasliu-0.1.55/PKG-INFO` & `eliasliu-0.1.56/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.55
+Version: 0.1.56
 Summary: A very easy tool to deal your data
 Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -24,14 +24,15 @@
 Requires-Dist: mysql-connector-python
 Requires-Dist: impyla
 Requires-Dist: clickhouse_sqlalchemy
 Requires-Dist: clickhouse_driver
 Requires-Dist: bs4
 Requires-Dist: selenium
 Requires-Dist: loguru
+Requires-Dist: ollama
 Requires-Dist: pillow
 Requires-Dist: opencv-python
 
 0 安装
 找到终端，再终端内输入以下代码
 安装
 pip install elias
```

### Comparing `eliasliu-0.1.55/README.md` & `eliasliu-0.1.56/README.md`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/elias/Scripts/MysqlTool.py` & `eliasliu-0.1.56/elias/Scripts/MysqlTool.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/elias/Scripts/douyin.py` & `eliasliu-0.1.56/elias/Scripts/douyin.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/elias/Scripts/jd.py` & `eliasliu-0.1.56/elias/Scripts/jd.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/elias/Scripts/name_in_db.py` & `eliasliu-0.1.56/elias/Scripts/name_in_db.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/elias/Scripts/py_clickhouse.py` & `eliasliu-0.1.56/elias/Scripts/py_clickhouse.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/elias/Scripts/vm_clickhouse.py` & `eliasliu-0.1.56/elias/Scripts/vm_clickhouse.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/elias/Scripts/youdao.py` & `eliasliu-0.1.56/elias/Scripts/youdao.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/elias/check.py` & `eliasliu-0.1.56/elias/check.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/elias/config_env_variable.py` & `eliasliu-0.1.56/elias/config_env_variable.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/elias/datamove.py` & `eliasliu-0.1.56/elias/datamove.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/elias/datax/auto_create_table.py` & `eliasliu-0.1.56/elias/datax/auto_create_table.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/elias/datax/job.py` & `eliasliu-0.1.56/elias/datax/job.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/elias/datax/main.py` & `eliasliu-0.1.56/elias/datax/main.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/elias/datax/reader.py` & `eliasliu-0.1.56/elias/datax/reader.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/elias/datax/run.py` & `eliasliu-0.1.56/elias/datax/run.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/elias/datax/writer.py` & `eliasliu-0.1.56/elias/datax/writer.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/elias/etl.py` & `eliasliu-0.1.56/elias/etl.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/elias/picture.py` & `eliasliu-0.1.56/elias/picture.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/elias/usual.py` & `eliasliu-0.1.56/elias/usual.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/elias/wechat.py` & `eliasliu-0.1.56/elias/wechat.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.55/eliasliu.egg-info/PKG-INFO` & `eliasliu-0.1.56/eliasliu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.55
+Version: 0.1.56
 Summary: A very easy tool to deal your data
 Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -24,14 +24,15 @@
 Requires-Dist: mysql-connector-python
 Requires-Dist: impyla
 Requires-Dist: clickhouse_sqlalchemy
 Requires-Dist: clickhouse_driver
 Requires-Dist: bs4
 Requires-Dist: selenium
 Requires-Dist: loguru
+Requires-Dist: ollama
 Requires-Dist: pillow
 Requires-Dist: opencv-python
 
 0 安装
 找到终端，再终端内输入以下代码
 安装
 pip install elias
```

### Comparing `eliasliu-0.1.55/eliasliu.egg-info/SOURCES.txt` & `eliasliu-0.1.56/eliasliu.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 setup.py
 elias/__init__.py
+elias/ai.py
 elias/check.py
 elias/config_env_variable.py
 elias/datamove.py
 elias/etl.py
 elias/picture.py
 elias/usual.py
 elias/wechat.py
```

### Comparing `eliasliu-0.1.55/setup.py` & `eliasliu-0.1.56/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='eliasliu',  # 包名
-    version='0.1.55',  # 版本号
+    version='0.1.56',  # 版本号
     description='A very easy tool to deal your data',  # 包的简要描述
     long_description = long_description,
     # long_description='Data Engineer & Analyst will use',  # 包的详细描述，通常从README文件中读取
     long_description_content_type='text/markdown',  # 详细描述的格式，这里是Markdown
     author='Elias Liu 刘益廷',  # 作者名称
     author_email='liuyiting120@126.com',  # 作者邮箱
     url='https://github.com/tenbj/elias',  # 项目的URL
@@ -34,14 +34,15 @@
         'clickhouse_sqlalchemy',
         'clickhouse_driver',
         # 'odps',
         'bs4',
         'selenium',
         'loguru',
         # 'googletrans',
+        'ollama',
         'pillow',
         'opencv-python'
     ],
     classifiers=[  # 包的分类标签
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```


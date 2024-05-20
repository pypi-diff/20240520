# Comparing `tmp/pipy-test-xiaoqiang-1.0.1.tar.gz` & `tmp/pipy-test-xiaoqiang-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipy-test-xiaoqiang-1.0.1.tar", last modified: Mon May 20 07:25:47 2024, max compression
+gzip compressed data, was "pipy-test-xiaoqiang-1.1.0.tar", last modified: Mon May 20 09:21:06 2024, max compression
```

## Comparing `pipy-test-xiaoqiang-1.0.1.tar` & `pipy-test-xiaoqiang-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-20 07:25:47.643521 pipy-test-xiaoqiang-1.0.1/
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      571 2024-05-20 07:25:47.643338 pipy-test-xiaoqiang-1.0.1/PKG-INFO
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       48 2024-05-20 07:13:42.000000 pipy-test-xiaoqiang-1.0.1/README.md
-drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-20 07:25:47.641986 pipy-test-xiaoqiang-1.0.1/pipy_test_xiaoqiang/
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)        0 2024-05-20 06:56:45.000000 pipy-test-xiaoqiang-1.0.1/pipy_test_xiaoqiang/__init__.py
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      519 2024-05-20 07:05:57.000000 pipy-test-xiaoqiang-1.0.1/pipy_test_xiaoqiang/main.py
-drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-20 07:25:47.643088 pipy-test-xiaoqiang-1.0.1/pipy_test_xiaoqiang.egg-info/
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      571 2024-05-20 07:25:47.000000 pipy-test-xiaoqiang-1.0.1/pipy_test_xiaoqiang.egg-info/PKG-INFO
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      250 2024-05-20 07:25:47.000000 pipy-test-xiaoqiang-1.0.1/pipy_test_xiaoqiang.egg-info/SOURCES.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)        1 2024-05-20 07:25:47.000000 pipy-test-xiaoqiang-1.0.1/pipy_test_xiaoqiang.egg-info/dependency_links.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       20 2024-05-20 07:25:47.000000 pipy-test-xiaoqiang-1.0.1/pipy_test_xiaoqiang.egg-info/top_level.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       38 2024-05-20 07:25:47.643579 pipy-test-xiaoqiang-1.0.1/setup.cfg
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)     1155 2024-05-20 07:16:10.000000 pipy-test-xiaoqiang-1.0.1/setup.py
+drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-20 09:21:06.813254 pipy-test-xiaoqiang-1.1.0/
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      683 2024-05-20 09:21:06.813061 pipy-test-xiaoqiang-1.1.0/PKG-INFO
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       48 2024-05-20 07:13:42.000000 pipy-test-xiaoqiang-1.1.0/README.md
+drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-20 09:21:06.810765 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang/
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)        0 2024-05-20 06:56:45.000000 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang/__init__.py
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       82 2024-05-20 09:08:07.000000 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang/cli.py
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      519 2024-05-20 07:05:57.000000 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang/main.py
+drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-20 09:21:06.812724 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang.egg-info/
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      683 2024-05-20 09:21:06.000000 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang.egg-info/PKG-INFO
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      365 2024-05-20 09:21:06.000000 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)        1 2024-05-20 09:21:06.000000 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       56 2024-05-20 09:21:06.000000 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang.egg-info/entry_points.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)        6 2024-05-20 09:21:06.000000 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang.egg-info/requires.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       20 2024-05-20 09:21:06.000000 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang.egg-info/top_level.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       38 2024-05-20 09:21:06.813331 pipy-test-xiaoqiang-1.1.0/setup.cfg
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)     1028 2024-05-20 09:21:03.000000 pipy-test-xiaoqiang-1.1.0/setup.py
```

### Comparing `pipy-test-xiaoqiang-1.0.1/PKG-INFO` & `pipy-test-xiaoqiang-1.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: pipy-test-xiaoqiang
-Version: 1.0.1
+Version: 1.1.0
+Summary: A short description of your project
+Home-page: https://github.com/yourusername/my_project
 Author: Ma Xiaoqiang
 Author-email: 851788096@qq.com
-License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+用于定义ETL处理前期的日志驱动阶段
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pipy-test-xiaoqiang-1.0.1/pipy_test_xiaoqiang/main.py` & `pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang/main.py`

 * *Files identical despite different names*

### Comparing `pipy-test-xiaoqiang-1.0.1/pipy_test_xiaoqiang.egg-info/PKG-INFO` & `pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: pipy-test-xiaoqiang
-Version: 1.0.1
+Version: 1.1.0
+Summary: A short description of your project
+Home-page: https://github.com/yourusername/my_project
 Author: Ma Xiaoqiang
 Author-email: 851788096@qq.com
-License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+用于定义ETL处理前期的日志驱动阶段
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

